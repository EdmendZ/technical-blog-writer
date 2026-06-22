# Image Guidelines

Images are expected for most technical articles, but they must explain something important.

## Core rule

Every image must materially improve understanding.

Do not create decorative images. A technical diagram is useful only if it makes a mechanism, flow, relationship, state change, or comparison clearer than text alone.

## When to use images

Use images for:

- System or module structure
- Request or execution flow
- Data flow
- State transitions
- Lifecycle steps
- Concept relationships
- Failure modes
- Solution comparisons
- Architecture diagrams
- Source-code call paths

## When not to use images

Do not add an image when:

- It only repeats a simple sentence.
- It is decorative.
- The topic is better explained with a short table or code block.
- The image would introduce more complexity than clarity.
- The image source or license is questionable.

## Choosing generated vs external images

Prefer original generated diagrams when explaining:

- Mechanisms
- Flows
- Lifecycles
- Data structures
- Architecture
- Comparisons

Use external images when:

- The official documentation has a clearer or canonical diagram.
- The image is from a standard/specification or authoritative source.
- Recreating the image may reduce accuracy.

When using external images, prefer official or clearly licensed sources and keep the source link in the article when appropriate.

## Diagram formats

Choose the format based on the explanation need:

- Flowchart: process, decision, algorithm, lifecycle
- Sequence diagram: interactions over time, request chains
- Architecture diagram: components and relationships
- Mind map: knowledge hierarchy
- Table-like graphic: comparisons and summaries
- State diagram: state transitions

Use available diagram skills/tools when they fit the task, such as UML, Graphviz, architecture, mindmap, infographic, infocard, Vega, or other suitable diagram tools.

## Image count

Normal technical articles usually need 1-5 high-value diagrams.

More images are allowed when the topic genuinely requires them, but avoid producing many small low-value diagrams. If more than 50 images would be needed, ask the user before generating/uploading them.

## Naming

Use topic-based image names when possible.

Examples:

- `mysql-mvcc-version-chain.png`
- `redis-cache-breakdown-flow.png`
- `spring-bean-lifecycle.png`
- `jwt-session-auth-flow.png`

Prefer descriptive names over random names when the upload workflow allows it.

## Local image backup

Keep local backups by default when generating or collecting images for an article.

When possible, save both:

- The rendered image used for upload, such as `.png`, `.jpg`, `.svg`, or `.webp`
- The editable source file, such as `.mmd`, `.puml`, `.dot`, `.svg`, or HTML/CSS source

Preferred structure when the article has a local output path:

```text
article-folder/
├── article.md
└── images/
    ├── mysql-mvcc-version-chain.png
    ├── mysql-mvcc-version-chain.mmd
    ├── mysql-mvcc-read-view-flow.png
    └── mysql-mvcc-read-view-flow.mmd
```

Use the PicList uploaded URL in the final Markdown, but do not delete the local image backup unless the user explicitly asks.

If the article has no local output path, create or propose a topic-based workspace folder and save image backups there.

## Integrating images into Markdown

Each image should have:

- A meaningful alt text
- A caption or nearby explanation
- A paragraph explaining what to look at in the image
- A stable uploaded URL after PicList upload

Example:

```markdown
![MVCC 版本链示意图](https://example.com/mysql-mvcc-version-chain.png)

上图展示了一行数据在多次更新后的版本链。每个版本都通过 `roll_pointer` 指向 undo log 中的旧版本，Read View 会根据事务 ID 判断当前事务能看到哪个版本。
```

## Quality check for images

Before final delivery, ask:

- Does this image explain a hard part of the article?
- Is the image referenced by the surrounding text?
- Is the image accurate enough for the topic?
- Would removing this image make the article harder to understand?

If the answer is no, remove or replace the image.
