# How to install — step by step

Written for anyone. No terminal required.

## Before you start

Pick one of these two paths:

- **Path A — Claude Code** (desktop or CLI). You'll install once and type `/skill-name` to use any skill.
- **Path B — Claude.ai in a web browser.** No install. You copy and paste the skill into a new chat.

If you're not sure which you have, use Path B.

---

## Path A — Claude Code (recommended)

### Step 1. Download the skills

1. Go to the top of this page on GitHub.
2. Find the green button that says **Code**.
3. Click it. A menu drops down.
4. Click **Download ZIP**.
5. A file called `future-horizons-main.zip` will download.

### Step 2. Unzip the file

**On Mac:** Double-click the zip file. A folder will appear next to it.

**On Windows:** Right-click the zip file → **Extract All** → click **Extract**.

You should now have a folder called `future-horizons-main`. Open it. Inside, you'll see a folder called `.claude`. **That's the folder you need.**

> The folder starts with a dot. On Mac you may need to press `Cmd + Shift + .` in Finder to see it. On Windows you may need to enable "Hidden items" in File Explorer's View menu.

### Step 3. Find your home `.claude` folder

This is where Claude Code looks for skills.

**On Mac:**

1. Open Finder.
2. In the top menu: **Go** → **Home**. (Or press `Cmd + Shift + H`.)
3. Press `Cmd + Shift + .` to show hidden folders.
4. Look for a folder called `.claude`. If it doesn't exist, make one: right-click → **New Folder** → name it exactly `.claude`.
5. Open `.claude`. If there's no folder called `skills` inside, make one.

**On Windows:**

1. Open File Explorer.
2. Click in the address bar. Type `%USERPROFILE%` and press Enter. This opens your home folder.
3. Enable hidden items: **View** menu → **Show** → **Hidden items**.
4. Look for a folder called `.claude`. If it doesn't exist, make one: right-click → **New** → **Folder** → name it exactly `.claude`.
5. Open `.claude`. If there's no folder called `skills` inside, make one.

### Step 4. Copy the skills in

From the `future-horizons-main` folder you unzipped:

1. Open `.claude/skills/` inside the unzipped folder.
2. Select all 3 skill folders.
3. Copy them: `Cmd + C` on Mac, `Ctrl + C` on Windows.
4. Go to your home `.claude/skills/` folder (from Step 3).
5. Paste them: `Cmd + V` on Mac, `Ctrl + V` on Windows.

You should now have 3 new folders inside `~/.claude/skills/`. (If you already installed Pack 1, these sit alongside the existing seven.)

### Step 5. Restart Claude Code

Fully quit Claude Code and open it again. This makes it notice the new skills.

### Step 6. Test it

Open any conversation in Claude Code. Type:

```
/one-decision-filter
```

Claude should activate the skill and ask you to state the decision. If it does, you're done.

If it doesn't recognize the command, see **Troubleshooting** below.

---

## Path B — Claude.ai in a web browser

No install required.

### Step 1. Open a skill file

Pick a skill from the list in the main README. Click into its folder on GitHub. Open `SKILL.md`.

### Step 2. Copy the instructions

You'll see a block at the top that looks like this:

```
---
name: skill-name
description: ...
---
```

**Skip that block.** Select everything below it — all the way to the end of the file. Copy it.

### Step 3. Start a new Claude chat

1. Go to [claude.ai](https://claude.ai).
2. Start a new conversation.
3. Paste the instructions you copied as your very first message.
4. Press Enter and wait for Claude to acknowledge.
5. Now type your situation.

The skill will run for that conversation. Start a new chat to use a different skill.

---

## Troubleshooting

**Claude Code doesn't find the skill when I type `/one-decision-filter`.**

- Check that the folder is exactly at `~/.claude/skills/one-decision-filter/SKILL.md`.
- The folder must be named exactly `one-decision-filter` (lowercase, hyphens, no extras).
- The file inside must be named exactly `SKILL.md`.
- Fully quit and reopen Claude Code.

**I can't see the `.claude` folder in my home directory.**

- It's a hidden folder. On Mac, press `Cmd + Shift + .` in Finder. On Windows, enable "Hidden items" in File Explorer's View menu.

**The skill runs but feels flat.**

- These skills work on real input. Vague input = vague output. The more specific and honest your dump, decision statement, or intention, the sharper the result.

**I want to update a skill.**

- Download the repo again and replace the folder in `~/.claude/skills/`. Your own saved files stay where you put them.

---

## Removing the skills

Delete the 3 folders from `~/.claude/skills/`. That's it.
