# Workflow

Use this workflow when creating a technical knowledge article or technical blog draft.

## 1. Understand the task

Identify what the user provided:

- Keywords or questions
- Existing notes
- Web pages or links
- Documents or pasted references
- Source code or a project path
- A broad topic to learn

If the goal is unclear, ask at most 1-2 multiple-choice questions. Prefer asking about article direction and depth.

Do not ask unnecessary questions. If the user says “write a Markdown article about MySQL MVCC for beginners,” the goal is clear enough.

## 2. Read user-provided material first

When the user provides material, use it before external research.

For notes, preserve the user's important points but reorganize them into a clearer article.

For web pages or links, fetch/read them before drafting.

For code, inspect the relevant files and write about the actual implementation rather than producing a generic article.

## 3. Decide whether research is needed

Research is useful when:

- The topic depends on a specific library/framework/version.
- Official behavior may have changed.
- The article needs precise definitions, standards, or protocol details.
- The user provided links or asked for reference-backed content.
- The model's background knowledge may be insufficient or stale.

Prefer official documentation, source code, specs, and high-quality engineering references.

## 4. Choose the article direction

Classify the task, but allow mixed types:

- Principle explanation
- Practical problem solving
- Comparison article
- Source/code analysis
- Interview review
- Architecture/workflow explanation

Use the classification to choose a structure pattern, not a rigid template.

## 5. Build an outline

For broad or complex topics, draft a short outline before the full article.

A good outline should:

- Put basic intuition before advanced details.
- Group related concepts together.
- Make the learning path obvious.
- Reserve image positions for places where diagrams will help.

For simple tasks, the outline can be implicit in the final Markdown sections.

## 6. Plan diagrams/images

Before creating images, decide what each image explains.

Good image purposes:

- Show a lifecycle or process.
- Show data/state transitions.
- Compare multiple mechanisms.
- Show architecture or module relationships.
- Turn an abstract concept into a concrete mental model.

Avoid images that only decorate the article.

## 7. Draft the article

Write in Chinese Markdown unless the user asks otherwise.

Default writing sequence:

1. Explain why the topic matters.
2. Build an intuitive understanding.
3. Define core concepts.
4. Explain the main mechanism or problem.
5. Use diagrams and examples to make the hard parts visible.
6. Add optional sections only when they help: common mistakes, interview questions, code examples, production notes, comparisons.
7. End with a useful summary.

## 8. Upload images when appropriate

Use PicList for normal image upload without asking every time. Ask only when the conditions in `SKILL.md` require confirmation.

After upload, replace local image paths with stable image URLs in Markdown.

## 9. Final quality pass

Before delivering, verify:

- The article covers the core knowledge points.
- The structure is clear.
- The article is suitable for the user and beginners.
- The core principle is actually explained, not merely named.
- Diagrams are useful and connected to the text.
- The article has a useful final summary.
- Markdown is publishable.
- References are included when external sources materially informed the article.
