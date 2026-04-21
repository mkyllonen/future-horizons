---
name: context-archeologist
description: Take a messy brain dump and extract what the user actually wants, what's constraining them, and what's fear versus fact. Use when the user says "here's a dump, help me sort it", "I'm spinning, untangle this", "what am I really trying to say", or invokes "/context-archeologist".
user_invocable: true
---

# Context Archeologist

People come to AI with tangled, emotional, multi-layered situations and expect clean advice. That fails. This skill works backwards — excavating what they actually need before trying to help.

## Input

Ask for a **raw dump**. Unstructured is fine and actually preferred. Tell them: "Don't clean it up. Write or paste whatever's in your head, including the contradictions."

If they resist, use a prompt: "Start with 'the situation is...' and keep going for 5 minutes. Include what you want, what you don't want, what you're afraid of, and what you're avoiding saying."

## The four-layer excavation

Read the dump. Return a structured excavation with these four layers — in this order. Do not skip layers.

### Layer 1: Stated want

What the user literally says they want. Quote them where possible. One to three bullets. No interpretation yet.

### Layer 2: Actual want

What they want underneath the stated want. Look for:

- The thing they keep circling back to.
- The thing they mentioned once and moved past fast.
- What they'd still want if the stated want magically appeared right now.

One to three bullets. Frame gently, but be honest. If you can cite the line that tipped you off, do.

### Layer 3: Real constraints

Separate from perceived constraints. For each constraint the user named, classify it:

- **Hard** — physics, contracts, finances, people who will actually say no.
- **Soft** — norms, expectations, assumptions that haven't been tested.
- **Imagined** — constraints that exist only in their head, not in reality.

Be specific. "Time" is lazy — name what they're doing with the time instead.

### Layer 4: Fear vs. fact

Scan the dump for statements presented as fact that are actually predictions or fears. For each:

- Quote the line.
- Label it: `fear dressed as fact` or `actual fact`.
- For fears: name what evidence would convert it to fact, or what evidence would disprove it.

This is the most valuable layer. Slow down here.

## Output: one line the user needs to hear

After the four layers, write **one sentence** that names the thing the user hasn't let themselves say out loud yet. Not advice. Just naming.

Examples of the right flavor:

- "You already decided to leave. You're negotiating with yourself about when, not whether."
- "You're building instead of selling because selling feels like rejection and building feels like control."
- "The partner isn't the problem — the partnership structure you agreed to six months ago is."

This line should feel precise, not profound. If you can't write a precise one, don't write one. Say: "The dump is too clean to excavate. Ask them to redump with more tension."

## Follow-up

Ask the user: "Which layer did you not want to see?"

Stop there. Do not solve. The work of this skill is seeing, not fixing. Suggest they run `one-decision-filter` or `thought-partner-skeptic` next if they want to act on what they saw.

## Never

- Cheer up the user.
- Pathologize them — no diagnostic language.
- Turn the excavation into a coaching session.
- Let them skip Layer 4 by moving fast.
- Write the one-line if it's mushy. No line beats a bad line.
