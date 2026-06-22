# PicList Upload

The user uses PicList as the blog image hosting workflow. Normal article images may be uploaded automatically without asking every time, unless the conditions in `SKILL.md` require confirmation.

## Current status

The exact local PicList/PicGo command may vary by environment. Do not hard-code a command until it has been verified in the user's environment.

When first performing an actual upload task:

1. Check which PicList/PicGo command is available.
2. If the command and config are clear, upload the generated images.
3. If unclear, ask only for the missing operational detail.
4. After the workflow is verified, update this reference with the exact command.

## Upload behavior

For normal technical articles:

- Generate or collect the images.
- Name images by topic when possible.
- Upload through PicList.
- Replace local image paths in Markdown with uploaded URLs.
- Report upload failures honestly.

## When to ask before uploading

Ask the user before uploading only when:

- The article needs more than 50 images.
- The PicList command/configuration is unknown or broken.
- The image source/license is questionable.
- The upload destination seems different from the expected blog image host.
- Uploading would publish content that is not part of the user's requested article.
- Image size/count is unusually high.

## Local backup behavior

Keep local backups by default.

For each generated or collected article image:

- Save the rendered image locally before or after upload.
- Save the editable diagram source when available, such as `.mmd`, `.puml`, `.dot`, `.svg`, or HTML/CSS source.
- Use the PicList uploaded URL in the final Markdown.
- Do not delete local image files unless the user explicitly asks.

Preferred structure when the article has a local output path:

```text
article-folder/
├── article.md
└── images/
    ├── topic-diagram.png
    └── topic-diagram.mmd
```

If the article has no local output path, create or propose a topic-based workspace folder for image backups.

## Expected output after upload

After upload, Markdown should contain stable image URLs:

```markdown
![图解说明](https://uploaded-image-url.example/topic-image.png)
```

Avoid leaving local paths such as:

```markdown
![图解说明](./images/topic-image.png)
```

unless the user explicitly asks for a local draft.

## Naming guidance

Use descriptive topic-based names when the tool allows it:

- `mysql-mvcc-read-view.png`
- `redis-cache-penetration-flow.png`
- `spring-bean-lifecycle.png`
- `jwt-session-comparison.png`
