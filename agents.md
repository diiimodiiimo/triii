# triii — Agent Operating Manual (agents.md)

Triii is a personal operating system for shipping projects using AI agents + persistent state.
Core idea: context is volatile; progress must live in files + git.

## Modes
### Mode A: Interactive (thinking/exploration)
Use when: deciding what to build, taste, strategy, product direction.
Output: specs, checklists, decisions, plans.

### Mode B: Loop/Implementation (Ralph-style)
Use when: specs are crisp and "done" is machine-verifiable.
Truth: tests, types, lint. State: files + git. Context: disposable.

## Global rules
- Always propose a plan before making changes.
- Prefer small, reversible commits.
- If stuck or looping: STOP, write what happened to `ralph/errors.log`, add a prevention rule to `ralph/guardrails.md`, then restart fresh.
- Never write secrets into the repo. Use environment variables.
- Every feature should have:
  - success criteria (checkboxes)
  - verification step (test/lint/typecheck/manual)

## Git rules
- Small commits. Message prefixes: feat:, fix:, refactor:, chore:, docs:
- If a change affects logic, add/adjust tests or add a verification step.
- Before finalizing: run the verify command if one exists.

## Triii output files
- `runs/daily.md`: daily top-3 tasks + quick plan
- `runs/weekly.md`: weekly plan + project priorities
- `vaults/ideas.md`: idea vault (structured cards)
- `vaults/swipe.md`: swipe vault (references + why they're good)
- `canon/voice_prestige.md`: Prestige.os voice contract
- `canon/voice_songbird.md`: SongBird voice contract
- `canon/principles.md`: your operating principles
- `ralph/*`: loop state hygiene and guardrails

## Default tech stack (when building apps)
- Next.js, Vercel
- DB: Supabase (Postgres)
- Auth: Clerk
- Payments: Stripe
- Styling: Tailwind
- Email: Resend

