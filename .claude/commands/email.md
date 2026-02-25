---
name: email
description: Draft emails with Gaby's writing style and relevant context
allowed-tools: Read, Write
---

# /email — Email Drafting

## Purpose
Draft emails that sound like Gaby — concise, professional, and contextually informed.

## Workflow

1. Read `memory/USER.md` — writing style preferences
2. Read `context/about-me.md` — relevant context
3. Read `notes/contacts/[recipient].md` if it exists — relationship context
4. Ask Gaby: recipient, purpose, key points to hit, any context I should know
5. Draft the email
6. Present for review — offer to revise or save to `notes/emails/`

## Style Guidelines (defaults — update in USER.md)

- Subject lines: clear and specific, not clever
- Opening: no "I hope this email finds you well"
- Length: as short as possible while covering the ask
- Closing: action-oriented ("Let me know if..." or "Happy to discuss")
- Tone: professional but warm

## Invocation Examples

- `/email` → I'll ask what you need
- `/email to [name] re: [topic]` → I'll draft immediately with context
