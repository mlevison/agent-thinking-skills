# GenAI Strangeness
// This file is a placeholder please ignore for now
Ways these tools behave that don't match what the interface suggests. Not a list of failure modes and not advice - the skills in this repo handle those. This is the machinery underneath, for anyone who wants to know why the advice is what it is.

Nothing here is a defect. It is all working as built.

## Every Reply Re-reads The Whole Conversation
There is no running state. Each answer is produced by reading the entire transcript again from the top, then continuing it. A one-line follow-up at the end of a long thread costs a full re-read of everything above it.

Two consequences. Cost and latency climb as a conversation grows, and they climb with the length of the thread rather than the length of your question. And a thread that took a wrong turn early carries that turn into every later answer, because it is still there in the text being re-read.

## Nothing Carries Between Conversations
Close the window and it is gone. There is no accumulated understanding of you, your project or your preferences waiting in the next session.

Where a product appears to remember, a separate mechanism is doing it - notes written to a file and pasted in at the start of the next conversation. Useful, but it is a filing system bolted on the side, not the model recalling anything.

## There Is No Inside To Look At
A model cannot inspect the process that produced its earlier words. Asked why it said something, it composes a fresh explanation that fits. The result reads like recollection and is not.

The same holds in the moment. Explanation and answer are written together, left to right, so text that appears to reason toward a conclusion may have been generated after that conclusion was already committed to.

## The Same Prompt Gives A Different Answer
Output is sampled rather than computed. At every word the model holds a ranked list of candidates and rolls a loaded die to choose one: three faces for the likeliest word, two for the next, one for the outsider. Ask twice and the wording differs; sometimes the substance does too.

The loading is what keeps the result coherent. The likeliest word usually wins, which is also why answers to the same question rhyme with each other and with the most common position in the training data. The die is why they are never identical.

Any single answer is one draw, not the model's position. This is the one piece of strangeness that works in your favour - re-running a question is cheap and tells you whether the answer is stable.

## Fluency Costs Nothing
Well-formed prose is what these systems produce regardless of whether the content is right. Confidence in the writing is not evidence about the world.

The register does not change at the edge of what the model has data for. No hesitation, no hedge, no drop in polish - the sentence that invents a citation is built the same way as the one that reports a real study.

## It Cannot Tell You What It Read
There is no index of the training data and no way to check whether a particular document was in it. "Where did you learn that?" gets a plausible answer rather than a true one.

## Position In The Input Matters
Material near the start and end of a long input carries more weight than material in the middle. A constraint mentioned once, twenty messages back, is more likely to be quietly dropped than one restated in the current message.

## The Training Cutoff Is A Soft Edge
Coverage thins for months before the stated date rather than stopping at it - recent events are represented by less text than settled ones, because the internet had not finished writing about them yet.

The model's own account of its cutoff is unreliable too. That date is a fact it absorbed from training text, not something it can observe about itself.

## Agreement Is Trained In
These models are tuned against human ratings, and humans rate agreement well. The pull toward telling you that your idea is a good one is not a quirk of a particular product - it is the shape of the training.

What suffers most is the thing you most need: a flat contradiction of something you have already asserted.

## Tokens Are Not Letters
Text is split into chunks before the model sees it, and those chunks rarely line up with characters or digits. Counting the letters in a word, reversing a string, or doing arithmetic on long numbers fails for reasons unconnected to how hard the task is.

## Search Changes What It Is
A model answering from training data and a model that has just fetched a page are doing different things, and the output looks identical.

Worth knowing which one you are talking to. With retrieval, the failure shifts from invention to bad sources and stale pages. Without it, everything comes from what was absorbed during training, cutoff and all.
