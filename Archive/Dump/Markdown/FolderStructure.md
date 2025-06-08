## **`FolderStructure.md` (Boilerplate Archive Overview, Version: 1.0)**

> Outlines the folder structure of this boilerplate template archive.  
> Its purpose is to help organize templates and supporting materials for initiating new projects.

## Root Level (`/`) - (Root of "BoilerPlate" directory)

- **`Archive/`** - Main directory for all boilerplate templates & support files.  
  (Designed to be moved into new projects during setup & then gitignored).
  - **`Context/`** - Storage for large text files/LLM reference material.
  - **`Dump/`** - General scratchpad; separates from `Context/`.
    - **`Examples/`** - Stores useful code snippets, UI mockups, or other illustrative examples.
    - **`Markdown/`** - Main directory for all Markdown files including Master templates & TODO's.
      - **`Core/`** - Houses subdirectories for planning core functionalities.
        - `Admin/`
          - _(Example: Create `TODO-AdminPanel.md` here from `TODO-Example.md`)_
        - `Auth/`
          - _(Example: Create `TODO-ReturningUserLogin.md` here from `TODO-Example.md`)_
        - `Dashboard/`
          - _(Example: Create `TODO-DashboardLayout.md` here from `TODO-Example.md`)_
        - `User/`
          - _(Example: For a simple settings page, create `TODO-Settings.md` here from `TODO-Example.md`.)_
          - _(For complex settings, create a `Settings/` subdirectory, then within it:_
            - `Settings/`
              - `TODO-SettingsShell.md` _(For the main shell, from `TODO-Example.md`)_
              - `TODO-Settings-PersonalInfo.md` _(For a specific tab, from `TODO-Example.md`)_
              - `...etc. for other tabs...`)\*
      - **`DevOps/`** - Houses subdirectories for DevOps planning.
        - _(Example: Create `TODO-CICD-Setup.md` here from `TODO-Example.md`)_
      - **`Features/`** - Houses subdirectories for specific application feature planning.
        - `ExampleFeature/` - Illustrates documentation for a potentially complex feature.
          - `TODO-ExampleFeature.md` _(The main plan for this example feature,  
             created from the master `TODO-Example.md` template and filled out)._
          - `TODO-ExampleFeature-UI.md` _(Illustrative: a separate detailed UI spec)._
          - `TODO-ExampleFeature-Backend.md` _(Illustrative: a separate detailed backend spec)._
      - **`Platform/`** - Houses subdirectories for platform-wide concerns.
        - _(Example: Create `TODO-GlobalErrorHandling.md` here from `TODO-Example.md`)_
      - **`StartPrompt.md`** - Master template for project initiation with an AI.
      - **`TODO.md`** - Master template for a project's main TODO list (MVP & Future Features).
      - **`TODO-Example.md`** - Master 10-point template for any detailed feature specification.
      - **`FolderStructure.md`** - Boilerplate template to define a _new project's_ code/doc folder structure.
      - **`initProject.md`** - Step-by-step guide for new project setup using this archive.

## Notes

- Master templates (`StartPrompt.md`, `TODO.md`, `TODO-Example.md` [the generic 10-point one], `FolderStructure.md`, `initProject.md`) are located in `Archive/Dump/Markdown/`.
- To plan a new feature/component:
  1.  Create the appropriate subdirectory if it doesn't exist (e.g., `Features/MyNewFeature/` or `Core/User/Settings/`).
  2.  Copy the master `Archive/Dump/Markdown/TODO-Example.md` into that subdirectory.
  3.  Rename it appropriately (e.g., `TODO-MyNewFeature.md` or `TODO-Settings-PersonalInfo.md`).
  4.  Collaborate with the AI LLM to Build it up & Fill it out.
  5.  If the feature/component is complex, create additional specialized planning documents within its subdirectory.
