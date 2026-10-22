<!-- Expected: inline footnotes [^1], named references [^note], backlink arrows, multi-paragraph footnote, abbreviation *[HTML]: syntax (GFM does not support abbr by default — check fallback) -->

# Footnotes

A claim with a reference[^1], a named note[^later], and an inline note.

Inline:^[This footnote is defined right here in the sentence.]

More text to push the footnote markers down[^1].

## Expected behaviour

Markers should become superscript links; the footnote list renders at the bottom with backlinks. Renderers without footnote support should show the literal `[^1]` — never crash.

[^1]: First footnote, single paragraph.

[^later]:
    A multi-paragraph footnote.

    The second paragraph keeps the indentation so it stays part of the note.

    - including a list
    - inside the note

## Abbreviations (extension syntax, often unsupported)

*[HTML]: HyperText Markup Language
*[GFM]: GitHub Flavored Markdown

The HTML spec predates GFM.
