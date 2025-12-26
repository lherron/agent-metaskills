# Agent Metaskills

Metaskills for AI agent harnesses. These skills enhance how agents interpret requests, synthesize information, and surface latent knowledge.

Follows the [Agent Skills specification](https://agentskills.io/specification).

## Skills

| Skill | Description |
|-------|-------------|
| **prompt-shaping** | Propose structured interpretations of underspecified requests. Rapidly prototypes intent by restating, structuring, and committing to a next action. |
| **cued-retrieval** | Surface tacit knowledge through Socratic questioning. Draws out understanding through targeted questions rather than proposing solutions. |

## Installation

### Claude Code

Register this repository as a plugin marketplace:
```
/plugin marketplace add lherron/agent-metaskills
```

Install the skills:
```
/plugin install metaskills@lherron-agent-metaskills
```

### Codex CLI

See [Codex Skills documentation](https://developers.openai.com/codex/skills/) for installation instructions.

## Creating New Skills

Each skill is a folder containing a `SKILL.md` file:

```markdown
---
name: skill-name
description: When the agent should use this skill
---

# Skill Name

Instructions the agent follows when this skill is active.
```

Use `./template/SKILL.md` as a starting point.

## License

MIT
