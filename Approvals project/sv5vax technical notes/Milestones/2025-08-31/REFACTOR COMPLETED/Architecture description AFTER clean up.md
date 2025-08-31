(same prompt)

---

## VideoFabricWithZoom Architecture Overview

This feature implements a sophisticated video annotation system with zoom/pan capabilities, following a **layered, reactive architecture** with clear separation of concerns.

### 🏗️ Core Architecture Patterns

#### 1. **Layered Rendering Architecture**

```
┌─────────────────────────────────────┐
│       ZoomContainer (Transform)     │  <- Handles zoom/pan transforms
├─────────────────────────────────────┤
│   VideoLayer  │   CanvasLayer       │  <- Synchronized layers
│   (Video.js)  │   (Fabric.js)       │
└─────────────────────────────────────┘
│               Minimap               │  <- Navigation overlay 
└─────────────────────────────────────┘     (outside transform)
```

- **Video Layer**: Base layer for video playback
- **Canvas Layer**: Transparent overlay for annotations
- **Transform Container**: Applies zoom/pan to both layers simultaneously
- **Minimap**: Navigation UI positioned outside the transform

#### 2. **State Management Architecture**

Using **Svelte 5 Runes** with class-based reactive stores:

```typescript
// Three primary state domains
videoState    → Video playback, dimensions, player reference
canvasState   → Drawing tools, annotations, Fabric canvas
transformState → Zoom level, pan position, boundaries
```

**Key Design Decisions:**

- **Single Source of Truth**: Each state domain manages its own concerns
- **Reactive Derivations**: Complex calculations use `$derived` for automatic updates
- **Effect-based Synchronization**: `$effect` runes coordinate cross-store updates

#### 3. **Controller Pattern**

Controllers act as **orchestrators** between stores and components:

```
DrawingController  → Manages drawing operations and tool behaviors
ZoomController     → Handles zoom/pan logic with animations
PanController      → Manages pan gestures and boundaries  
VideoCanvasSync    → Synchronizes video and canvas states
MinimapController  → Handles minimap interactions
```

#### 4. **Coordinate System Architecture**

The feature manages **four coordinate spaces**:

1. **Video Space**: Original video dimensions (e.g., 1920×1080)
2. **Display Space**: Scaled video in container (with baseZoom)
3. **Transform Space**: After zoom/pan transformations
4. **Minimap Space**: Scaled representation (max 200×150)

```typescript
// Coordinate transformation flow
Video Coords → Display Coords (baseZoom) → Transform Coords (zoom/pan) → Screen Coords
                                               ↓
                                         Minimap Coords
```

### 📁 Directory Structure & Responsibilities

```
videoFabricWithZoom/
├── components/           # UI Components
│   ├── VideoCanvas/     # Core video/canvas layers
│   ├── Controls/        # User controls (zoom, tools, colors)
│   ├── Navigation/      # Minimap and viewport
│   └── Diagnostics/     # Memory and performance monitoring
│
├── controllers/         # Business Logic Orchestrators
│   ├── DrawingController    # Drawing operations
│   ├── ZoomController       # Zoom/pan calculations
│   └── VideoCanvasSync      # Layer synchronization
│
├── stores/             # Reactive State Management
│   ├── videoState          # Video player state
│   ├── canvasState         # Canvas and drawing state
│   └── transformState      # Zoom/pan transform state
│
├── services/           # External Service Integration
│   ├── VideoService        # Video loading/processing
│   └── AnnotationService   # Annotation persistence
│
├── utils/              # Shared Utilities
│   ├── performance         # Throttle, debounce, RAF
│   ├── canvasHelpers       # Fabric.js utilities
│   └── gestureHandlers     # Touch/mouse normalization
│
└── types/              # TypeScript Definitions
    ├── video.ts            # Video-related types
    ├── canvas.ts           # Canvas/drawing types
    └── transform.ts        # Transform/viewport types
```

### 🔄 Data Flow Architecture

#### 1. **User Input Flow**

```
User Input → Controller → State Store → Components (via reactivity)
                ↓
        Side Effects ($effect) → Canvas/Video Updates
```

#### 2. **Transform Synchronization**

```
Transform Change → transformState.setZoom()
                        ↓
                   $effect (reactive)
                   ↙          ↘
        Update Video Style   Update Canvas Transform
                   ↘          ↙
                  Minimap Updates
```

#### 3. **Drawing Operations Flow**

```
Tool Selection → canvasState.setActiveTool()
                        ↓
Mouse Events → DrawingController.handleDrawing()
                        ↓
              Fabric.js Object Creation
                        ↓
              canvasState.addAnnotation()
```

### 🎯 Key Architectural Decisions

#### 1. **Separation of Concerns**

- **Presentation**: Svelte components handle UI only
- **Business Logic**: Controllers manage complex operations
- **State**: Stores are the single source of truth
- **Side Effects**: Managed via `$effect` runes

#### 2. **Performance Optimizations**

- **Throttled Updates**: 60fps cap on expensive operations
- **Frame Caching**: Minimap caches video frames
- **Selective Rendering**: Only update changed elements
- **Memory Management**: Explicit cleanup in destroy methods

#### 3. **Reactive Architecture Benefits**

- **Automatic Updates**: Changes propagate without manual subscription
- **Derived Values**: Complex calculations update automatically
- **Predictable State**: Unidirectional data flow
- **Type Safety**: Full TypeScript coverage

#### 4. **Modularity & Extensibility**

- **Plugin-like Tools**: Easy to add new drawing tools
- **Service Layer**: Abstract external integrations
- **Dependency Injection**: Components receive dependencies via props
- **Feature Flags**: Runtime feature toggling

### 🔌 Integration Points

1. **Video.js Integration**
    
    - Wrapped in VideoLayer component
    - Events proxied to videoState
    - Custom controls disabled (using own UI)
2. **Fabric.js Integration**
    
    - Canvas instance managed by canvasState
    - Custom event handlers in canvasHelpers
    - Object serialization for persistence
3. **Browser APIs**
    
    - ResizeObserver for responsive sizing
    - IntersectionObserver for visibility
    - Pointer Events for unified input
    - RAF for smooth animations

### 🎨 Design Patterns Used

1. **Observer Pattern**: Reactive stores with subscribers
2. **Strategy Pattern**: Swappable drawing tools
3. **Command Pattern**: Undo/redo operations (in services)
4. **Facade Pattern**: Controllers simplify complex operations
5. **Singleton Pattern**: Global state stores
6. **Factory Pattern**: Annotation object creation

### 🚀 Scalability Considerations

- **Lazy Loading**: Components loaded on demand
- **Code Splitting**: Features as separate chunks
- **Worker Support**: Ready for WebWorker integration
- **Modular Architecture**: Easy to add/remove features
- **Performance Monitoring**: Built-in diagnostics

This architecture provides a robust foundation for a complex video annotation system while maintaining clarity, performance, and extensibility.