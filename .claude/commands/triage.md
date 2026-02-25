---
name: triage
description: Triage incoming items — tasks, messages, emails — and route them appropriately
allowed-tools: Read, Edit, Write
---

# /triage — Inbox Triage

## Purpose
Process a batch of incoming items (tasks, messages, emails, notes Gaby pastes in) and route each one: add to task list, log to notes, flag for response, or discard.

## Workflow

1. Gaby pastes in items to triage (emails, Slack messages, meeting notes, brain dump, etc.)
2. For each item, determine:
   - **Action required?** → Add to `my-tasks.yaml`
   - **Information to retain?** → Log to appropriate `notes/` file
   - **Decision made?** → Log to `notes/decisions/`
   - **No action needed?** → Confirm and discard
3. Show a triage summary before writing anything
4. Ask for confirmation, then write all at once

## Triage Categories

- **Task** → `my-tasks.yaml` (with priority and area)
- **Meeting note** → `notes/meetings/YYYY-MM/DD.md`
- **Contact update** → `notes/contacts/[name].md`
- **Decision** → `notes/decisions/YYYY-MM-DD-[slug].md`
- **Project update** → `notes/projects/[project].md`
- **Discard** → No action

## Output Format

```
TRIAGE SUMMARY — [Date]

[Item 1 summary] → Task (high, Academic) — "Do X by Friday"
[Item 2 summary] → Contact note — update Jane Doe's file
[Item 3 summary] → Discard — no action needed

Ready to write? (confirm to proceed)
```
