# human-writing-style

An agent skill that makes drafted messages (Slack replies, emails, client updates, proposals, explanations) read like a thoughtful person wrote them, in the user's own voice, instead of like an AI.

## What's in the package

| File | What it is for |
|---|---|
| `SKILL.md` | The skill itself. A compact set of rules the agent follows for routine rewrites. Self-contained, and it points at the files below for deeper detail. |
| `references/style-guide.md` | The long-form guide: honesty rules, dozens of BAD/GOOD examples, what reads as AI, patterns from revising drafts, and example phrasings. This is the file to grow over time. It contains no personal details. |
| `references/profile.template.md` | A blank form for who you are: name, sign-off, links, what is live versus a prototype, honest limits. Optional. |
| `references/corrections.template.md` | A blank log for the edits you make to drafts, with an entry format, an example, and an always/never list. Optional. |

Two files are not shipped but are read if you create them:

- `references/profile.md`: a filled-in copy of `profile.template.md`. Keep it private.
- `references/corrections.md`: a filled-in copy of `corrections.template.md`, a running list of edits you make to drafts ("I'd never say X", "always sign off with Y"). Keep it private, and occasionally move the corrections that apply to everyone into `style-guide.md` with the specifics removed.

The guide is written about "the author" (whoever's voice is being matched). Edit, delete, or add to any file as you see fit.

## Install

Copy the whole `human-writing-style` folder (the folder, not just `SKILL.md`) into your agent's skills directory:

| Agent | Directory |
|---|---|
| Claude Code (personal, all projects) | `~/.claude/skills/human-writing-style/` |
| Claude Code (one project) | `<project>/.claude/skills/human-writing-style/` |
| Codex | `~/.codex/skills/human-writing-style/` |
| Other agents | wherever they load `SKILL.md` skills from, often `~/.agents/skills/` |

Or clone it straight into place (this is the easiest way to get updates later with `git pull`):

    git clone https://github.com/vandyand/human-writing-style ~/.claude/skills/human-writing-style

From a zip, Windows (PowerShell):

    Expand-Archive human-writing-style.zip -DestinationPath "$HOME\.claude\skills"

From a zip, macOS / Linux:

    unzip human-writing-style.zip -d ~/.claude/skills

Start a new session so the skill list reloads, then try: "use human-writing-style to rewrite this reply: ..."

For agents with no skill system, paste the body of `SKILL.md` (below the `---` frontmatter) into your system prompt or custom instructions, and attach `references/style-guide.md` if you want the full detail.

## Make it yours

1. Copy `references/profile.template.md` to `references/profile.md` and fill it in.
2. Copy `references/corrections.template.md` to `references/corrections.md` and add an entry each time you fix a draft.
3. Replace the example anecdotes in `references/style-guide.md` with your own as you collect real edits. Your corrections always beat the defaults.
4. If you update the package and send it to someone else, remove your `profile.md` and `corrections.md` first.
