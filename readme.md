# Spec-Kit Plus Installation & Setup (Windows)

Spec-Kit Plus is a structured AI development framework that organizes
your workflow using **Spec-Driven Development (SDD)**: **Specifications
→ Plans → Tasks → Code**.

This README provides a complete, correct, and ready-to-download setup
guide for Windows users.

------------------------------------------------------------------------

## Prerequisites

Ensure the following before you begin:

-   **Python 3.12 or higher**

    ``` powershell
    python --version
    ```

-   **Optional:** Git for version control

    ``` powershell
    git --version
    ```

------------------------------------------------------------------------

## Install Spec-Kit Plus CLI

Open **PowerShell (Run as Administrator)** and install:

``` powershell
pip install specifyplus
```

Verify the installation:

``` powershell
specifyplus --version
```

Check available command options:

``` powershell
specifyplus --help
```

------------------------------------------------------------------------

## Initialize a New Project

Navigate to your desired folder:

``` powershell
cd C:\path\to\your\project
```

Initialize a new Spec-Kit Plus project:

``` powershell
specifyplus init my-project-name
```

During setup, you will select:

-   Your AI tool (Claude Code or Gemini CLI)
-   Terminal type (PowerShell recommended)

Move into your new project:

``` powershell
cd my-project-name
```

------------------------------------------------------------------------

## Verify Project Structure

After initialization, your project should contain:

    my-project-name/
    ├── .claude/
    │   └── commands/
    ├── .specify/
    │   ├── memory/
    │   ├── scripts/
    │   └── templates/
    ├── .git/
    ├── CLAUDE.md
    ├── README.md
    └── .gitignore

As you proceed, directories such as `specs/` and `history/` will appear.

------------------------------------------------------------------------

## Test Spec-Kit Plus Commands

Launch your chosen AI tool:

``` powershell
claude
# or
gemini
```

Then type:

    /sp.

You should see commands like:

-   `/sp.constitution`
-   `/sp.specify`
-   `/sp.clarify`
-   `/sp.plan`
-   `/sp.adr`
-   `/sp.tasks`
-   `/sp.implement`
-   `/sp.phr`

If these appear, Spec-Kit Plus is working properly.

------------------------------------------------------------------------

## Update Spec-Kit Plus

Keep your installation up to date:

``` powershell
pip install --upgrade specifyplus
```

------------------------------------------------------------------------

## Common Pitfalls

-   Installing only the AI tool --- Spec-Kit Plus must be installed
    separately.
-   Running Python older than 3.12.
-   Manually creating folders instead of using `specifyplus init`.

------------------------------------------------------------------------

## Quick Start Commands

``` powershell
python --version
pip install specifyplus
specifyplus init my-first-project
cd my-first-project
claude   # or gemini
/sp.
```

You are now ready to build structured AI projects using Spec-Kit Plus!
