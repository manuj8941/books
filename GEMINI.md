# Book Publishing & Typography Guidelines

## 1. Typography & CSS Invariants
- **Text Alignment**: Always use `text-align: left;` for HTML and EPUB styles (never justify, avoiding loose word rivers).
- **Leading (Line-Height)**:
  - English book text: `line-height: 1.42 - 1.45;` (compact, dense literary texture matching physical paperbacks).
  - Hindi book text: `line-height: 1.50 - 1.55;` (provides breathing room for top and bottom matras while maintaining book density).
- **Paragraph Spacing**: Authentic printed book style with `margin-bottom: 0;` and `text-indent: 1.8em;` (zero vertical void between paragraphs; transitions demarcated purely by indents).
  - The first paragraph of any chapter or after a subhead has `text-indent: 0;`.
- **Palette**: Warm newsprint `#FBFAF8` paper with `#121212` obsidian ink.

## 2. PDF Text Extraction
- Always verify bottom line coordinates (use `ly0 > 865` or dynamic page height minus footer margin) to avoid dropping bottom lines across pages.
- Inspect page breaks across chapters to ensure split sentences are stitched cleanly.
- Standalone literary excerpts/quotations must be isolated into distinct `<blockquote>` blocks.

## 3. Translation Register
- Hindi translations must use Option A (धारदार साहित्यिक हिंदुस्तानी): natural, evocative, journalistic Hindi with fluid Hindustani/Urdu idioms, preserving the author's original voice.
