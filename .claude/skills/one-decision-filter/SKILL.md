---
name: one-decision-filter
description: Kill decision paralysis with five sharp questions and a verdict. Use when the user says "help me decide", "I'm stuck on this choice", "run it through the filter", or invokes "/one-decision-filter".
user_invocable: true
---

# One Decision Filter

Paralysis is almost always a symptom of one of two things: the wrong question or missing information. This skill surfaces which, then forces a verdict.

## Input

Ask the user to state **the decision** in one sentence. If they can't, that's the first tell — their framing is fuzzy. Help them sharpen it first.

Acceptable forms:

- "Should I X or Y?"
- "Should I X, yes or no?"
- "X by [date] or push it?"

Unacceptable forms (rewrite with the user):

- "What should I do about X?" (too open)
- "How do I think about X?" (not a decision)
- "I'm worried about X." (not a decision)

## The five questions

Ask one at a time. Wait for each answer before moving on. Each question has a purpose — don't explain it to the user, just ask.

1. **What's the cost of being wrong?**
   (Reveals reversibility. Cheap reversal = just pick and move.)

2. **What do you already know the right answer is?**
   (Cuts through analysis. Often the answer is already there and they're hunting for permission.)

3. **What's the one piece of information that would make this obvious?**
   (Surfaces whether this is actually a research problem disguised as a decision.)

4. **Who are you avoiding disappointing by not deciding?**
   (Exposes social drag. Often the real block is a person, not the choice.)

5. **If you had to decide in the next 10 minutes, what would you pick?**
   (Time pressure collapses fake optionality.)

## Verdict

After the five answers, return one of these four verdicts. No hedging.

- **Decide now: [X].** The answers make it obvious. State the call and the reasoning in two sentences.

- **Get the data first.** Question 3 named a specific piece of missing information. State what it is, how to get it, and by when. After that, revisit.

- **It's not about the decision.** Questions 2 or 4 revealed the real block is emotional, social, or identity-level. Name it. Suggest one thing they could do to unblock — but do not pretend it's a tactical problem.

- **Reversible — just pick.** Question 1 showed low cost of reversal. Tell them to flip a coin or go with gut and commit. The time spent deciding now costs more than a wrong pick would.

## After the verdict

Ask: "Are you going to do it?"

- If yes — log the decision (suggest the `decision-journal` skill if available) and move on.
- If no — one follow-up question: "What would have to be true for you to do it?" Do not loop back into the filter. The filter is done. The next conversation is about the block, not the choice.

## Never

- Run through the five questions without waiting for real answers.
- Offer a fifth option when the user framed it as binary.
- Soften the verdict.
- Let the user stay in analysis when question 3 had no real answer.
