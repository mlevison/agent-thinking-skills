---
name: systems-thinking
description: Trace a problem that keeps coming back to the feedback loops holding it in place, through questions rather than prescribed solutions. Use when the user says "systems thinking", "systemic", "feedback loops", "unintended consequences", "root cause", "interconnected", or brings a complex, multi-factor problem.
license: CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/
metadata:
  author: agilepainrelief.com
  version: '0.35'
---

# Systems Thinking Analysis
Guide users through systemic analysis by selecting the appropriate framework and applying it conversationally.

## Workflow

1. **Expand perspective:**
   - Help the user zoom out from the immediately visible problem
   - Ask: What larger system is this problem part of?
   - Compare causes inside and outside the immediate context; choose the system boundary from evidence rather than assuming an external cause
   - Resist quick fixes — expand understanding first

2. **Determine temporal orientation:**
   - **Forward-looking** (planning, predicting, designing) → Explore potential consequences, feedback loops, leverage points
   - **Backward-looking** (diagnosing, understanding, post-mortem) → Trace causal chains and feedback within the system and across its boundary; distinguish observations from proposed mechanisms

3. **Select framework based on context:**
   - **Questions of a Systems Thinker** → Default for most analyses. See `references/questions-of-a-systems-thinker.md`
   - **Causal Loop Diagrams (CLDs)** → Use when:
     - User explicitly mentions "CLD", "Causal Loop Diagram", or asks for a visual/diagram
     - User has articulated 3+ interconnected variables or described circular causation ("A causes B which causes A")
     - User describes feedback loops, vicious/virtuous cycles, or reinforcing/balancing dynamics
     - The conversation has surfaced enough relationships that a picture would clarify the system
     - See `references/causal-loop-diagrams.md`

4. **Apply iteratively:**
   - Offer one lens or question at a time
   - Provide a one-sentence explanation of the concept
   - Ask a probing question to deepen the user's thinking
   - Let the user's response guide the next lens

## Conversational Style
- Curious, not prescriptive
- Surface assumptions and mental models
- Help users see connections they may have missed
- Encourage collaborative discovery with their team where relevant

## Evidence and boundaries

Treat the first causal map as a working hypothesis. For each important link, name its mechanism, supporting observation, uncertainty and a check that could overturn it. Include significant delays and scope limits. Broaden the boundary when a missing influence changes the explanation; do not assume a wider view is automatically more accurate. A reinforcing or balancing loop describes structure, not measured causal strength or a guaranteed trajectory.

## Attribution

Adapted from [Mark Levison / Agile Pain Relief systems-thinking skill](https://github.com/mlevison/systems-thinking/tree/9aaa506e513668bd8d1871473a65d2f5e960269c/skills/systems-thinking), licensed [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Modified by andromia3 to use evidence-led boundaries and explicit causal uncertainty; this adaptation remains under CC BY-SA 4.0.
