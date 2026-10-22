<!-- Expected: CJK line breaking, RTL text, emoji sequences, escaped markdown chars, autolinks, hard breaks (two spaces & backslash), 500-char single line, tabs inside code -->

# Edge Cases

## Unicode & scripts

中文、日本語、한국어 mixed inline text renders without breaking words. 这是一段中文，混入 English 和 emoji 🎉.

العربية and עברית — right-to-left scripts inside an LTR document.

## Emoji

Flags: 🇯🇵 🇩🇪 🇺🇸 · Skin tones: 👋🏽 👩🏾‍💻 · ZWJ families: 👨‍👩‍👧‍👦 · Keycaps: 1️⃣

## Escapes — should render literally, not as syntax

\*not italic\* \#not heading \[not link\] \`not code\` \\_not emphasis\\_ \~\~not strike\~\~ 4\|5 in-cell

## Hard breaks

Line one with two trailing spaces  
Line two — same paragraph, hard break.

Line A with backslash break\
Line B — same paragraph.

## Autolinks

<https://example.com> and <mailto:hello@example.com> and www.bare-domain.com (GFM autolinks bare www).

## Very long line (no spaces for ~300 chars, tests overflow handling)

AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA

## Tabs & windows line endings

Indented block below uses real tabs:

	tabbed line one
	tabbed line two

## Mixed inline emphasis

**bold with _nested italic_ inside**, and _italic with **nested bold**_, and ***both at once***, and ****empty emphasis****, and *unclosed emphasis.

## Setext headings vs ATX

Setext H1
=========

Setext H2
---------

## Normal paragraph after everything

Done.
