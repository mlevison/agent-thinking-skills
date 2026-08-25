# Critical Thinking
Part of [Agent Thinking Skills](../../README.md).

You've made up your mind. You're fairly sure you're right. And the only person available to check is the one who just agreed with everything you said.

This skill asks the questions a good colleague would ask, in the order that actually helps.

## The Problem This Solves
Reasoning fails quietly. Not with an obvious error, but with a word two people define differently, an assumption nobody stated, a piece of evidence nobody went looking for because it would have been inconvenient.

You can't spot these from inside your own position. That's the whole difficulty - the assumption you can't see is the one doing the most work.

Richard Paul and Linda Elder broke reasoning into eight parts you can examine one at a time, and nine standards you can hold any answer to. This skill turns both into questions.

## It Starts By Asking Where You Are
Most frameworks march you through their steps from the top. That's how you end up being asked "what's your purpose here?" when you've spent two days buried in data and want to know whether it means what you think it means.

So the first question is about you, not your argument: **where are you with this right now?**

- Still working out what you're deciding
- Gathering evidence
- Trying to make sense of what you've got
- Testing a conclusion you've already reached
- Judging something somebody else told you
- About to commit, and want a last look

Your answer picks the starting point. From there it follows wherever your reasoning is thinnest - which is usually your assumptions or your point of view, because those are the two things invisible from where you're standing.

## What You Get
Eight lenses, offered one question at a time:

- **Purpose** - what you're actually trying to accomplish, and whose goal it really is
- **Question at Issue** - the question you're settling, and whether it's secretly three questions
- **Information** - what your evidence is, where it came from, and what would count against you
- **Inferences** - where the evidence stops and your interpretation starts
- **Concepts** - the key terms, and whether two people would define them the same way
- **Assumptions** - what you're taking for granted, and which one collapses everything if it's wrong
- **Point of View** - what your frame shows you, and what it hides
- **Implications** - what follows if you're right, what it costs if you're wrong, and who pays

And nine standards used to test your answers rather than start conversations: **clarity, accuracy, precision, relevance, depth, breadth, logic, significance, fairness.** When an answer is vague, the skill names which standard it missed - so you learn the tool, not just the verdict.

## It Also Interrogates AI Output
Sometimes the thing you need to check isn't your reasoning - it's a wall of confident text a model just handed you. That needs different questions.

Walking someone back through how they reached a conclusion doesn't work on a model. Your reasons come before your conclusion. A model's are written front to back, each word picked on a loaded die: three faces for the likeliest word, two for the next, one for the outsider. Nothing was weighed or ruled out, so "what took you from the evidence to that?" gets you more fluent text and no information.

So this mode tests the output instead of asking the author:

- **Start over rather than correct** - the most effective and least used tactic. A thread carries its early wrong turns forward, and a correction revises the bad answer rather than replacing it. Take a short brief to a fresh session, not the transcript.
- **It can't tell you why it got something wrong** - ask what happened and you'll get a specific, confident, invented cause. Worse, asking leaves the mistake and the fake reason sitting in the thread, where every later answer re-reads them. Repair the prompt and start again instead.
- **Make it name its assumptions, then check them somewhere else** - ask which assumptions the claim rests on and which one, if wrong, changes the answer. Then verify those against a real source. An assumption confirmed by the model that produced it isn't confirmed.
- **The reasons may be decoration** - find the one claim that would collapse the whole thing if it were false, and check that. Or put the same evidence to a fresh session and ask for the opposite conclusion; if the reverse comes back just as convincing, the reasons were decoration.
- **Confidence tells you nothing** - it reads exactly the same whether it's citing a real paper or one it invented. Choose what to check by what it would cost you to be wrong, not by how sure the answer sounds. Don't ask the model if it's sure; it doesn't know.
- **Your framing may have written the answer** - ask why X is a good idea, get reasons X is good. Re-ask neutrally in a fresh session. If the answer flips, it was describing your prompt, not the world.
- **It may have answered a nearby question** - write down what it actually answered and compare.
- **The default view is the average view** - consensus over-stated, good minority positions under-stated, anything recent thin or missing.
- **Hedging isn't fairness** - "both sides have a point" balances the presentation, not the evidence.
- **Vagueness marks the edges** - where it goes generic is usually where it knows least, and nothing in the tone warns you.
- **Omissions leave no trace** - a complete-sounding answer and a complete answer read the same.

There's a recursive problem too, and the skill names it: the assistant running these checks is itself a model, and it will defend text it wrote. Ask it for the strongest objection to its own earlier answer rather than whether that answer was right - or take it to a fresh session.

## When to Use It
- A conclusion you want stress-tested before you act on it
- AI output you're about to rely on, forward, or paste into something that matters
- A claim someone else made that you need to judge
- A decision that's hard to reverse
- An argument that keeps going in circles
- A room where everyone agrees and it feels too easy
- Anything where being wrong would be expensive

**Trigger phrases:** "critical thinking", "check my reasoning", "poke holes in this", "is this a good argument", "am I missing something", "how do I know this is true", "did it make this up", "can I trust this AI answer"

## What It Won't Do
It won't agree with you to be pleasant. Sycophancy is the default failure mode of an AI asked to review your thinking, and this skill is built to push against it: before affirming anything, it has to find the strongest objection and put it to you.

It also won't do your homework. It asks where your evidence came from rather than going and finding some for you - because reasoning you didn't build isn't reasoning you can defend.

And any fact it contributes is held to the same accuracy standard as yours. If it can't verify something, it says so.

## Related
Use **[Systems Thinking](../systems-thinking/)** when the problem keeps coming back and you need to understand the structure holding it in place. Use this one when you have a claim, a conclusion or a decision and need to know whether it holds up. They overlap on assumptions and perspective - and running one after the other works well.

## What's In Here
- `SKILL.md` - the workflow Claude follows
- `references/entry-points.md` - the opening question and where each answer routes
- `references/elements-of-reasoning.md` - the eight elements as questions
- `references/intellectual-standards.md` - the nine standards, what each catches, and what failing it sounds like
- `references/interrogating-genai-output.md` - probes for text a model produced, where walking back through the reasoning doesn't work

## Installation
See [Installing a Skill](../../README.md#installing-a-skill) in the repository README.

## Credit
The Elements of Reasoning and the Universal Intellectual Standards are the work of Richard Paul and Linda Elder at the [Foundation for Critical Thinking](https://www.criticalthinking.org). The questions here are one way of putting their framework to work in conversation.

## License
CC BY-SA 4.0 - https://creativecommons.org/licenses/by-sa/4.0/

Created by [Agile Pain Relief](https://agilepainrelief.com)
