# Markdown Sample Files

Practical sample documents and test fixtures for Markdown viewers, parsers, renderers, and static-site tooling. Each file isolates one feature area, so you can see (or test) exactly how a renderer handles it.

**Quick preview:** open any file here directly in [Markdown File Viewer](https://markdownfileviewer.com) — it renders `.md` files entirely in your browser; nothing is uploaded to a server.

## What's inside

| File | Covers |
|------|--------|
| `01-gfm-basics.md` | Headings, emphasis, lists, blockquotes, links, images, inline code |
| `02-tables.md` | Aligned, wide, and empty-cell GitHub-Flavored tables |
| `03-task-lists.md` | Flat and nested task lists with mixed states |
| `04-code-blocks.md` | Fenced blocks in 10 languages, indented blocks, metadata strings |
| `05-diagrams.md` | Mermaid flowchart, sequence, gantt, state, pie |
| `06-footnotes-and-abbr.md` | Footnotes and abbreviation syntax |
| `07-html-mixed.md` | Raw HTML blocks, `<details>` accordions, inline HTML |
| `08-long-article.md` | Deep heading tree for TOC / scroll-spy testing |
| `09-edge-cases.md` | CJK text, emoji, escapes, autolinks, hard breaks, long lines |
| `samples/readme-style.md` | A realistic project README (badges, install, usage, license) |
| `samples/blog-post.md` | Long-form prose with images and a pull quote |
| `fixtures/legacy.sample.markdown` | `.markdown` extension check |
| `fixtures/plain.txt` | `.txt` fallback rendering check |
| `fixtures/empty.md` | Near-empty document check |

## Using these files

- **Rendering checks** — drop any file into a Markdown viewer and compare the output.
- **Parser tests** — each numbered file opens with a comment listing expected elements.
- **UI stress tests** — `09-edge-cases.md` and `08-long-article.md` are deliberately awkward.

## Contributing

Pull requests welcome. Keep each file focused on one Markdown feature family.

## License

CC0 — public domain; no attribution required for the sample content.
