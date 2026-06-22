# Research Guidelines

Use research to improve correctness, not to make the article look artificially sourced.

## When to research

Research is recommended or required when:

- The topic depends on specific versions of a framework, language, database, or tool.
- The article discusses APIs, configuration, commands, or behavior that may change.
- The topic involves standards, protocols, RFCs, specifications, or official definitions.
- The user provides web pages, documentation, or source links.
- The user asks for references.
- The article makes claims about performance, limits, defaults, or compatibility.
- The topic is unfamiliar or could be affected by recent changes.

## When model knowledge may be enough

For stable foundational concepts, model knowledge may be enough for a first draft, but still verify if the user needs high accuracy or references.

Examples:

- Basic concept explanation
- General mental models
- Stable computer science principles

## Source priority

Prefer sources in this order:

1. User-provided notes, links, documents, or code
2. Official documentation
3. Source code, standards, RFCs, or specifications
4. Vendor engineering blogs or reputable project maintainers
5. High-quality technical blogs with clear reasoning
6. General web content

Avoid relying on reposted, low-quality, or unsourced content when official sources are available.

## How to use sources

- Use sources to verify facts, not to copy structure blindly.
- Preserve the user's learning goal and article style.
- If sources disagree, mention the version/context or choose the official source.
- Keep important reference links in the final article when they materially informed the content.

## Citation style

For blog drafts, a simple reference section is enough unless the user asks for formal citations.

Example:

```markdown
## 参考资料

- MySQL 官方文档：InnoDB Multi-Versioning
- Redis 官方文档：Distributed Locks with Redis
- Spring Framework Reference Documentation：Core Technologies
```

## Avoid unsupported claims

Be careful with:

- Performance numbers
- “always/never” statements
- Security recommendations
- Version-specific behavior
- Production best practices
- Comparisons between tools

When uncertain, qualify the statement or verify it.
