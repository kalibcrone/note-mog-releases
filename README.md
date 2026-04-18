# note-mog-releases

**Note Mog - Quick Note Taker for Claude Code Developers**

Official Note Mog releases repo for Note Mog, the quick note taker for Claude Code developers - Take notes any time, organize them automatically within your projects, and run queued up Claude Code prompts based on your todo and bug notes from the day by referencing a design document to save tokens, or by scanning your entire project for more accuracy.

Intended to group together lots of small tasks and bug fixes together.  Not recommended for large feature changes.

Optionally, use for your daily tasks by creating "projects" as 

**How to use**

`Ctrl + Shift + Space`  ===== Take a quick note

`Ctrl + Shift + L`      ===== Open Note Pad Control Panel

**Features**

* Quickly pop up a light weight note taker
* Multi-select groupings of todos, bugs, and design changes to queue up for taking action on all of them
* Select actions such as Create/Update design document for project, complete TODOs, Fix Bugs, or Run full pipeline

**Other**

* Tip: When taking a note, type @project-name to write a note for your particular project
* Tip: When taking a quick note, type: "todo", "bug", "idea", "feedback" at the beginning to label your note (Optionally, write nothing and AI will decide for you)
* Tip: Shift + Enter to add multiple notes in the quick note taker pop up
* Tip: Break apart your project into multiple features within note mog, where each feature of a project is it's own "project"
* Tip: You don't technically need an API key or a Project Path to use the note taker for some other category, such as @Grocery-List or @Friday-Meeting notes
* Note: This app is intended for Claude Code Developers. You must use your own Claude API key and Claude Code account for documentation creation and todo/bug prompts from your notes

**Security & privacy**

* Note Mog has no server, database, or telemetry — your key is never sent to the developer or any third party, and it is not bundled with the app.
* Your Claude API key is saved only to a local SQLite file on your machine and encrypted at rest using Windows' Data Protection API (DPAPI), tied to your Windows user account.
* The key is transmitted only to Anthropic (api.anthropic.com) over HTTPS, and only when you generate docs or classify a note.
* If OS-level encryption is unavailable on your system, Note Mog falls back to base64-obfuscated storage and shows a warning in Settings so you know.
