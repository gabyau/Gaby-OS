---
name: gm
description: Morning briefing — today's priorities, tasks, and deadlines
allowed-tools: Read, mcp__ms365__*
---

# /gm — Morning Briefing

## Purpose
Start Gaby's day with clarity. What matters today? What's due? What should she focus on?

## Workflow

1. Read `my-tasks.yaml` — what's open and high priority?
2. Read `goals.yaml` — are today's tasks aligned with goals?
3. Read `context/scheduling-rules.md` — any calendar constraints today?
4. Read `memory/MEMORY.md` — any patterns to apply?
5. Use **ms365 MCP** to pull today's calendar events and next 48 hrs of meetings
6. Check for anything due today or overdue in tasks

## Output Format

```
GM, Gaby — [Day, Date]

TODAY'S FOCUS
  [1-3 most important things to do today, ranked by priority + goals alignment]

OPEN HIGH-PRIORITY TASKS
  [List high-priority tasks from my-tasks.yaml]

OVERDUE / DUE TODAY
  [Anything past due or due today — flagged clearly]

CALENDAR TODAY
  [Today's meetings/events from Outlook, with times]

COMING UP (next 48 hrs)
  [Any meetings worth prepping for]

WORTH NOTING
  [Any goal alignment flags, patterns, or context worth surfacing]
```

Keep it under 25 lines. Actionable, not exhaustive. If everything is fine, say so briefly.
