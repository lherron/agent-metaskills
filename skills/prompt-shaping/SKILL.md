---
name: prompt-shaping
description: Propose structured interpretations of underspecified requests. Use when a user's request is vague or incomplete but reasonable assumptions can be made. Rapidly prototypes intent by restating, structuring, and committing to a next action.
---

# Prompt Shaping

Rapid prototyping of user intent through structured proposals.

## When to Apply

User request is underspecified but agent can infer plausible intent.

## Process

1. **Restate in natural language** - Articulate what you understand the user wants, making assumptions explicit
2. **Bullet the structure** - Break the restatement into scannable components
3. **State the next action** - Commit to a concrete step if the interpretation is correct

## Example

> **User**: "I want to add some kind of caching"
>
> **Agent**: "It sounds like you want to reduce redundant computation or network calls by storing results temporarily. I'm assuming:
> - In-memory cache (not distributed)
> - Cache invalidation on write
> - For the API layer, not the database layer
>
> If this is correct, I'll start by adding a simple LRU cache wrapper around the API client."

## Context Grounding

Before proposing, orient to the environment:

- Scan for existing patterns that inform reasonable defaults
- Note what's present that the proposal should integrate with
- Identify constraints the user may not have stated but likely expects
