# Triii

Triii is a personal operating system for building, thinking, and shipping projects using AI agents and persistent state.

It is **not** a product, app, or company (yet).
It is an internal system designed to:
- externalize thinking
- reduce context loss
- turn ideas into shipped work
- compound learning over time

Triii treats AI as a **volatile collaborator** and files + git as the **source of truth**.

---

## Core Philosophy

### 1. Context is volatile
AI sessions rot over time. Bad turns accumulate. Memory pollutes.

Triii assumes this is inevitable.

Instead of trying to preserve long chat histories, Triii:
- treats conversations as disposable
- deliberately rotates context
- persists only what matters to files

### 2. Progress must be written
If it is not written to disk, it does not exist.

Triii persists:
- decisions
- plans
- guardrails
- progress
- lessons learned

State lives in:
- markdown files
- git history
- (eventually) databases

### 3. Two modes of work

**Mode A — Interactive / Exploration**
Used when:
- deciding what to build
- making product or taste decisions
- exploring ideas

Output:
- specs
- plans
- checklists
- written decisions

**Mode B — Implementation / Loop (Ralph-style)**
Used when:
- success criteria are clear
- "done" is machine-verifiable

Truth comes from:
- tests
- types
- lint
- explicit checklists

Context is disposable. State is external.

---

## What Triii Is Used For

- Managing multiple long-term projects without losing focus
- Running daily and weekly planning loops
- Capturing and structuring ideas from the internet
- Turning AI from a chat partner into an execution engine
- Learning by building ahead of current capability
- Preventing repeated mistakes through explicit guardrails

Triii supports:
- solo work
- agent-driven development
- exploration without emotional attachment
- shipping without burnout

---

## Repository Structure

```
triii/
├── agents.md          # Global operating rules for AI agents
├── README.md          # This file
├── canon/             # Stable truths (principles, voice contracts)
│   ├── principles.md
│   ├── voice_prestige.md
│   └── voice_songbird.md
├── vaults/            # Idea vault + swipe vault
│   ├── ideas.md
│   └── swipe.md
├── ralph/             # Loop state, guardrails, logs
│   ├── ralph_task.md
│   ├── guardrails.md
│   ├── progress.md
│   ├── errors.log
│   └── activity.log
├── runs/              # Daily and weekly execution plans
│   ├── daily.md
│   └── weekly.md
└── templates/         # Reusable templates
```

Each folder has a specific role.
Nothing is accidental.

---

## Guardrails Over Memory

Triii does not rely on "remembering everything".

Instead:
- mistakes are recorded once
- prevention rules are added
- future agents read guardrails before acting

Failures evaporate.
Lessons accumulate.

---

## Design Goals

- Simple over clever
- Files over prompts
- Checklists over vibes
- Shipping over perfection
- Play over pressure

Triii is meant to be used daily, lightly, and continuously.

---

## Status

Triii is a living system.
It will evolve as tools, models, and workflows change.

The goal is not to build the perfect system —
the goal is to **build momentum that compounds**.

