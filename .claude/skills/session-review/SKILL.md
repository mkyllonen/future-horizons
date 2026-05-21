---
name: session-review
description: Process any conversation, thread, or work session to extract lessons, spot patterns, and append them to the user's lessons.md. Run at the end of meaningful sessions to capture compound learning. Suggests (never auto-applies) updates to CONTEXT.md or HEARTBEAT.md when patterns warrant. Use when the user says "run session-review", "capture the lessons from this", "what did we learn here", "review this session", or invokes "/session-review".
user_invocable: true
---

# Session Review Skill

## Purpose

This skill is the compound loop's writing layer. Every session you have with Co-You, every coding session in Cowork or Claude Code, every meaningful conversation you want to capture — point this skill at it, and it does the lesson extraction for you.

## When to invoke

Invoke this skill when:
- You finish a Co-You session that produced something useful
- You complete a coding/marketing/build session in Cowork or Claude Code
- You wrap a client call or meeting where lessons emerged
- Anytime you'd otherwise close the tab and forget what just happened

## How to use

Share the session content with Co-You and say: "Run session-review on this."

Or paste a transcript, conversation export, or session log and invoke the skill by name.

## What the skill does

When invoked, the skill:

1. **Reads your context files** — SOUL.md, CONTEXT.md, HEARTBEAT.md, and lessons.md (if it exists). This ensures the lessons it captures are calibrated to your actual operating system, not generic.

2. **Analyzes the input session** along these dimensions:
   - What decisions were made and why
   - What worked and what didn't
   - Patterns or themes that emerged
   - Insights worth keeping
   - Mistakes or false starts worth not repeating
   - Open questions or follow-ups

3. **Extracts lessons** in this format:

   ```
   ## [YYYY-MM-DD] [Brief lesson title]

   **Context:** [One-line description of the session that produced this lesson]

   **Lesson:** [The lesson itself, written as a directive or principle]

   **Why it matters:** [Why this lesson is worth keeping — what it prevents or enables]

   **Tags:** [Optional: areas of business this applies to, e.g., sales, ops, content]
   ```

4. **Appends lessons to lessons.md** — Creates the file in your root directory if it doesn't exist. Always appends; never overwrites. Most recent lessons go at the top.

5. **Suggests updates to other files** — If a pattern in the session strongly suggests your CONTEXT.md or HEARTBEAT.md is out of date, the skill flags this. It does NOT auto-apply. It tells you what it noticed and lets you decide.

6. **Returns a summary** showing:
   - Number of lessons extracted
   - Preview of each lesson title
   - Any suggested updates to other files
   - Confirmation that lessons.md was updated

## What this skill does NOT do

- It does not auto-modify CONTEXT.md, HEARTBEAT.md, or any file other than lessons.md
- It does not delete or overwrite existing lessons
- It does not write lessons that are generic or could apply to anyone — every lesson is grounded in YOUR session and YOUR context
- It does not capture every observation — only ones that pass a "worth keeping six months from now" filter

## Setup requirement

This skill expects:
- SOUL.md, CONTEXT.md, HEARTBEAT.md in your root or accessible to Co-You
- CLAUDE.md updated to reference lessons.md on every conversation (the one-time setup)

If lessons.md doesn't exist yet, the skill creates it on first run.

## The CLAUDE.md one-time setup

Add this section to your CLAUDE.md so Co-You reads lessons every conversation:

```markdown
## Lessons Loop

At the start of every conversation, read lessons.md from the root directory.
Treat the contents as accumulated operating knowledge. Reference relevant
lessons when they apply to the current work. Do not list lessons unprompted;
use them as context for sharper responses.
```

That's it. Once this section is in CLAUDE.md, the loop is live. Run session-review whenever you want to capture a lesson. Co-You reads what you've captured on every conversation thereafter.

## Example invocation

```
You: "Run session-review on the conversation we just had about pricing the
new offer. Capture what we figured out."

Co-You: [reads SOUL.md, CONTEXT.md, HEARTBEAT.md, lessons.md]
        [analyzes the pricing conversation]
        [extracts 2 lessons]
        [appends to lessons.md]
        [returns summary]

Co-You: "Captured 2 lessons:
1. [2026-05-21] Anchor pricing to outcome value, not delivery time
2. [2026-05-21] Premium positioning requires premium friction in qualifying

Suggested update: Your HEARTBEAT.md still lists 'finalize pricing model'
as a priority. Based on this session, that may be ready to close out.
Want me to update HEARTBEAT.md or leave it for you to review?

lessons.md updated."
```

## Maintenance

- Review lessons.md weekly during your Friday touchpoint
- Archive or consolidate old lessons quarterly (don't delete; move to lessons-archive.md)
- If lessons.md grows past 500 lines, ask Co-You to help cluster and consolidate

## Final note

This skill is the compound loop's writing arm. The loop only works if you actually run the skill. The compound only happens if the loop runs. The result only shows up six months in.

Trust the loop. Run the skill. Watch what becomes possible.
