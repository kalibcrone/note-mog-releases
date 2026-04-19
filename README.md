**Note Mog - Quick Note Taker for Claude Code Developers**

Official release repo for _Note Mog_ - Take notes and take action.

_Note Mog_ allows you to quickly take notes as you work, then _Note Mog_ organizes your tasks automatically within each of your projects and lets you run queued up Claude Code prompts based on your todo and bug tasks created from your notes by referencing a design document to save tokens, or by scanning your entire project for more accuracy.

Best used to group together lots of small todo tasks and bug fixes together.  Not recommended for large feature changes that require lots of back and forth iteration.

Optionally, use for your daily tasks by creating "projects" as misc life categories.

--------------------------------------------------------------------
<img width="731" height="505" alt="image" src="https://github.com/user-attachments/assets/26f3f28d-6ad7-4afb-b0e0-61b770b529ad" />

--------------------------------------------------------------------

<img width="794" height="494" alt="image" src="https://github.com/user-attachments/assets/a82be2b5-6d1c-480b-b884-da7d4a67d0d5" />

--------------------------------------------------------------------

<img width="794" height="493" alt="image" src="https://github.com/user-attachments/assets/3032ced3-d040-464b-9bf2-f5d968f5f360" />

--------------------------------------------------------------------

**How to Install**

Download and Simply open the setup .exe

Move the setup exe to another folder if it doesn't open in the downloads folder.

Windows may prevent the setup app from installing if you try to click it from inside the Downloads folder because the app is not signed. 

You may also get a security warning from Windows because the app is unsigned.  Select **More Info** then **Run Anyway** if that happens.


<img width="233" height="148" alt="image" src="https://github.com/user-attachments/assets/8ccc597d-221e-49ae-b111-6744557f5db5" />

 
**How to use**

`Ctrl + Shift + Space` - Take a quick note

`Ctrl + Shift + L` - Open Note Pad Control Panel

**Features**

* Quickly pop up a light weight note taker
* Multi-select groupings of todos, bugs, and design changes to queue up for taking action on all of them
* Select actions such as Create/Update design document for project, complete TODOs, Fix Bugs, or Run full pipeline

**Claude Skills**
Note mog comes bundled with 6 skills that run automatically when using the Note Mog action buttons

* note-generate-spec — Scans your codebase and generates (or updates) a living design document (design-spec.md)
* note-generate-bugs — Compiles your captured bug notes into a consolidated, severity-ranked bug report
* note-plan-todos — Groups your TODO notes into PR-sized implementation bundles ready to work through
* note-implement-todos — Works through your planned TODO bundles and commits each one separately
* note-fix-bugs — Reads your bug report and fixes each bug with a separate commit per fix
* note-run-pipeline (Work in Progress) — Runs the full workflow end-to-end: spec → plan → implement → fix bugs

Install them for each project

<img width="427" height="113" alt="image" src="https://github.com/user-attachments/assets/db79f535-ca78-4f4e-ba7d-52a8d9949efc" />


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
