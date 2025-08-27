This has the definitions for all the MCPs I want CD to use.

As of end of August 2025

If/when this changes, I'll update here and let you guys know

## 1 - Desktop Commander
Gives CD access to your file system, and the ability to run things. With great power comes great responsibility... 
DO NOT blindly just give it blanket access to everything. Months from now Claude will start blackmailing you...
Fabulously useful, e.g. "My project Xyz is located here - /Full/Path/To/Your/Project/Root/Folder - please take a look and tell me what you see
Or
Please read through all the files in the docs/ folder
Or
My coding rules are in the .cursor/rules/ folder - please read every file there
Or
... you get the idea"

## 2 - Context 7 MCP
Currently the best resource for *How To Get An AI To Read The Latest Documentation For Xyz*
E.g. Tell it to "*Use Context 7 MCP to read the documentation for Svelte 5*" as part of your chat context setup. It is a doublebarrelled thing - first it find the library-id then it uses that to read the docs. You can ask it to just get the library-id and then check it is the right one - useful for things that have many similar names.

## 3 - Playwright MCP
Probably the best way to get CD to use a browser to test stuff that's just been written and confirm it is good, or tell it exactly how to get the error you are troubleshooting to appear and it will do it, reliably repeatable. Such a time saver.

# Here's the file you need
![[claude_desktop_config.json]]

On a Mac this goes in this folder: '/Users/YOUR-MAC-NAME/Library/Application Support/Claude'
it probably already exists. If it does then maybe you already have some MCPs! Well, if so, it's not hard figuring out how to merge this file with that file.
