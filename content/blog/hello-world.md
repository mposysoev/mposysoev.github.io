+++
title = "First post"
date = 2026-04-15
description = "A short first note on the site setup, math, and images."

[taxonomies]
tags = ["meta"]

[extra]
math = true
+++

This is the first post on the new site. The setup is intentionally minimal: plain Markdown in, static HTML out, no JavaScript framework.

## Math

Inline math works like $E = mc^2$, and display math like:

$$
\int_{-\infty}^{\infty} e^{-x^2}\, dx = \sqrt{\pi}
$$

To enable math on a post, add `math = true` under `[extra]` in the front matter.

## Code

```python
def hello(name: str) -> str:
    return f"Hello, {name}"
```

## Images

Drop images into the same folder as the post and reference them with a relative path:

```markdown
![Caption](image.png)
```

This post also serves as a compact reference for the blog's Markdown features.
