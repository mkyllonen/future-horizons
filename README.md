# Future Horizons — Pack 2

Four Claude Code skills for the hard stuff: deciding when you're stuck, sorting yourself when you're spinning, following through when it matters, and capturing what you learned so it compounds.

Pack 2 of a series. Pack 1 lives at [redesigned-existence](https://github.com/mkyllonen/redesigned-existence).

No API keys. No Python. Drop four folders in the right place and you're done.

## What you get

| Skill | What it does | When to use |
|---|---|---|
| `one-decision-filter` | Five sharp questions + a verdict. Kills paralysis. | When you've been stuck on a choice for more than a day |
| `context-archeologist` | Take a messy brain dump. Return what you actually want vs. what you said, real vs. imagined constraints, fear dressed as fact | When you're spinning and can't tell why |
| `accountability-artifact` | Generate a thing that costs you something if you don't follow through — not a reminder, a consequence | When you need to stop relying on willpower |
| `session-review` | Mine a session or conversation for lessons, append them to your `lessons.md`. The compound loop's writing layer | When you finish a meaningful session and don't want to lose what you learned |

Each skill is a single markdown file. No code runs. Claude reads and follows.

## Install in 60 seconds

See **[INSTALL.md](INSTALL.md)** for the exact step-by-step. Made for people who have never used a terminal.

Short version:

1. Download this repo (green **Code** button at top → **Download ZIP**).
2. Unzip it.
3. Copy the `.claude/skills/` folder into your home folder (Mac: `~/.claude/skills/`. Windows: `C:\Users\YourName\.claude\skills\`).
4. Open Claude Code.
5. Type `/one-decision-filter` or any other skill name.

If you already installed Pack 1, these four folders just go in next to the existing seven. Nothing conflicts.

## Use in Claude.ai (web, no install)

Every skill also works in Claude.ai without any install:

1. Open any `SKILL.md` file in this repo.
2. Copy everything **below** the block that starts and ends with `---`.
3. Paste it as your first message in a new Claude chat.
4. Type your situation after.

## How Pack 2 pairs with Pack 1

These four skills compound with Pack 1 skills:

- **`context-archeologist`** → once you've excavated, run `one-decision-filter` to act on what you saw.
- **`one-decision-filter`** → once you decide, log it with `decision-journal` (Pack 1).
- **`accountability-artifact`** → once you commit, revisit it in `weekly-compound` (Pack 1) next Friday.
- **`session-review`** → when the work wraps, mine the session for lessons and feed them back into your `lessons.md` so next time starts sharper.

You can use them independently. They just get sharper together.

## What makes these different

Pack 1 sharpened your output. Pack 2 sharpens your actions.

- `one-decision-filter` doesn't give you more options. It makes you pick one.
- `context-archeologist` doesn't make you feel better. It makes you see clearly.
- `accountability-artifact` doesn't set a reminder. It sets a cost.
- `session-review` doesn't summarize the session. It extracts what's worth keeping six months from now.

The theme: AI that works against your default of staying stuck, not with it.

## License

MIT. Use them, remix them, share them, sell products on top of them. Keep the attribution.

## Built by

[Max Kyllonen](https://github.com/mkyllonen) — AI implementation consultant. Pack 2 of a series.

Pack 3 coming. Follow or watch the repo for drops.

---

**Troubleshooting, feedback, or ideas for Pack 3?** Open an issue on this repo.
