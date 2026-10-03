# sap-learning-assist

A Claude Code skill that coaches you through SAP security certification (C_SEC, ADM940, ADM945, Access Control 12.0 Emergency Access Management).

## Install

Clone the repo. The skill lives at `.claude/skills/sap-learning-assist/`, so Claude Code picks it up automatically when you open the repo. To use it in every project instead, copy the whole folder to your personal skills folder:

- Mac and Linux: `~/.claude/skills/`
- Windows: `%USERPROFILE%\.claude\skills\`

Copy the whole folder, including `references/`. The skill finds its notes relative to itself, so nothing else needs configuring.

## Use

Run `/sap-learning-assist` and say what you want, for example "quiz me on emergency access management" or "build a study plan, exam in 6 weeks".

## Notes

- `references/` holds the source notes (17 files, about 1.9 MB).
- `progress.md` is created on first use and is gitignored, so everyone tracks their own scores.
- Sample question files are from third party sites and are treated as unverified.
# SAP-Learning-Assistant
