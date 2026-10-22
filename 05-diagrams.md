<!-- Expected: Mermaid flowchart/sequence/gantt/state/pie; renderers without Mermaid show a code block instead — that is acceptable fallback -->

# Mermaid Diagrams

## Flowchart

```mermaid
flowchart TD
    A[Open .md file] --> B{Client-side?}
    B -- yes --> C[Parse with marked]
    B -- no --> D[Upload → reject]
    C --> E[Render HTML]
    E --> F[TOC + anchors]
```

## Sequence

```mermaid
sequenceDiagram
    participant U as User
    participant V as Viewer (browser)
    U->>V: drop file.md
    V->>V: FileReader → parse → render
    V-->>U: formatted HTML + scrollable TOC
```

## Gantt

```mermaid
gantt
    title Launch plan
    dateFormat  YYYY-MM-DD
    section Build
    Parser hardening   :a1, 2026-01-01, 14d
    Mermaid support    :a2, after a1, 7d
    section Launch
    Directory listings :b1, 2026-01-20, 10d
```

## State

```mermaid
stateDiagram-v2
    [*] --> Idle
    Idle --> Loading: open file
    Loading --> Rendered: success
    Loading --> Error: parse fail
    Rendered --> Idle: close
```

## Pie

```mermaid
pie showData
    title Traffic sources
    "Search" : 62
    "Directories" : 9
    "GitHub lists" : 7
    "Direct" : 22
```
