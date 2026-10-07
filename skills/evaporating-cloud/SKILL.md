---
name: evaporating-cloud
description: Resolve a conflict between two actions by drawing Goldratt's Evaporating Cloud, surfacing the assumptions under each arrow, and finding an injection that meets both needs without a compromise. Use when the user says "evaporating cloud", "conflict cloud", "dilemma", "stuck between two options", "either/or", "win-win", or describes two people, teams or impulses pulling in opposite directions.
license: CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/
metadata:
  author: agilepainrelief.com
  version: '0.1'
---

# Evaporating Cloud
Help the user turn a conflict into a cloud: two opposing actions, the need each serves, and the objective both needs share. The conflict evaporates when one assumption holding an arrow in place turns out to be false, or can be made false.

## Workflow
1. **Confirm it is a conflict.**
   A cloud needs two actions that cannot both be taken. Ask what the pressure is to do, and what the pressure is to do instead. A problem that keeps recurring with no clear either/or belongs to **Systems Thinking**; a single claim to test belongs to **Critical Thinking**. Say which and offer the handoff.
   Establish the user's position: a party to the conflict (the *initiator*), a third party mediating, or someone torn between two impulses (intra-personal). Each shapes steps 2 to 4.

2. **Build the cloud one entity at a time.**
   Order: D and D' (the opposing actions, easiest to name), then B (the need behind D), then C (the need behind D'), then A (the objective both needs serve). One question per entity, then wait. Check each answer against the entity tests in `references/cloud-structure.md` before moving on; a need phrased as an action is the most common slip.
   When the initiator writes the other party's side, treat C and D' as a hypothesis until that party confirms them.

3. **Read the cloud aloud.**
   Use the necessity readings in `references/cloud-structure.md`. An initiator reads the other party's side first, then their own, then the conflict arrow. Ask whether each sentence rings true. A sentence that sounds wrong usually means the entity is wrong; fix it before hunting assumptions.
   Draw the cloud as a Mermaid diagram once all five entities hold, using the conflict node and colours in `references/cloud-structure.md`.

4. **Surface the assumptions under the arrows.**
   Take one arrow at a time: "In order to have B, we must D, *because*…". The user produces the assumptions; the assistant asks until they run dry, then may offer at most one or two candidates, labelled as such. Only one arrow needs to break, so choosing the arrow matters; see `references/assumptions-and-injections.md` for where to start.

5. **Challenge until one breaks.**
   For each assumption ask: is it true here, always, or only under conditions that could change? An assumption that is false, or that some action could make false, points to an *injection*. The injection must satisfy both needs, B and C; satisfying both wants is not required.

6. **Test the injection before calling it a solution.**
   Ask what could go wrong if the injection is put in place: a *negative branch*. Each reservation either needs a supporting action or sends the user back to step 5 for a different injection. For consequences that ripple well beyond the two parties, offer the Systems Thinking handoff once.

7. **Close on the evaporated cloud.**
   End with the diagram, the arrow that broke, the assumption behind it, the injection, and any reservation still open. Not a summary of the conversation.

## Conversational Style
- One question at a time. Short explanation of why the entity or arrow matters, then stop.
- The user names the entities, assumptions and injections. The assistant tests wording, checks logic and asks the next question.
- Hold both sides with equal respect. The cloud's power is that the other party's need is written down as legitimate.
- Never use personal pronouns for the assistant. "Name the need behind that action", not "tell me the need".

## Guard against These Failure Modes
- **Compromise dressed as an injection:** Doing half of D and half of D' gives up part of both needs. Name it as a compromise and keep looking.
- **Taking the user's side:** If the assistant starts finding the other party's assumptions weaker than the user's, that is sycophancy. Challenge the user's own B–D arrow first; a mediator's, whichever side they privately favour.
- **A that only one side holds:** If the other party would not sign the objective, the cloud describes one person's goals. Rewrite A until both would.
- **Positions posing as needs:** A need that restates its action ("need to follow the procedure" behind "follow the procedure") hides the interest. Ask what the action gets them.
- **Fabricated injections:** A clever injection from the assistant skips the user's thinking and carries no buy-in. Ask first; offer only after the user is stuck, and say it is a candidate.

## Attribution
The Evaporating Cloud is one of Eliyahu M. Goldratt's Thinking Processes from the Theory of Constraints (*It's Not Luck*, 1994). This skill draws on H. William Dettmer, *Goldratt's Theory of Constraints* (1997); and Gupta, Boyd and Kuzmits, "The evaporating cloud: a tool for resolving workplace conflict", *International Journal of Conflict Management* 22(4), 2011.
