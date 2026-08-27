# Agent Thinking Skills
A collection of Agent/Claude Skills to help you think, instead of having your thinking taken from you by GenAI.

These skills are designed to give you agency back. They ask questions, one at a time, and use your answers to decide what to ask next.

In addition, these skills are intended to flag potential weaknesses that are inherent in all GenAI, such as sycophancy and verification errors.

## The Skills
| Skill | What it's for |
| --- | --- |
| [Systems Thinking](skills/systems-thinking/) | Problems that keep coming back. Traces causes upstream, finds the feedback loops holding a situation in place, and draws Causal Loop Diagrams when the picture would help. |
| [Critical Thinking](skills/critical-thinking/) | Claims, conclusions and decisions that need testing before you act. Paul and Elder's eight Elements of Reasoning and nine Intellectual Standards, asked as questions - starting from wherever your thinking already is. |
| [Critical Thinking for GenAI](skills/critical-thinking-genai/) | Text a model produced, where walking the author back through the reasoning doesn't work because there was no route. Eleven probes that test the output instead of asking the author. |

## Roadmap
- **Cynefin** - complexity/uncertainty classification, as an additional framework within Systems Thinking.
- **Glossary** - domain vocabulary for the terms used across the skills, each linking to the APR glossary or a blog post for depth. For people reading the repo, not loaded at runtime.

## A Note on Language
These skills never have the model refer to itself as a person. It asks you to "provide an example", not to "give me an example". It doesn't say "I think" or "let me draw that".

Using personal pronouns with GenAI models leads to errors where we falsely attribute human thinking to the model. A model that speaks as "I" invites you to treat it as a colleague who has weighed the evidence and formed a view. It hasn't, and it hasn't. The moment you forget that, you stop checking its work, which is the one thing these skills exist to keep you doing.

The same rule governs the instructions inside each `SKILL.md`. They say what **the assistant** should do rather than addressing it as "you", so nothing in the text implies there is someone in there being spoken to.

## Installing a Skill
Copy-and-paste is a placeholder. Later versions will offer a proper installation method, so you won't have to move directories around by hand.

Each skill is a self-contained directory under `skills/`. For now, copy or upload the one you want:

- **Claude Code (project)** - copy the skill directory into `.claude/skills/` in your project
- **Claude Code (personal)** - copy it into `~/.claude/skills/` to use it everywhere
- **Claude apps** - zip the skill directory and upload it

Anthropic's guide: https://support.claude.com/en/articles/12512180-using-skills-in-claude

## Invoking a Skill
Two ways, and you get both by default:

- **Type the slash command** - `/critical-thinking`, `/systems-thinking`, `/critical-thinking-genai`. In Claude Code a skill directory named `x` creates `/x`, so the directory name is the command.
- **Say something that matches** - each skill lists its trigger phrases, and Claude reaches for the skill when one turns up.

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
2026-08-26 - Split Critical Thinking for GenAI out of Critical Thinking into a skill you can invoke on its own.

2026-08-24 - Added the Critical Thinking skill.

2026-08-24 - Renamed and restructured the repo from "systems-thinking" to "agent-thinking-skills" to allow for more skills.

## GenAI Usage
Claude is used to help me author the skills themselves and write the installation instructions.

## License
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) - full text in [LICENSE](LICENSE).

Copy, adapt and build on these skills, commercially or otherwise. Two conditions: keep the
attribution, and put the same licence on what you build.

That holds for derivative work assembled by a GenAI agent from these files exactly as it holds
for work assembled by hand. The obligation sits with whoever directed the agent. Keep this line:

> Mark Levison, [Agile Pain Relief](https://agilepainrelief.com) - [github.com/mlevison/agent-thinking-skills](https://github.com/mlevison/agent-thinking-skills)

[ATTRIBUTION.md](ATTRIBUTION.md) says the same thing in a form an agent can parse.

Created by [Agile Pain Relief](https://agilepainrelief.com)
