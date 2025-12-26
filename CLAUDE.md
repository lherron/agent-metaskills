# Agent Metaskills

Meta-skills for agent harnesses following the [Agent Skills standard](https://agentskills.io).

## Structure

- `.claude-plugin/marketplace.json` - Plugin marketplace configuration
- `skills/` - Individual skill implementations (each with a `SKILL.md`)
- `template/` - Template for creating new skills

Specification: https://agentskills.io/specification

## Creating Skills

Each skill is a folder containing:
- `SKILL.md` - Required. YAML frontmatter (`name`, `description`) + markdown instructions

```markdown
---
name: skill-name
description: When Claude should use this skill
---

# Instructions here
```

## Marketplace

- **Name**: `lherron-agent-metaskills`
- **Owner**: Lance Herron <skills@notlevel.com>
- **Install**: `/plugin marketplace add lherron/agent-metaskills`

## License

MIT
