---
name: prep
description: Meeting prep — research attendees, pull context, generate talking points
allowed-tools: Read, Write, WebSearch
---

# /prep — Meeting Prep

## Purpose
Get Gaby ready for a meeting with relevant context, talking points, and any open items to address.

## Workflow

1. Ask: who is the meeting with? What's the purpose?
2. Read `notes/contacts/[name].md` for each attendee if files exist
3. Read relevant `notes/projects/` or `notes/decisions/` files
4. Check `my-tasks.yaml` for any open items related to this meeting or person
5. (Optional) Web search for attendee or company context if needed
6. Generate briefing

## Output Format

```
MEETING PREP — [Meeting Name] — [Date/Time]

ATTENDEES
  [Name] — [Role, relationship, last interaction]

CONTEXT
  [Relevant project/relationship background]

OPEN ITEMS TO ADDRESS
  [Any tasks or decisions pending with these people]

TALKING POINTS
  1. [Key point]
  2. [Key point]
  3. [Key point]

GOAL FOR THIS MEETING
  [What does Gaby want to walk away with?]
```

## After the Meeting
Run `/triage` with meeting notes to capture action items.
