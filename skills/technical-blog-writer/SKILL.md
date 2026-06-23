---
name: technical-blog-writer
description: Use this skill whenever the user wants to write, organize, rewrite, expand, or polish a Chinese technical Markdown article, study note, principle explanation, comparison document, interview review, or source-material-to-blog draft. Use it especially when the article should explain mechanisms clearly, build intuition for beginners, use helpful diagrams/tables/code snippets, and become publishable or reviewable Markdown. This skill should make the article more structured, more explanatory, and more useful for later review than a generic answer.
---

# Technical Blog Writer

Use this skill to write Chinese technical Markdown articles that are useful for learning, review, blog publishing, or interview preparation.

The goal is not to fill a fixed template. The goal is to help the reader understand a technical topic clearly: build intuition first, explain the mechanism, connect concepts with examples or diagrams, and end with a summary that is useful for later review.

## Defaults

Unless the user says otherwise:

- Write in Chinese Markdown.
- Write for the user and beginner-to-intermediate readers.
- Prefer “先建立直觉，再讲流程/原理，最后总结复习点”.
- Use an adaptive structure instead of forcing every article into the same template.
- Use Mermaid diagrams, Markdown tables, and small code snippets when they make the explanation clearer.
- Do not add decorative diagrams.
- Do not upload images or use image hosting unless the user explicitly asks.
- Do not ask clarification questions when the request is already clear enough.

## Writing workflow

1. Identify the article type:
   - principle explanation
   - process walkthrough
   - comparison
   - practical troubleshooting
   - source/code analysis
   - interview review

2. Pick one concrete thread to carry the article, such as:
   - one API call
   - one request flow
   - one input example
   - one lifecycle
   - one data transformation path

3. Build the article around the reader's learning path:
   - why this topic matters
   - the mental model
   - core concepts
   - the main flow or mechanism
   - examples, diagrams, tables, or code where helpful
   - common misunderstandings or engineering notes when useful
   - final review summary

4. Write directly unless the topic is broad; for broad topics, give a short outline before the full article.

5. Before final delivery, quickly check:
   - Is the main mechanism actually explained?
   - Are concepts connected instead of listed separately?
   - Is the structure suitable for this topic?
   - Does each diagram/table/code block reduce confusion?
   - Does the final summary help later review?

## Style rules

- Use clear, natural Chinese technical blog style.
- Be beginner-friendly but not shallow.
- Explain “why” and “how,” not just “what”.
- Use examples to make abstract mechanisms concrete.
- Use tables for comparisons, tradeoffs, and checklists.
- Use Mermaid for flows, lifecycles, component relationships, and process diagrams.
- Avoid turning every article into interview Q&A unless the user asks for that format.
- Avoid unsupported version-specific claims; verify or qualify them when needed.

## Clarification rules

Ask at most 1-2 concise questions only when the article goal is genuinely unclear.

Useful clarification choices:

1. Direction:
   - principle explanation
   - practical application / troubleshooting
   - comparison
   - interview review
   - mixed

2. Depth:
   - beginner-friendly
   - moderately deep
   - interview-deep
   - source/implementation-level

If the user does not choose, default to beginner-friendly but not superficial.

## Input handling

The user may provide keywords, notes, links, documents, source code, or a vague learning topic.

Use sources in this order:

1. User-provided material
2. Official documentation, specifications, standards, or source code
3. High-quality engineering articles
4. General web content
5. Model background knowledge

When using external sources, include important reference links in the final article if they materially informed the content.

## Output expectations

Deliver a complete Markdown document or write it to the requested file path.

A good final article should usually include:

- a clear title and heading hierarchy
- an opening that explains why the topic matters
- a mental model before detailed terms
- one concrete flow/example that connects the sections
- useful diagrams/tables/code snippets where appropriate
- common misunderstandings, boundaries, or troubleshooting notes when useful
- a final summary for review

Avoid placeholders such as “TODO: add image” or broken local image paths unless the user explicitly asked for a rough draft.
