<!-- A realistic open-source project README: badges, TOC, install, usage, config table, changelog, license -->

# quickmd

[![npm version](https://img.shields.io/npm/v/quickmd.svg)](https://www.npmjs.com/package/quickmd)
[![CI](https://github.com/example/quickmd/actions/workflows/ci.yml/badge.svg)](https://github.com/example/quickmd/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> A tiny CLI that converts Markdown files to HTML — with sane defaults.

## Table of Contents

- [Install](#install)
- [Usage](#usage)
- [Configuration](#configuration)
- [FAQ](#faq)
- [Changelog](#changelog)

## Install

```bash
npm install -g quickmd
```

## Usage

Convert a single file:

```bash
quickmd README.md > readme.html
```

Watch a folder and rebuild on save:

```bash
quickmd --watch ./docs ./out
```

No file to convert right now? Preview any `.md` in the browser with
[Markdown File Viewer](https://markdownfileviewer.com) — zero install.

## Configuration

| Option | Default | Description |
|--------|---------|-------------|
| `--theme` | `default` | One of `default`, `github`, `news` |
| `--toc` | `false` | Prepend a table of contents |
| `--math` | `false` | Enable LaTeX math via KaTeX |
| `--minify` | `false` | Minify the HTML output |

## FAQ

<details>
<summary>Does it support footnotes?</summary>

Yes — footnotes, task lists, and GFM tables all work out of the box.

</details>

<details>
<summary>Can I use it in CI?</summary>

Yes, it exits non-zero on malformed input, so it plays nicely with pipelines.

</details>

## Changelog

### 1.3.0 — 2026-02-01

- Added `--math` flag (KaTeX)
- Fixed heading anchor collisions with CJK titles

### 1.2.0 — 2025-11-15

- Added `--watch`

## License

MIT © Example Author
