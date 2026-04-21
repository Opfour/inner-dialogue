# Inner Dialogue -- Portable AI Therapist Toolkit

A private, persistent AI therapist that lives on your computer. Sessions stay local, AI remembers everything. Works with Claude, GPT, or any AI.

## What It Is

An open-source framework (not an app) -- a collection of markdown files that give any AI therapeutic capabilities with persistent memory.

## Key Files

- `manifest.json` -- Package manifest
- `safety-protocol.md` -- Crisis protocols (always loaded first)
- `profile.template.md` -- Client profile template
- `CLAUDE.template.md` -- Template CLAUDE.md for therapeutic sessions
- `commands.md` -- User commands for customization
- `personas/` -- Therapist personality definitions
- `modalities/` -- Therapeutic approaches (CBT, ACT, DBT, IFS, etc.)
- `structures/` -- Session structure definitions
- `docs/` -- Documentation and getting started guide

## Features

- Evidence-based: CBT, ACT, DBT, and more built in
- Portable across AI platforms
- Optional password protection
- Customizable therapist persona and communication style

## Related

- `~/Sage/` -- David's personal therapeutic support instance using this framework


## Git Recon (run before reading code)

```bash
# Churn hotspots
git log --format=format: --name-only --since="1 year ago" | sort | uniq -c | sort -nr | head -20
# Bus factor
git shortlog -sn --no-merges
# Bug clusters
git log -i -E --grep="fix|bug|broken" --name-only --format= | sort | uniq -c | sort -nr | head -20
# Activity timeline
git log --format='%ad' --date=format:'%Y-%m' | sort | uniq -c
# Crisis patterns
git log --oneline --since="1 year ago" | grep -iE 'revert|hotfix|emergency|rollback'
```
