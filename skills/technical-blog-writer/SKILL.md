---
name: technical-blog-writer
description: Use this skill whenever the user wants to create, organize, rewrite, expand, or polish a technical knowledge document, technical blog post, beginner-friendly study note, interview-oriented summary, principle explanation, or source-material-to-article draft from keywords, questions, notes, web pages, references, or code. Use it especially when the user wants Markdown output, clear explanations of technical principles, adaptive structure instead of a rigid template, diagrams/images that improve understanding, research-backed content, or image hosting through PicList/blog image hosting.
---

# Technical Blog Writer

Use this skill to create Chinese-language technical Markdown documents for blog publishing, self-study, deeper understanding, and interview preparation.

The goal is not to fill a fixed template. The goal is to help the user understand a technical topic clearly, with an adaptive article structure, accurate research, useful diagrams, and a publishable Markdown result.

## Default assumptions

Unless the user says otherwise:

- Output a Chinese Markdown article suitable for a technical blog.
- The audience is the user and beginner learners.
- Prioritize explaining principles clearly; build intuition first, then deepen the details.
- Core concepts, useful diagrams, and a final summary are required.
- Common mistakes, interview questions, code examples, production notes, and references are optional; include them only when they genuinely fit the task.
- Use an adaptive structure. Do not force every article into the same section template.
- Web research is allowed when it improves correctness, fills gaps, verifies version-specific behavior, or the user provides web/source materials.
- Images are usually expected, but every image must materially improve understanding.
- PicList upload is authorized for normal article generation; see the PicList rules below.
- Keep local image backups by default when generating or collecting article images.

## Core workflow

1. Clarify the current document goal only if needed.
2. Read user-provided materials first: keywords, questions, notes, web pages, references, or code.
3. Search external sources when needed for correctness, official definitions, versions, or missing context.
4. Choose a suitable article direction and structure pattern.
5. Draft a clear outline before writing the full article when the task is broad.
6. Decide which diagrams/images are needed and what each one must explain.
7. Generate original diagrams or source authoritative images as appropriate.
8. Upload images through PicList when appropriate, following the upload rules.
9. Assemble the final Markdown document.
10. Run the quality checklist before final delivery.

For the detailed workflow, read `references/workflow.md`.

## Clarification rules

If the request is unclear, ask at most 1-2 concise multiple-choice questions. Prefer option-style questions over open-ended questions.

Do not ask questions when the user has already provided enough context; proceed with reasonable defaults.

Good default clarification questions:

1. Article direction:
   - A. Principle explanation: explain the underlying mechanism and why it works this way
   - B. Practical application: focus on how to use it, how to implement it, and production notes
   - C. Interview review: focus on high-frequency questions, traps, and concise summaries
   - D. Mixed: cover principle + application + interview points, with principle clarity first

2. Depth:
   - A. Beginner-friendly: build intuition first, then explain the core mechanism
   - B. Moderately deep: suitable for someone with some background who wants deeper understanding
   - C. Interview-deep: emphasize principles, boundaries, comparisons, and common mistakes
   - D. Source/implementation-level: explain using code, source code, or implementation details

If the user does not choose, default to a beginner-friendly or moderately deep article depending on the topic, with principle clarity as the priority.

## Input handling

The user may provide:

- A group of keywords or questions
- Existing notes
- Web pages or reference links
- Documents or copied material
- Source code or a project path
- A vague topic they want to learn

Prioritize sources in this order:

1. User-provided material
2. Official documentation, specifications, standards, or source code
3. High-quality engineering articles or reputable technical blogs
4. General web content
5. Model background knowledge

When using external sources, preserve important reference links in the final article if they materially informed the content.

For research rules, read `references/research-guidelines.md`.

## Article structure

Adapt the structure to the task. Do not force a rigid template.

Use structure patterns from `references/structure-patterns.md` when helpful, especially for:

- Principle explanation
- Practical problem solving
- Comparison articles
- Source/code analysis
- Interview-oriented summaries
- Architecture or workflow explanations

Every article should still have:

- A clear title
- A clear outline or logically obvious section hierarchy
- Core concepts
- A clear explanation of the main principle/mechanism/problem
- Diagrams/images when they improve understanding
- A final summary useful for review

## Writing style

Use the default writing style from `references/writing-style.md` unless the user provides style examples or feedback.

Important style defaults:

- Write in clear Chinese technical blog style.
- Explain for the user and beginners, not for experts only.
- Prefer “first intuition, then details.”
- Avoid merely listing terms or interview answers.
- Use examples, analogies, diagrams, and step-by-step reasoning for abstract mechanisms.
- Keep the tone natural, systematic, and useful for later review.

If the user gives feedback about style, generalize it into future behavior rather than overfitting to one article.

## Image and diagram rules

Images must explain something. Do not create decorative images.

Use images for:

- System structure
- Execution flow
- Data flow
- State changes
- Concept relationships
- Lifecycle steps
- Architecture
- Comparisons

Prefer original diagrams for mechanisms, flows, structures, and comparisons. Use external images when they are official, authoritative, or clearly more accurate than a generated diagram.

Every image should have:

- A clear purpose
- A relevant surrounding explanation
- A caption or nearby explanation
- A stable Markdown link after upload

Most normal articles should use 1-5 high-value diagrams. More are allowed when the topic needs them, but do not create many low-value images just because upload is available.

For detailed image rules, read `references/image-guidelines.md`.

## Local image backup rules

When generating or collecting images for an article, keep local backups by default.

- Save the rendered image locally.
- Save the editable diagram source when available, such as `.mmd`, `.puml`, `.dot`, `.svg`, or HTML/CSS source.
- Use PicList uploaded URLs in the final Markdown.
- Do not delete local image files unless the user explicitly asks.
- Prefer an `images/` folder next to the article when the article has a local output path.
- If the article has no local output path, create or propose a topic-based workspace folder and keep image backups there.

## PicList upload rules

The user authorizes automatic PicList upload for normal article generation. Do not ask for confirmation before uploading images unless one of these applies:

- The article needs more than 50 images.
- PicList configuration, command, or upload target is unclear.
- The image source/license is questionable.
- Upload results are abnormal.
- The number or size of images is unusually high.
- Uploading would publish content that differs from the user's described intent.

Use topic-based image names when possible.

Because the exact PicList command may vary by environment, detect the available PicList/PicGo workflow before first use. If the upload command is not yet known, follow `references/piclist-upload.md` and ask only for the missing operational detail.

## Final output expectations

When delivering the article, provide a complete Markdown document or write it to the user-requested file path.

The final article should be directly useful for blog publishing or later editing. Avoid placeholders such as “TODO: add image” or broken local image paths unless explicitly delivering a draft.

If external sources were used, include a short references section when appropriate.

Before final delivery, run the checklist in `references/quality-checklist.md`.
