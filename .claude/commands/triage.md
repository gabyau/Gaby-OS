---
name: triage
description: Triage inbox and incoming items — pull MIT Outlook email, route tasks, log notes
allowed-tools: Read, Edit, Write, mcp__ms365__*
---

# /triage — Inbox Triage

## Purpose
Process incoming items — pull Gaby's MIT Outlook inbox via the ms365 MCP and/or triage items she pastes in. Route each one: add to task list, log to notes, flag for response, or discard.

## Workflow

1. **Pull inbox** (unless Gaby pastes items directly):
   - Use ms365 MCP → `list-mail-messages` on Inbox, unread or last 24–48 hrs
   - Focus on unread emails first
2. For each item, determine:
   - **Action required?** → Add to `my-tasks.yaml`
   - **Response needed?** → Flag with draft or note to use `/email`
   - **Information to retain?** → Log to appropriate `notes/` file
   - **Decision made?** → Log to `notes/decisions/`
   - **No action needed?** → Confirm and discard
3. Show a triage summary before writing anything
4. Ask for confirmation, then write all at once

## Triage Categories

- **Task** → `my-tasks.yaml` (with priority and area)
- **Response needed** → Flag: "Draft reply with /email — [subject]"
- **Meeting note** → `notes/meetings/YYYY-MM/DD.md`
- **Contact update** → `notes/contacts/[name].md`
- **Decision** → `notes/decisions/YYYY-MM-DD-[slug].md`
- **Project update** → `notes/projects/[project].md`
- **Discard** → No action

## Output Format

```
TRIAGE — [Date] ([N] items)

[Sender / Item] — [Subject/summary] → Task (high, Academic) — "Do X by Friday"
[Sender / Item] — [Subject/summary] → Reply needed — draft with /email
[Sender / Item] — [Subject/summary] → Contact note — update Jane Doe's file
[Sender / Item] — [Subject/summary] → Discard

Ready to write? (confirm to proceed)
```

## Invocation
- `/triage` → Pull Outlook inbox automatically via ms365 MCP
- `/triage` + pasted text → Triage whatever Gaby pastes in (no inbox pull)
