# Markdown Quality Check

This document describes a lightweight manual check for generated Markdown articles. It can later be replaced by a deterministic script if repeated issues appear.

## Check items

Before delivering a Markdown article, verify:

1. The article has exactly one main `#` title unless the user's publishing platform requires otherwise.
2. Heading levels do not jump in confusing ways.
3. Image links are not broken placeholders.
4. Code blocks use language labels when the language is known.
5. Tables render cleanly in Markdown.
6. There are no leftover TODO markers.
7. The final summary exists and is useful.
8. References are present when external sources materially informed the article.

## Optional future automation

If this skill repeatedly produces long articles, consider adding a script that checks:

- Missing title
- Broken local image paths after upload
- TODO placeholders
- Heading hierarchy
- Empty sections
- Missing final summary
