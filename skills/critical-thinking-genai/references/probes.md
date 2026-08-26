# Probes
Eleven probes for text a model produced. Choose by what it would cost to be wrong, not by how sure the answer sounds. Do not run all of them.

Where a probe says to check something outside the model, another GenAI chat is not outside. The second model generates its answers the same way the first one did, so two of them agreeing is not corroboration. It can still be useful as a search tool. Ask it for the evidence on all sides of a claim, then read the sources it names and let the user draw their own conclusions.

## Start A Fresh Conversation Rather Than Correcting This One
The most effective and least used tactic available. Say so explicitly, most users do not know it is an option.

A thread carries its early wrong turns forward. A correction revises the bad answer rather than replacing it, and the revision stays anchored to it. Length costs as well: the whole conversation is re-read to produce every new answer.

Make the restart cheap.

- Carry a short brief, not the transcript: the restated question, the constraints missing the first time, the facts established since.
- Do not paste the earlier answer in, that re-imports the anchor.
- The work so far bought a better question. Ask what is known now that was not known at the first prompt, and open with that.
- Run the brief in a new session alongside the old one and compare the two answers.

## The Reasons Are Written, Not Followed
A person's reasons come before their conclusion, which is why walking someone back through them works. A model writes front to back, each word picked on a loaded die: three faces for the likeliest word, two for the next, one for the outsider. Text produced that way can look like human reasoning and still be just text.

Reading the reasoning output will not prove it right or wrong. Find and test the claims in the reasoning instead.

- Which claims, if false, would collapse this? There may be one, there may be several. Check them outside this model, with a strong preference for finding human-authored sources that test them.
- Put the same evidence to a fresh session and ask for the opposite conclusion. It has to be fresh. In this thread the original answer is still in context and the request reads as an instruction to play along. If the reverse case comes back just as strong, the reasons were decoration.

## It Cannot Say Why It Got Something Wrong
When an error surfaces, the reflex is to ask what happened. Do not.

The model doesn't understand that it made a mistake, nor does it have a real understanding of how it got there. Asked "why did you make that mistake?", it writes a plausible explanation: specific, confident, and unconnected to what happened.

The real problem: the question, the wrong answer and the invented cause now all sit in the thread, and every later reply is produced by re-reading them. The mistake has been restated, elaborated, and given a reason to be there.

Start again in a new thread. Restate the question, carry the learnings picked up along the way, and name what the first prompt lacked: a constraint, a source, a definition, an ambiguity that got resolved the wrong way.

## Make It Name The Assumptions, Then Check Them Elsewhere
Generated claims rest on assumptions, often left unstated. Unlike a question about a mistake, a question about assumptions is worth asking: what comes back is a list of things to check.

- Ask for the assumptions behind the claim as a plain list. Then ask which of them, if wrong, changes the conclusion.
- That list is generated too, so it is more likely than human reflection to miss the case that matters. Treat it as a starting point, not a complete list.
- Take the assumptions to a human-authored source: the primary document, the actual data, a person with direct knowledge. Another model can point at candidate sources, but it cannot confirm an assumption, it may be relying on equally flawed data.
- Invented detail collects wherever the training data was thin: anything niche, local, recent, or particular to the user's own situation - scale, budget, jurisdiction, what is already in place. Start there, and the user can usually check it faster than anything else in the output.

## Confidence Is Decoupled From Reliability
Fluency costs a model nothing. Nothing in the output distinguishes a verified fact from an invented one. Even when the model shouldn't be confident, it still sounds that way.

- Pick what to check by what it would cost to be wrong, not by how sure the answer sounds.
- Do not ask the model whether it is sure, and do not accept a confidence figure it gives. It has no basis on which to make such a claim.
- Open every citation. Sources that look right and do not exist are a routine output, not an edge case.

## Your Framing May Have Produced The Answer
Ask why something is a good idea and you will get reasons it is good. Sentiment expressed in the question, or anywhere in the discussion, is baked into the answer. LLMs have been trained to please human judges, not to provide factually correct information.

- List what the wording took for granted. Anything asserted in the question comes back unchallenged.
- Rewrite the question with a neutral stance. Ask the updated question in a fresh session.
- If the answer changes with the framing, the original says more about the prompt than about the world.

## It Answered The Question It Recognised
Models settle on the nearest familiar question, and the substitution is silent.

- Write down the question this output actually answers. Compare it with the one you asked.
- Which of your constraints were never in the prompt - budget, org, regulatory setting, prior decisions? Those are absent from the answer, not weighed and dismissed.

## The Default View Is The Average View
GenAI is trained on all of the text on the internet. The output of these tools regresses toward the most represented position. Consensus is over-stated, well-argued minority positions are understated, and anything after the training cutoff is thin or missing.

- Ask the model: "Who disagrees with this, and what do they argue?" It will name people and positions.
- Search one of those names outside the model. A real argument that the first answer never mentioned means the model missed key viewpoints.
- Anything that changes quickly - prices, tools, versions, law, current practice - is where the training cutoff hits. Assume the answer is out of date and find a source with a date on it.

## Hedging Is Not Fairness
"There are arguments on both sides" balances the presentation, not the evidence. False balance reads as even-handedness.

- Does it commit anywhere? Where the evidence genuinely favours one side, did the output say so?
- Are the two sides given equal weight because the evidence is equal, or because equal weight sounds fair?

## Vagueness Marks The Edges
The model's output is deep where it had more training data and generic where it did not. Unfortunately, there is no marker in the output saying: "Beyond this point I'm relying on limited information."

- Mark every point where the answer turns general.
- Ask for specifics at exactly those points: numbers, names, steps, a worked example. What is still vague is a gap.

## Omissions Leave No Trace
An answer that sounds complete reads exactly like one that is. Nothing points at what was left out, which is why this is the failure users catch least often.

- In a fresh session, ask what a good answer to the original question would have to cover. Do not paste in the answer already received, because shown that, the model marks its own work generously.
- Compare the two lists. Whatever appears on the checklist but not in the answer is the omission.
- Ask "when would this be the wrong thing to do?" Advice tends to arrive without its exceptions.
