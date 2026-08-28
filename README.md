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

## What To Ask
**Systems Thinking - causes upstream, consequences downstream**
State the problem, or the plan
- We solved this problem last quarter and it keeps coming back
- Everyone sees a different cause for the same problem
- We're considering bonuses for resolving client calls within five minutes
- In three years we expect GenAI to do most of the work

For more detail see: [Systems Thinking](https://agilepainrelief.com/glossary/systems-thinking/)

**Critical Thinking - testing human reasoning and its implications**
State the claim, or the decision
- Adding another step in the review process will reduce the number of defects
- I've decided to take a new job
- My co-worker is getting under my skin and raising the problem will just make it worse
- We selected a new supplier in ten minutes with no objections

**Critical Thinking for GenAI - testing output that has no human reasoning**
Share what the model generated
- It quoted a statistic without a source
- It summarised a sensitive meeting and agreed with claims people made in it
- I asked two different LLMs and they agreed
- It reviewed the contract and said "no flags"

## Roadmap
- **Cynefin** - complexity/uncertainty classification, as an additional framework within Systems Thinking.
- **Glossary** - domain vocabulary for the terms used across the skills, each linking to the APR glossary or a blog post for depth. For people reading the repo, not loaded at runtime.

## A Note on Language
These skills never have the model refer to itself as a person. It asks you to "provide an example", not to "give me an example". It doesn't say "I think" or "let me draw that".

Using personal pronouns with GenAI models leads to errors where we falsely attribute human thinking to the model. A model that speaks as "I" invites you to treat it as a colleague who has weighed the evidence and formed a view. It hasn't, and it hasn't. The moment you forget that, you stop checking its work, which is the one thing these skills exist to keep you doing.

The same rule governs the instructions inside each `SKILL.md`. They say what **the assistant** should do rather than addressing it as "you", so nothing in the text implies there is someone in there being spoken to.

## Installing a Skill
Three routes. The first two update themselves; the third doesn't.

### npx skills
Works with Claude Code, Codex, Cursor, OpenCode and around thirty other agents. The registry is
[skills.sh](https://skills.sh); this repository is the package.

```bash
npx skills add mlevison/agent-thinking-skills                       # asks where to put them, offers all three
npx skills add mlevison/agent-thinking-skills -g                    # personal, so every project has them
npx skills add mlevison/agent-thinking-skills -s critical-thinking  # one skill only
npx skills update                                                   # pull later versions
```

The CLI reports anonymous install counts by default; `DO_NOT_TRACK=1` turns that off.

### Claude Code plugin
Installs all three at once and keeps them current through `/plugin update`.

```
/plugin marketplace add mlevison/agent-thinking-skills
/plugin install thinking-skills@agile-pain-relief
```

The first line registers the catalogue and installs nothing. The second does the installing.
`agile-pain-relief` is the marketplace name rather than the repository name, so the two
deliberately differ.

To remove: `/plugin uninstall thinking-skills@agile-pain-relief`.

### By hand
Each skill is a self-contained directory under `skills/`. Copy the whole thing, `references/` and
all, or the skill won't load:

- **Claude Code (project)** - into `.claude/skills/`, committed
- **Claude Code (personal)** - into `~/.claude/skills/`, for every project
- **Claude apps** - zip the directory and upload it

Symlinking a clone instead of copying makes `git pull` the update:
`ln -s "$PWD/skills/critical-thinking" ~/.claude/skills/critical-thinking`.

Anthropic's guide: https://support.claude.com/en/articles/12512180-using-skills-in-claude

## Invoking a Skill
Two ways, and you get both by default:

- **Type the slash command** - `/critical-thinking`, `/systems-thinking`, `/critical-thinking-genai`. In Claude Code a skill directory named `x` creates `/x`, so the directory name is the command.
- **Say something that matches** - each skill lists its trigger phrases, and Claude reaches for the skill when one turns up.

Installed as a plugin, each skill also answers to a namespaced command,
`/thinking-skills:critical-thinking`, which is what to type if something else on the machine has
already claimed the short name.

## Repository Layout
```
.claude-plugin/
  marketplace.json  # the catalogue /plugin marketplace add reads
  plugin.json       # this repo as a single plugin
skills/
  <skill-name>/
    SKILL.md        # frontmatter + workflow; what Claude loads
    README.md       # the human-facing explanation
    references/     # frameworks and detail, loaded on demand
```

`SKILL.md` stays short on purpose. Anything long lives in `references/` so it's only read
when it's actually needed.

## Updates
- 2026-08-26 - Split Critical Thinking for GenAI out of Critical Thinking into a skill you can invoke on its own.
- 2026-08-24 - Added the Critical Thinking skill. Renamed and restructured the repo from "systems-thinking" to "agent-thinking-skills" to allow for more skills.

## GenAI Usage
Claude is used to help me design the skills themselves and write the installation instructions. The core content remains human authored. *To the extent that Mark Levison remains human.*

## Contributing
Issues first, please, for ideas every bit as much as for bugs. It's the cheapest place to find out whether something fits, and it saves you writing a patch that was never going to land.

The wording here is fussed over to a degree that is probably unreasonable, down to the pronouns. Changing a skill's text changes how the skill behaves, so it's worth a conversation before anyone spends an evening on it.

Pull requests written by an agent won't be merged. A model helped draft plenty of what's here, so that's a fair thing to raise: the difference is that every line was argued with, cut and rewritten by someone who has to live with the result. 

*The irony that this is the longest stretch of generated text in the repository has been noted.*

## License
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) - full text in [LICENSE](LICENSE).

Copy, adapt and build on these skills, commercially or otherwise. Two conditions: keep the
attribution, and put the same licence on what you build.

That holds for derivative work assembled by a GenAI agent from these files exactly as it holds
for work assembled by hand. The obligation sits with whoever directed the agent. Keep this line:

> Mark Levison, [Agile Pain Relief](https://agilepainrelief.com) - [github.com/mlevison/agent-thinking-skills](https://github.com/mlevison/agent-thinking-skills)

[ATTRIBUTION.md](ATTRIBUTION.md) says the same thing in a form an agent can parse.

Created by [Agile Pain Relief](https://agilepainrelief.com)
