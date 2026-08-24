# Agent Thinking Skills
A collection of Agent/Claude Skills to help you think, instead of having your thinking taken from you by GenAI.

These skills are designed to give you agency back. They ask questions, one at a time, and use your answers to decide what to ask next.

In addition, these skills are intended to flag potential weaknesses that are inherent in all GenAI, such as sycophancy and verification errors.

## The Skills
| Skill | What it's for |
| --- | --- |
| [Systems Thinking](skills/systems-thinking/) | Problems that keep coming back. Traces causes upstream, finds the feedback loops holding a situation in place, and draws Causal Loop Diagrams when the picture would help. |

## Roadmap
- **Critical Thinking** - a new skill, examining claims, evidence and reasoning before acting on them.
- **Cynefin** - complexity/uncertainty classification, as an additional framework within Systems Thinking.

## Installing a Skill
Each skill is a self-contained directory under `skills/`. Copy or upload the one you want:

- **Claude Code (project)** - copy the skill directory into `.claude/skills/` in your project
- **Claude Code (personal)** - copy it into `~/.claude/skills/` to use it everywhere
- **Claude apps** - zip the skill directory and upload it

Anthropic's guide: https://support.claude.com/en/articles/12512180-using-skills-in-claude

Keep the directory intact when you copy it. Each `SKILL.md` loads files from its own
`references/` folder, and the skill won't work without them.

## Repository Layout
```
skills/
  <skill-name>/
    SKILL.md      # frontmatter + workflow; what Claude loads
    README.md     # the human-facing explanation
    references/   # frameworks and detail, loaded on demand
```

`SKILL.md` stays short on purpose. Anything long lives in `references/` so it's only read
when it's actually needed.

## Updates
2026-08-24 - Renamed and restructured the repo from "systems-thinking" to "agent-thinking-skills" to allow for more skills.

## GenAI Usage
Claude is used to help me author the skills themselves and write the installation instructions.

## License
CC BY-SA 4.0 - https://creativecommons.org/licenses/by-sa/4.0/

Created by [Agile Pain Relief](https://agilepainrelief.com)
