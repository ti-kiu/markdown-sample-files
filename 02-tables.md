<!-- Expected: aligned columns (left/center/right), headerless rows, empty cells, escaped pipes, very wide table, long wrapping cells, in-cell code/link/bold -->

# Tables

## Alignment

| Left | Center | Right |
|:-----|:------:|------:|
| a | b | c |
| longer cell | 1 | 100 |

## Empty cells & escapes

| Col 1 | Col 2 | Col 3 |
|-------|-------|-------|
| filled |  | also filled |
| a \| b | backslash-escaped pipe | ok |

## Wide table (wraps on narrow viewports)

| ID | Name | Description | Status | Owner | Created | Notes |
|----|------|-------------|--------|-------|---------|-------|
| 1 | Renderer alpha | Handles the full CommonMark 0.31 suite plus GFM tables | ✅ | @ana | 2026-01-12 | Fast |
| 2 | Renderer beta | Mermaid diagrams break when a `<br>` appears inside a node label; needs sanitiser update | ⚠️ | @bo | 2026-02-03 | Blocked on upstream |
| 3 | Legacy shim | Converts HTML tables to Markdown via `pandoc`; round-trip loses alignment | ❌ | @cy | 2025-11-20 | Deprecate |

## In-cell formatting

| Feature | Example | Supported |
|---------|---------|-----------|
| Code | `inline code` in a cell | ✅ |
| Link | [docs](https://example.com) | ✅ |
| Bold | **strong** text | ✅ |
| Math | `$x^2$` | renderer-specific |
