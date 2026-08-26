# Critical Thinking
Part of [Agent Thinking Skills](../../README.md).

You've done the hard work, research and thinking. The obvious conclusion is in front of you.
This skill asks the questions a good critical thinker would ask, in the order that is most likely to help.

## The Problem This Solves
Reasoning fails without a red flag. It fails with an unstated assumption, a missing piece of evidence, or a word two people define differently.

You can't spot these from inside your own position. The assumption you can't see might be the most important one.

Richard Paul and Linda Elder broke reasoning into eight elements you can examine one at a time, and nine standards you can hold any answer to. This skill turns both into questions.

## How Much of This Is Worth Doing
Reversibility sets the effort. Where a decision can be undone cheaply, being wrong costs less, so the decision doesn't need the full pass.

What it needs is the cheapest way to reduce the uncertainty. Sometimes that's reading what has already been written, or asking someone who has done it. Sometimes it's a small experiment. Critical thinking earns its keep either way, mostly to design the check: what would count as this going wrong, what to measure, and when to look. The rest of the elements are for the decisions that are expensive or slow to undo.

How well the problem is understood matters as much as reversibility. Where a situation is complex in the [Cynefin](https://agilepainrelief.com/glossary/complexity/) sense, there is little to predict from, and an experiment says more than another round of analysis.

## It Starts by Asking Where You Are
The eight elements are not a sequence, so there is no fixed place to begin. Where you already are decides which one opens the conversation.

The first question is about you, not your argument: **where are you with this right now?**

- Still working out what you're deciding
- Gathering evidence
- Trying to make sense of what you've got
- Testing a conclusion you've already reached
- Judging something somebody else told you
- About to commit, and want a last look

The answer picks the starting point. From there the questioning follows wherever the reasoning is thinnest, usually assumptions or point of view, because those are the two things invisible from where you're standing.

## What You Get
Eight elements, offered one question at a time:

- **Purpose** - what the work is meant to accomplish, and whose goal it is
- **Question at Issue** - the question being settled, and whether it's secretly three questions
- **Information** - what the evidence is, where it came from, and what would count against it
- **Inferences** - where the evidence stops and interpretation starts
- **Concepts** - the key terms, and whether two people would define them the same way
- **Assumptions** - what's being taken for granted, and which ones collapse everything if they're wrong
- **Point of View** - what the frame shows, and what it hides
- **Implications** - what follows if the conclusion holds, what it costs if it doesn't, and who pays

And nine standards used to test the answers rather than to start conversations: **clarity, accuracy, precision, relevance, depth, breadth, logic, significance, fairness.** When an answer is vague, the skill names which standard it missed, so the reason is explicit, not just the next step.

## When the Text Came from GenAI
Sometimes the thing you need to check isn't your reasoning: it's a wall of confident text an LLM just handed you. That needs different questions, and this skill hands off rather than improvising them.

Walking someone back through how they reached a conclusion doesn't work on a model. Your reasons come before your conclusion. A model's are written front to back, each word picked on a loaded die: three faces for the likeliest word, two for the next, one for the outsider. Nothing was weighed or ruled out, so "what took you from the evidence to that?" gets you more text and no information.

That's a separate skill: **[Critical Thinking for GenAI](../critical-thinking-genai/)**. Install it alongside this one if you check AI output as well as your own thinking.

Mixed cases are common: a model drafted the text and you now own it. Then the GenAI probes go to what the model contributed, and the element questions above to what you decided to keep.

## When to Use It
- A conclusion you want stress-tested before you act on it
- A claim someone else made that you need to judge
- An argument that keeps going in circles
- A room where everyone agrees and it feels too easy
- Anything where being wrong would be expensive or hard to undo

**Trigger phrases:** "critical thinking", "check my reasoning", "poke holes in this", "is this a good argument", "am I missing something", "how do I know this is true"

## What It Won't Do
It won't agree just to be pleasant. LLMs have been trained to please human judges, not to provide factually correct information, so agreement is the cheap answer. The skill blocks that route: before affirming anything, it has to find the strongest objection and put that first.

It won't supply the evidence, the examples, or the counter-arguments. It asks where the evidence came from instead, because reasoning that arrives ready-made is harder to defend when someone pushes back on it.

And it is told to hold any fact it contributes to the same accuracy standard as yours. Expect it to miss some. A model has no reliable way to sort its own verified claims from its invented ones, which is why the checking belongs to you.

## Related
Use **[Critical Thinking for GenAI](../critical-thinking-genai/)** when the text under examination came out of a model rather than out of you. Use **[Systems Thinking](../systems-thinking/)** when the problem keeps coming back and you want to understand why. Use this one when you have a claim, a conclusion or a decision and need to know whether it holds up. Critical Thinking and Systems Thinking overlap on assumptions and perspective, and running one after the other works well.

## What's in Here
- `SKILL.md` - the workflow Claude follows
- `references/entry-points.md` - the opening question and where each answer routes
- `references/elements-of-reasoning.md` - the eight elements as questions
- `references/intellectual-standards.md` - the nine standards, what each catches, and what failing it sounds like

## Installation
See [Installing a Skill](../../README.md#installing-a-skill) in the repository README.

In Claude Code, invoke it on demand with `/critical-thinking`, or let Claude reach for it when one of the trigger phrases turns up.

## Credit
The Elements of Reasoning and the Universal Intellectual Standards are the work of Richard Paul and Linda Elder at the [Foundation for Critical Thinking](https://www.criticalthinking.org). The questions here are one way of putting their framework to work in conversation.

## License
CC BY-SA 4.0 - https://creativecommons.org/licenses/by-sa/4.0/

Created by [Agile Pain Relief](https://agilepainrelief.com)
