# Technical Blog Writer / 技术博客写作助手

## 中文说明

`technical-blog-writer` 是一个用于撰写中文技术 Markdown 文档的 Claude skill。它适合把关键词、零散笔记、问题、链接、代码或学习主题整理成结构清晰、适合学习复习和博客发布的技术文章。

这个 skill 的重点不是套模板，而是帮助文章更好地解释技术概念：先建立直觉，再讲流程和原理，用图表、示例和代码片段降低理解难度，最后给出便于复习的总结。

### 适合使用的场景

- 写一篇技术博客或学习笔记
- 整理零散技术笔记
- 解释某个技术原理或执行流程
- 对比两个技术方案或概念
- 准备面试复习文档
- 根据代码、链接或资料生成技术文章草稿
- 把一个抽象概念讲得更适合初学者理解

### 输出特点

默认情况下，skill 会倾向于：

- 输出中文 Markdown；
- 面向初学者到中级读者；
- 先建立 mental model，再展开细节；
- 使用自适应结构，而不是固定模板；
- 在合适的位置加入 Mermaid 图、表格或小段代码；
- 解释概念之间的关系，而不是只罗列定义；
- 加入常见误解、边界条件或工程经验；
- 以便于复习的总结收尾。

### 使用示例

```text
帮我写一篇 Markdown 技术博客，主题是 MySQL MVCC，读者是初学者。需要讲清 undo log、Read View、版本链和可重复读，最好有图解和总结。
```

```text
我有一堆 Redis 缓存穿透、缓存击穿、缓存雪崩的笔记，帮我整理成适合面试复习的技术文档。
```

```text
帮我写一篇 Hugging Face pipeline 和 AutoTokenizer + AutoModel 的对比文章，要通过同一个文本分类例子讲清楚区别。
```

### 不适合做什么

这个 skill 不是完整的图床上传、排版发布、自动评测或 benchmark 流水线。它只专注于提升技术文章本身的结构和解释质量。

---

## English Description

`technical-blog-writer` is a Claude skill for writing Chinese technical Markdown documents. It helps turn keywords, scattered notes, questions, links, source code, or learning topics into clear technical articles for study, review, interview preparation, or blog publishing.

The skill is not designed to force a rigid template. Its goal is to make technical explanations easier to understand: build intuition first, explain the mechanism, connect concepts with examples or diagrams, and end with a review-friendly summary.

### When to use

Use this skill when you want to:

- write a technical blog post or study note;
- organize scattered technical notes;
- explain a technical principle or execution flow;
- compare two technologies, concepts, or approaches;
- prepare an interview-oriented review document;
- generate an article draft from code, links, or reference material;
- make an abstract technical concept easier for beginners to understand.

### Output style

By default, the skill tends to:

- write in Chinese Markdown;
- target beginner-to-intermediate readers;
- build a mental model before details;
- use an adaptive article structure instead of a fixed template;
- add Mermaid diagrams, tables, or short code snippets when useful;
- explain relationships between concepts instead of only listing definitions;
- include common misunderstandings, boundaries, or engineering notes when helpful;
- end with a summary that is useful for later review.

### Example prompts

```text
Write a Chinese Markdown technical blog about MySQL MVCC for beginners. Explain undo log, Read View, version chains, and repeatable read with diagrams and a final summary.
```

```text
Organize my notes about Redis cache penetration, cache breakdown, and cache avalanche into an interview-oriented technical document.
```

```text
Write a comparison article about Hugging Face pipeline vs AutoTokenizer + AutoModel using the same text classification example.
```

### What this skill is not

This skill is not a full image-hosting, publishing, automated evaluation, or benchmarking pipeline. It focuses only on improving the structure and explanatory quality of technical writing.
