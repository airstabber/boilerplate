## **`initProject.md` (Guide to Initialise a New Project, Version: 1.0)**

## 1. Purpose

This document outlines the standardized procedure for initiating a new software  
 by cloning and utilizing the templates within this boilerplate Git repository.  
Following these steps ensures consistency and a well-organized start to project planning and development.

## 2. Prerequisites

- Git installed and configured.
- Node.js and a package manager (pnpm, yarn, or npm) installed (if applicable to chosen stack for the new project).
- Any other CLI tools required for your new project's chosen technology stack.
- A Git hosting account (e.g., GitHub, GitLab) for your new project's remote repository.

## 3. Boilerplate Repository Overview

This repository (`airstabber/boilerplate`) contains master templates in its `Archive/Markdown/` subdirectory:  
`StartPrompt.md`, `TODO.md`, `TODO-Example.md` (for detailed features),  
 `FolderStructure.md` (template for project structure), and `initProject.md` (this guide).

## 4. New Project Initialization Steps

1.  **Clone This Boilerplate Repository to Your New Project's Name:**

    - Navigate to the directory where you want to create your new project.
    - Run:
      ```
      git clone https://github.com/airstabber/boilerplate.git MyNewAwesomeAppName
      cd MyNewAwesomeAppName
      ```
    - This creates `MyNewAwesomeAppName/` containing all the boilerplate files (including `Archive/`).

2.  **Decouple from Boilerplate Git History (Crucial for a New Project):**

    - You want `MyNewAwesomeAppName` to have its _own independent Git history_, not the history of the boilerplate.
    - Inside `MyNewAwesomeAppName/`, remove the boilerplate's Git tracking:
      ```
      rm -rf .git
      ```
    - Initialize a fresh Git repository for your new project:
      ```
      git init .
      ```

3.  **Initialize Core Technology Stack:**

    - Run your stack's initializer to use the _current directory_ (`MyNewAwesomeAppName/`) as the project root.
    - **Example (for T3 Stack):**
      ```
      pnpx create-t3-app@latest .
      ```
    - Follow the CLI prompts for your new project.

4.  **Configure `.gitignore` for the New Project:**

    - Ensure a `.gitignore` file exists in `MyNewAwesomeAppName/`.
    - Add the line `Archive/` to this file. (The `Archive/` directory, containing copies of the boilerplate templates,  
      is for this project's internal planning and should not be part of its primary codebase commits).
    - Add other necessary ignores (`node_modules/`, `.env`, etc.).
    - Save `.gitignore`.

5.  **Initial Git Commit for the New Project:**

    - Stage all files:
      ```
      git add .
      git commit -m "Initial commit - [Tech Stack] setup and project planning boilerplate from template"
      ```
    - (Recommended) Create a new remote repository on GitHub/GitLab for `MyNewAwesomeAppName` and push:
      ```
      # Example GitHub commands
      # git remote add origin <new_project_remote_repo_url>
      # git branch -M main
      # git push -u origin main
      ```

6.  **Customize Planning Documents for the New Project:**

    - Navigate into `MyNewAwesomeAppName/Archive/Markdown/`.
    - Edit `StartPrompt.md`, `TODO.md`, and `FolderStructure.md` to reflect the specifics  
       of `MyNewAwesomeAppName` (update project names, versions in headers, fill in content).
    - `TODO-Example.md` is your template for feature planning within this project.
    - `initProject.md` (this guide) is now a reference within this project.

7.  **Begin Project Planning & Development:**
    - Flesh out the project-specific `StartPrompt.md` and `TODO.md`.
    - Use `TODO-Example.md` for detailed feature planning.

## 5. Notes/Tips

- To get updates to the _master boilerplate templates_ in the future, you would `git pull` in your _original local clone_  
  of the `airstabber/boilerplate` repository (the one not tied to a specific project), or re-clone it.  
  Then, you could manually copy updated templates into ongoing projects if desired, or use them for new projects.
- The `Archive/` folder _within your actual project_ (`MyNewAwesomeAppName/Archive/`)  
  is for that project's internal planning and is ignored by its main Git repository.
