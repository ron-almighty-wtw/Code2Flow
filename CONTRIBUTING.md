
# Contributing to Code2Flow

## Branch & PR
- Use feature branches: `feature/<project>-<module>-<diagram>`
- Include a screenshot or exported SVG in the PR description when feasible.
- Request review from maintainers.

## Folder & Naming
- Path: `projects/<project-name>/flows/<module>/`
- File: `<scope>_<feature>_<version>.mmd` (e.g., `auth_login_v1.mmd`)
- Keep `<scope>` and `<feature>` kebab-case; increment `<version>` when meaningfully changing logic.

## Required Metadata (top of file)
```mermaid
%% title: <Diagram Title>
%% author: <Your Name>
%% last-updated: YYYY-MM-DD
%% description: <One-sentence overview>
```

## Style Guidelines
- Default direction: `flowchart TD`
- Decision nodes: rhombus; processes: rectangles; terminators: rounded
- Keep edges labeled for clarity; avoid long sentences
- Group related nodes with `subgraph`
- For sequences: use `sequenceDiagram` with participants in logical order

## Validation Checklist
- ✅ Clear start/end nodes
- ✅ Every branch leads to a terminal or rejoins the main flow
- ✅ Labels are consistent and concise
- ✅ Metadata is present and accurate
- ✅ Matches folder/naming conventions

## Exports
- Optional: export PNG/SVG to `assets/exports/<project>/<diagram>.svg` for documentation or presentations.
