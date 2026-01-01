# GitHub Copilot / AI Agent Instructions

**Purpose:** Short, actionable guidance so an AI coding agent can be immediately productive in this repository.

## Project summary
- Minimal Java example: single-file CLI app. Primary file: `QuickStart.java` (contains a `public static void main`).
- No build tool (Maven/Gradle) or test framework present; sources live at repository root.

## How to build & run (explicit commands)
- Compile: `javac QuickStart.java`
- Run: `java QuickStart` (run from the repository root)
- In VS Code: use the Java Extension Pack (Run/Debug on `QuickStart` main class)

## Formatting & IDE settings
- Project provides a Java formatter profile: `.vscode/java-formatter.xml` and VS Code setting `.vscode/settings.json` pointing to it.
- Apply formatting using the editor's Java formatter (Eclipse/VSCode Java formatter) so formatting stays consistent (4-space indent, line wrap ≈120 cols).

## Conventions & patterns specific to this repo
- No package declarations used; files live at repository root and assume default package.
- Main class is `QuickStart` and prints `Hello, World A` — prefer non-invasive edits (do not rename the main class unless adjusting all run/debug steps).
- Keep changes small and well-scoped; because there are no tests or CI, run manual compile+run after edits.

## Tests & CI
- No tests or CI configuration found. If adding functionality, include a simple test harness (JUnit) and a basic build file (Maven/Gradle) and add instructions to `README.md`.

## Useful examples for patching
- Small change example: to change program output, edit `QuickStart.java`, then run `javac QuickStart.java && java QuickStart`.
- Add a new module: create proper package structure (e.g., `src/main/java/...`) and add a `pom.xml` or `build.gradle` before introducing complex logic or tests.

## Safety & repository rules
- Repo is tiny and likely used for demos. Avoid adding unrelated heavy dependencies or complex scaffolding without owner approval.

## What I couldn't find (ask maintainers)
- Desired test framework and CI setup
- Commit message conventions or branching policy

---

If anything in this file is incomplete or you'd like more detail (example unit tests, a sample `pom.xml`, or preferred Java version), tell me which area to expand. Thanks!