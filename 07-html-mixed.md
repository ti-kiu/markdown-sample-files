<!-- Expected: raw block-level HTML, inline HTML inside paragraphs, details/summary disclosure, iframe blocked by sanitizers, no XSS execution (script tag must not run) -->

# Mixed HTML

Block-level div:

<div class="callout" style="padding:8px;border-left:4px solid #b95235">
  This is raw HTML, not Markdown. <strong>Bold still works.</strong>
</div>

Inline HTML in a paragraph: text with a <sub>subscript</sub> and <sup>superscript</sup> and a <kbd>⌘</kbd> + <kbd>K</kbd> shortcut.

## Details disclosure

<details>
<summary>What happens to HTML inside <code>&lt;details&gt;</code>?</summary>

Markdown inside the body **may or may not** render, depending on the parser. GFM renders it; some strict CommonMark configs do not.

</details>

## Should be neutralised, not executed

<script>alert('must not run')</script>

<img src="x" onerror="alert('must not run')">

A secure viewer (like [Markdown File Viewer](https://markdownfileviewer.com)) strips or disables these.

## Table in HTML next to Markdown table

<table><tr><td>HTML cell</td><td>another</td></tr></table>

| Markdown | table |
|----------|-------|
| side by side | ok |
