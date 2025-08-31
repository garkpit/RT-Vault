AI can't think large enough for the entire project, so we have to split it into parts.

Use Feature Slice Design

Code in progress is currently in Jay's **sv5vax** repository
...where there are an awful lot of branches and commits and long messages, because I was documenting what was working and what was not.

One large feature slice has been done (ish). See the 2025-08-31 milestone folder for details.

Plan forwards:
* More feature slices
* Do one simple Recipe, as a template/lesson for future recipes

(
We already have 2 slices that would make an interesting recipe: 
VideoFabricWithZoom + MediaMetadata = Video + Drawing + hierarchy of timelines that you can CRUD timelineRange blobs on.
Could be done, but functionally "not exactly what we want"
Leave it - for now
)

## Features wishlist
Review the Ross and Jay brainstorming PRD. And, invent whatever others you want.
* Comments
	* dto = color, user, comment string (markdown? use the mdsvex library, timecodeIn, timecodeOut, isTodo
	* with interface hook to 
		* attach Fabric drawing
		* attach video 
		* version
		* etc
* User Management, Teams, and Permissions
* Workflow
* Versions
* Storage & Retrieval (abstraction - support any e.g. database, API, file system, browser storage, ...)
* Alternative media: PDFs, Image(s), etc. + Fabric drawing tools overlaid

Basically, loosely coupled, strongly typed :LiLaugh:

## More Drawing things needed
The Drawing tools in VideoFabricWithZoom are missing
* Color options
* Fill options
* Onion skin
* Laser pointer
* Highlighter
* etc
Easiest is to add them to the feature (there is room). More interesting is to write them as a separate feature + link the two in a Recipe.

## Writing Recipes
You want to be able to export/import just the interfaces of the Features you are using. Then AI only has to read as far as the interface definition. Whenever you find you are missing a hook then you branch out to a new mini-PRD to add the necessary logic to the feature and export the hook you need.




