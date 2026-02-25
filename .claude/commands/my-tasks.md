---
name: my-tasks
description: View and manage all open tasks across Academic, Professional, and Personal areas
allowed-tools: Read, Edit, Write
---

# /my-tasks — Task Management

## Purpose
Give Gaby a clear view of all open tasks across all areas. Capture new tasks instantly. Help prioritize against goals.

## Workflow

1. Read `my-tasks.yaml` — load all open tasks
2. Read `goals.yaml` — understand current priorities for context
3. Read `memory/MEMORY.md` — apply any task management preferences

### Display tasks:
- Group by: **Priority** (high → medium → low), then by Area
- Show due dates if present
- Flag anything overdue or due within 48 hours
- Keep it scannable — no walls of text

### Capture new tasks:
If Gaby mentions a new task (or one comes up in conversation):
1. Confirm: "Should I add '[task]' to my-tasks.yaml?"
2. Ask: priority? area? due date?
3. Append to `my-tasks.yaml` immediately
4. Confirm: "Added."

### Task operations:
- "done [task]" → move task to `completed[]` in my-tasks.yaml with today's date
- "prioritize [task]" → update priority field
- "add [task]" → capture new task
- "focus" → surface only high-priority items
- "academic" / "work" / "personal" → filter by area

## Output Format

```
TASKS — [Day, Date]

HIGH PRIORITY
  [ ] Task name (Area) — due: date if applicable
  [ ] Task name (Area)

MEDIUM PRIORITY
  [ ] Task name (Area)

LOW PRIORITY
  [ ] Task name (Area)

OVERDUE: [flag any overdue items here]
```

Keep it under 25 lines. If there are many tasks, summarize by area counts and show high priority only, with option to expand.
