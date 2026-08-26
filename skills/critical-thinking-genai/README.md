# Critical Thinking for GenAI
Part of [Agent Thinking Skills](../../README.md).

An LLM created a large block of confident-sounding text, in response to a question you asked. You want to use it. Is it reliable? In the real world, we humans engage in [Critical Thinking](../critical-thinking/), a process that Richard Paul and Linda Elder have documented thoroughly. With human reasoning, we can ask questions about purpose, evidence, logic, etc. The questions guide us to better-reasoned answers. This doesn't work with GenAI.

## The Problem This Solves
Critical Thinking assumes a person reached a conclusion and can be walked back through how they got there. On an LLM there was no route to walk back.

Your reasons come before your conclusion. A model writes front to back, each word picked on a loaded die: three faces for the likeliest word, two for the next, one for the outsider. Text produced that way can look exactly like reasoning and still be only text. Asking an LLM "what took you from the evidence to that?" generates a fresh block of text about a process that never occurred.

This skill tests the output instead of asking the author.

And where a probe says to check something outside the model, another GenAI chat is not outside. The second model generates its answers the same way the first one did, so two of them agreeing is not corroboration. It can still be useful as a search tool. Ask it for the evidence on all sides of a claim, then go and read the sources it names. Draw your own conclusions.

## What You Get
Eleven probes, asked one at a time. Which ones you get depends on what being wrong would cost you. How confident the answer sounds tells you nothing.

- **Start a fresh conversation rather than correcting this one** - the most effective and least used tactic available. A thread carries its early wrong turns forward, and a correction revises the bad answer rather than replacing it. Carry a short brief to a new session, not the transcript: pasting the earlier answer in re-imports the anchor.
- **The reasons are written, not followed** - reading the reasoning won't prove it right or wrong. Find the claims that would collapse the whole thing if they were false, and check those. Or put the same evidence to a fresh session and ask for the opposite conclusion; if the reverse case comes back just as strong, the reasons were decoration.
- **It cannot say why it got something wrong** - asked "why did you make that mistake?", it writes a plausible explanation: specific, confident, and unconnected to what happened. Worse, the question, the wrong answer and the invented cause now all sit in the thread, and every later reply re-reads them.
- **Make it name the assumptions, then check them elsewhere** - unlike a question about a mistake, this one is worth asking: what comes back is a list of things to check. Take that list to a primary document, the actual data, or a person with direct knowledge.
- **Confidence is decoupled from reliability** - nothing in the output distinguishes a verified fact from an invented one. Don't ask the model whether it's sure; it has no basis on which to make that claim. Open every citation: sources that look right and do not exist are a routine output, not an edge case.
- **Your framing may have produced the answer** - ask why something is a good idea and you get reasons it is good. Re-ask with a neutral stance in a fresh session. If the answer changes with the framing, the original says more about your prompt than about the world.
- **It answered the question it recognised** - models settle on the nearest familiar question, and the substitution is silent. Which of your constraints were never in the prompt?
- **The default view is the average view** - consensus over-stated, well-argued minority positions understated, anything after the training cutoff thin or missing.
- **Hedging is not fairness** - "there are arguments on both sides" balances the presentation, not the evidence.
- **Vagueness marks the edges** - the output is deep where the training data was and generic where it wasn't, and there is no marker saying "beyond this point I'm relying on limited information."
- **Omissions leave no trace** - an answer that sounds complete reads exactly like one that is. This is the failure users catch least often.

## Where To Start Looking
Invented detail collects wherever the training data was thin: anything niche, local, recent. Or particular to your own situation: scale, budget, jurisdiction, what is already in place. Then look for key claims or assumptions.

## The Recursive Problem
Asking the LLM to run these checks on its own output has every failure mode above, and one more: it will defend text it produced.

The skill doesn't ask "was your earlier answer right?" It asks for the strongest objection to that answer instead, or takes it to a fresh session. And it must never be asked to account for a mistake it made earlier in the conversation, for the same reason no model can.

## When to Use It
- AI output you're about to rely on
- An answer that feels wrong
- Anything niche, local, recent, or specific to your situation
- A citation, a number, a name, a version
- A conclusion that sounds certain in a situation that lacks certainty
- Anywhere being wrong would be expensive

**Trigger phrases:** "is this AI answer any good", "did it make this up", "check what ChatGPT told me", "can I trust this", "verify this AI output", "hallucination"

## What It Won't Do
It won't confirm the output by asking another model. That is another generator, not a source.

It won't tell you the output is right or wrong when what it can actually say is that some claims need more evidence to verify.

And it is told to hold its own contributions to the same standard. Any fact, source or statistic it adds is subject to the check it asks of the output.

Expect it to miss some. An instruction is not a guarantee, and a model has no reliable way to sort its own verified claims from its invented ones, which is the whole reason the probes exist. So the answer to "will it flag its own errors?" is: sometimes, and you cannot tell which times. Which is why every check in this skill points at a source outside the model, including the checks on the model running it.

## Related
Use **[Critical Thinking](../critical-thinking/)** when the reasoning under examination is your own, and there is an author who can be walked back through it. Use **[Systems Thinking](../systems-thinking/)** when the problem keeps coming back and you need the structure holding it in place.

## What's In Here
- `SKILL.md` - the workflow Claude follows
- `references/probes.md` - the eleven probes, each with what it catches and what to do about it

## Installation
See [Installing a Skill](../../README.md#installing-a-skill) in the repository README.

In Claude Code, invoke it on demand with `/critical-thinking-genai`, or let Claude reach for it when one of the trigger phrases turns up.

## Credit
Critical Thinking is the work of Richard Paul and Linda Elder at the [Foundation for Critical Thinking](https://www.criticalthinking.org).

The eleven probes here are an original adaptation of Critical Thinking for GenAI, by [Mark Levison](https://agilepainrelief.com). Paul and Elder's questions assume an author who can be walked back through their reasoning. This skill starts where that assumption stops holding, and is not a restatement of their framework.

## License
CC BY-SA 4.0 - https://creativecommons.org/licenses/by-sa/4.0/

Created by [Agile Pain Relief](https://agilepainrelief.com)
