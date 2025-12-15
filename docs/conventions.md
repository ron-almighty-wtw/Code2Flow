
# Diagram Conventions

## Direction & Layout
- Prefer `flowchart TD` (top-down). Use `LR` when left-to-right improves readability.
- Use `subgraph` to group related steps.

## Node Types
- Start/End: rounded rectangles
- Process: rectangles
- Decision: diamonds
- External systems: cylinders or labeled nodes

## Labeling
- Use concise verbs for actions and nouns for states.
- Add edge labels for branch clarity (e.g., `Yes`/`No`).

## Metadata Header
Include at the top of each `.mmd` file:
```mermaid
%% title: <Diagram Title>
%% author: <Your Name>
%% last-updated: YYYY-MM-DD
%% description: <Short overview>
```

## Review Checklist
- Start and end are clear
- All branches resolve (terminate or merge)
- Consistent naming and casing
- No overlapping or ambiguous edges
- Updated `last-updated` date
