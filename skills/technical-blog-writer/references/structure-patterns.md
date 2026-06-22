# Structure Patterns

These are structure patterns, not mandatory templates. Choose and adapt based on the current task.

## Principle explanation

Use for mechanisms such as MVCC, JVM GC, TCP handshake, AQS, Raft, Redis persistence, Spring IoC, or similar topics.

Possible structure:

```markdown
# Title

## Why this mechanism matters
## First intuition
## Core concepts
## The main mechanism
## Diagram walkthrough
## Key details and edge cases
## Common misunderstandings, if useful
## Summary
```

Good diagrams:

- State transition diagram
- Execution flow
- Data structure relationship
- Lifecycle diagram

## Practical problem solving

Use for practical engineering problems such as cache penetration/breakdown/avalanche, distributed locks, idempotency, rate limiting, circuit breaking, logging, monitoring, or deployment problems.

Possible structure:

```markdown
# Title

## Problem background
## What the problem looks like
## Why it happens
## Solution options
## Diagram of the flow or failure mode
## Comparison of solutions
## Production notes
## Summary
```

Good diagrams:

- Failure flow
- Request path
- Solution architecture
- Before/after comparison

## Comparison article

Use when comparing mechanisms, technologies, or solutions, such as JWT vs Session, Kafka vs RabbitMQ, MySQL vs PostgreSQL, Redis persistence options, or different locking strategies.

Possible structure:

```markdown
# Title

## What problem are we comparing for?
## Quick conclusion
## Concept overview
## Comparison dimensions
## Scenario-based recommendations
## Diagram or table summary
## Common mistakes when choosing
## Summary
```

Good diagrams:

- Decision tree
- Comparison matrix
- Request/interaction flow comparison

## Source/code analysis

Use when the user provides code, a project path, or asks to explain an implementation.

Possible structure:

```markdown
# Title

## What this code/module does
## Entry point and request flow
## Key classes/functions/files
## Diagram of the execution path
## Important implementation details
## Risks or improvement points
## Summary
```

Rules:

- Read relevant code before writing.
- Reference actual files/functions when possible.
- Do not replace code analysis with a generic explanation.

Good diagrams:

- Sequence diagram
- Call graph
- Component relationship diagram
- State/lifecycle diagram

## Interview-oriented summary

Use when the user explicitly asks for interview preparation, high-frequency questions, or review notes.

Possible structure:

```markdown
# Title

## Core conclusion
## Must-know concepts
## Principle explanation
## Common interview questions
## Easy-to-miss details
## Summary table
```

Rules:

- Do not make the whole article a Q&A if the user also wants principle clarity.
- Explain why each answer is true, not just the answer itself.

Good diagrams:

- Mental model diagram
- Comparison table
- Process diagram for common questions

## Architecture or workflow explanation

Use for system design, request chains, authentication flows, data pipelines, or module interactions.

Possible structure:

```markdown
# Title

## System/problem context
## Main components
## End-to-end flow
## Diagram walkthrough
## Key design decisions
## Tradeoffs and limitations
## Summary
```

Good diagrams:

- Architecture diagram
- Sequence diagram
- Data flow diagram
- Layered component diagram

## Mixed articles

Many user requests are mixed. For example: “讲清楚 Redis 缓存问题，适合面试，也要能落地.”

For mixed articles:

- Start with the dominant need.
- Add secondary sections only where useful.
- Keep principle clarity first when the user is learning.
- Avoid bloating the article with every possible section.
