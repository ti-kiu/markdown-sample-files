<!-- Expected: H1–H6, bold/italic/strikethrough, ordered/unordered/nested lists, blockquotes (incl. nested), links, reference links, images, inline code, horizontal rules -->

# GFM Basics

## Headings

Six levels of heading, then paragraph text with **bold**, _italic_, ***bold italic***, ~~strikethrough~~, and `inline code`.

## Lists

Unordered:

- First item
- Second item
  - Nested under second
    - Deeper still
- Third item with a [link](https://example.com)

Ordered:

1. Step one
2. Step two
   1. Sub-step
3. Step three

Task list:

- [x] Completed task
- [ ] Pending task
- [ ] Blocked task

## Blockquotes

> A plain quote with **emphasis**.
>
> > Nested quote.
> >
> > > Triple nesting.

## Links & Images

Inline: [Example](https://example.com "title attribute")

Reference style:

[Markdown Guide][mdg]

Auto-link: <https://markdownfileviewer.com>

[mdg]: https://www.markdownguide.org

![A decorative image](https://picsum.photos/seed/mdsample/320/120 "Image title")

## Inline code & escapes

Use `npm install` to start. Escape pipes and brackets: \| \[ \] \*. Backslash itself: \\.

## Horizontal rules

---

***

___
