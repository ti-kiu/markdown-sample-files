<!-- Expected: fenced blocks with language + metadata strings, indented 4-space block, unnamed fence, empty fence, nested fences, inline code with backtick runs -->

# Code Blocks

## JavaScript with metadata

```js title="viewer.js"
import { render } from "./render.js";

const html = await render("# Hello");
document.querySelector("#out").innerHTML = html;
```

## Python

```python
def head(text: str, n: int = 3) -> str:
    lines = text.splitlines()
    return "\n".join(lines[:n])
```

## Shell (no trailing newline inside)

```bash
curl -s https://markdownfileviewer.com/test-doc.md | head -5
```

## Other languages, one line each

```json
{"ok": true, "submission_id": "srv_abc"}
```

```yaml
categories: [files, general-tools]
```

```sql
SELECT name, url FROM tools WHERE category = 'files';
```

```rust
fn main() { println!("render!"); }
```

```go
package main

import "fmt"

func main() { fmt.Println("hi") }
```

```css
.markdown-body table { border-collapse: collapse; }
```

```c
#include <stdio.h>
int main(void) { puts("hi"); return 0; }
```

```
plain fence, no language — must render as monospace block, no highlighting
```

## Indented (legacy) style

    This block is indented by four spaces.
    It stays verbatim.

## Empty fence

```
```

## Inline with multiple backticks

`` `code with a literal backtick inside` `` and `single` are both fine.
