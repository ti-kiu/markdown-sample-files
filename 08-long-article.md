<!-- Expected: TOC generation from 40+ headings across 5 levels; scroll-spy; heading anchor ids with CJK + punctuation; deep nesting -->

# Long Article — Heading Tree Stress Test

This document exists to stress table-of-contents generators, scroll-spy navs, and heading anchor schemes. It has 5 levels and ~40 headings.

## 1. Introduction

Lorem-style placeholder prose.

### 1.1 Background

Text.

#### 1.1.1 Early work

Text.

##### 1.1.1.1 The deepest level

Five levels deep — TOC tools must not overflow.

#### 1.1.2 Later work

### 1.2 Scope

## 2. Core concepts

### 2.1 Documents

#### 2.1.1 Structure

#### 2.1.2 Metadata

### 2.2 Rendering

#### 2.2.1 Inline spans

#### 2.2.2 Block elements

### 2.3 Extensions

#### 2.3.1 Tables

#### 2.3.2 Task lists

#### 2.3.3 Footnotes

## 3. Implementation notes

### 3.1 Parser

### 3.2 Sanitiser

### 3.3 Mermaid

## 4. Headings with special characters

### 4.1 CJK 中文标题 stress

### 4.2 French accents: résumé, naïve

### 4.3 Punctuation-heavy: what's this?! (really?)

#### 4.3.1 Emojis 🚀 in headings

### 4.4 Code in heading: `npm install` and HTML in heading

## 5. Duplicate headings

### 5.1 Setup

### 5.2 Setup

### 5.3 Setup

Anchor schemes should disambiguate duplicates (`setup`, `setup-1`, `setup-2` or similar).

## 6. Long headings that wrap across lines

### 6.1 A heading so long it must wrap gracefully in the table of contents sidebar without breaking the layout or clipping the trailing words

## 7. Conclusion

## 8. References

- [Markdown Guide](https://www.markdownguide.org)
- [CommonMark spec](https://spec.commonmark.org)
