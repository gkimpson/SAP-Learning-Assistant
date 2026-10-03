# SAP Learning Assist

A study coach for SAP security certification. It quizzes you, explains concepts, builds flashcards and study plans, and tracks your weak spots. It covers C_SEC, ADM940, ADM945 and SAP Access Control 12.0 Emergency Access Management.

All the study notes are bundled inside the skill, so there is nothing else to download.

## What you need

- [Claude Code](https://claude.com/claude-code) installed and signed in
- Git (to clone the repo)

## Install

Pick **one** of the two options. Option A is the easiest.

### Option A: use it inside this repo (easiest)

1. Clone the repo and open it in Claude Code.

   ```
   git clone <repo-url>
   cd <repo-folder>
   claude
   ```

2. That's it. Claude Code picks up the skill from `.claude/skills/sap-learning-assist/` automatically.

The skill only works while you are in this repo folder.

### Option B: install it for every project

Copy the **whole** `sap-learning-assist` folder (including `references/`) into your personal skills folder.

**Mac or Linux**

```
mkdir -p ~/.claude/skills
cp -R .claude/skills/sap-learning-assist ~/.claude/skills/
```

**Windows (PowerShell)**

```
New-Item -ItemType Directory -Force "$env:USERPROFILE\.claude\skills"
Copy-Item -Recurse .claude\skills\sap-learning-assist "$env:USERPROFILE\.claude\skills\"
```

Restart Claude Code after copying.

## Check it works

Start Claude Code and type `/sap-learning-assist`. It should appear in the list. If it doesn't, see Troubleshooting below.

## How to use it

Type `/sap-learning-assist` followed by what you want. Some examples:

| Say this | You get |
|---|---|
| `quiz me on emergency access management` | One question at a time, marked as you go |
| `quiz me on PFCG roles, 10 questions` | A timed-style set on a chosen topic |
| `scenario drill on firefighter logs` | A short hands-on task to talk through |
| `flashcards on HANA security` | 10 Q and A cards |
| `explain derived roles` | A short explanation plus a check question |
| `cheat sheet for Fiori authorisations` | A one-page summary |
| `study plan, exam in 6 weeks, 5 hours a week` | A week-by-week plan |
| `mock test` | 20 mixed questions with a score by topic |

Answer in the chat. The coach tells you if you're right, why, and where in the notes to look.

## Your progress

The skill saves your scores and weak topics to `progress.md` in the skill folder. Next session it suggests your weakest topic first. This file is gitignored, so each person keeps their own and nobody overwrites anyone else's.

## What's inside

```
sap-learning-assist/
  SKILL.md        the instructions Claude follows
  README.md       this file
  references/     17 study notes (about 1.9 MB)
  progress.md     created on first use, not committed
```

## Update to the latest version

Option A: run `git pull`.

Option B: pull the repo, then copy the folder over your installed copy again. Your `progress.md` is kept unless you delete the old folder first, so copy the new files over the top rather than removing it.

## Troubleshooting

- **The command doesn't show up.** Restart Claude Code. For Option A, make sure you started it from inside the repo folder. For Option B, check the folder is at `~/.claude/skills/sap-learning-assist/SKILL.md`.
- **It says it can't find a note.** The `references/` folder must sit next to `SKILL.md`. Copy the whole folder, not just `SKILL.md`.
- **A very long answer or a slow reply on S/4HANA topics.** Reference 15 is 1.6 MB, so the coach searches it rather than reading it all. Ask a narrower question.

## Good to know

- The sample questions in the notes come from third-party prep sites and are treated as unverified. The coach writes its own practice questions and checks them against the notes.
- Always confirm exam details (format, pass mark, price, renewal) on the official SAP certification page. The notes contain a few conflicting figures and the coach will flag them.
