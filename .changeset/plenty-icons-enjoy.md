---
'@emotion/serialize': major
---

What: Fix error allowing invalid fontWeight values

Why: The `fontweight` property of CSSObject allows invalid values (e.g. 'wrong'). It's expected behavior is to show an error.

How: Add `validFontWeight` type to `StrictCSSProperties`, declaring which values are only allowed.
