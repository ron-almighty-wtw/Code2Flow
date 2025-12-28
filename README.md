
# Code2Flow

**Code2Flow** is a centralized repository for visual documentation across projects, using Mermaid (`.mmd`) flowcharts. It transforms complex code logic into clear, easy-to-understand flowcharts, enabling faster comprehension and streamlined collaboration.
This repository serves as a visual reference for developers, architects, and stakeholders, making it easier to analyze workflows, debug processes, and maintain codebases efficiently.

Key Features:
Organized flowcharts for multiple projects
Visual representation of algorithms, workflows, and system logic
Improves readability and accelerates onboarding for new developers
Ideal for documentation, presentations, and technical reviews

## What this repo contains
- Organized Mermaid flowcharts (.mmd) grouped by project and module
- Templates and conventions for consistent diagram authoring
- Optional exports (PNG/SVG) for presentations and wiki pages

> Flowcharts are authored in a separate VS Code project, then manually imported here.

## Viewing Mermaid Charts in VS Code
1. Install following extensions in vscode plugins (ctrl + shift + x):
   - **mermaidchart.vscode-mermaid-chart**
   - **vstirbu.vscode-mermaid-preview**
2. Open any `.mmd` file and:
   - Use the extension’s preview command (e.g., `Markdown: Open Preview to the Side`)
   - Or insert Mermaid blocks in Markdown and preview them.

## Folder Structure
```
projects/<project-name>/flows/<module>/<ScopeFeature>.mmd
```
- **project-name**: kebab-case (e.g., `billing-service`)
- **module**: group related flows (e.g., `auth`, `pipeline`, `orders`)
- **ScopeFeature**: e.g., `AuthenticateUserFlowChart.mmd`

## Conventions
Each `.mmd` should start with metadata:
```mermaid
%% title: Login Flow
%% author: Ronald Jose
%% last-updated: 2025-12-16
%% description: User login path with validation and error branches.
```

Style guidelines (see `docs/conventions.md`):
- Use `flowchart TD` (top-down) for process flows unless left-right improves readability.
- Keep node labels concise; prefer verbs for actions and nouns for states.
- Color or style only for emphasis; avoid excessive decoration.

## Contributing
See `CONTRIBUTING.md` for:
- Naming rules
- Review checklist
- Diagram validation steps
- PR workflow

## License
MIT (or change to your preferred license)
