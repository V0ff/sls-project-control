# Project decisions and proposals

Accepted decisions are durable. Proposed rules remain proposals until the project owner explicitly accepts them. Superseded entries remain in the record with an explicit supersession note.

## D-001 — Separate public project control from private technical source

- **Date:** 2026-11-27
- **Status:** ACCEPTED
- **Decision:** Use `V0ff/sls-project-control` as the public shared control point. Keep `V0ff/sls-core` private.
- **Rationale:** Rool needs a common reference point for project priorities and mandates but cannot read the private source repository. Public control files must not become a route for publishing private technical material.
- **Consequences:** Store only approved project-level priorities, decisions, task mandates and sanitized status. Share any necessary private technical input through a separately approved, bounded channel.

## D-002 — Canonical source of project-level status

- **Date proposed:** 2026-11-27
- **Status:** PROPOSED — owner decision required
- **Proposal:** `PROJECT_STATE.md`, `PRIORITIES.md`, `DECISIONS.md` and individual task files become the canonical project-level reference. A GitHub Project board, if used, is a presentation/workflow view only.
- **Rationale:** Avoid conflicting status across chat threads, boards and generated reports.
- **Owner decision:** Pending.

## D-003 — Owner-controlled authorization gates

- **Date proposed:** 2026-11-27
- **Status:** PROPOSED — owner decision required
- **Proposal:** Agents may inspect and propose. The project owner approves scope, priority, activation, implementation, tests and deployment separately. No agent writes directly to `main`; writes to a working branch require task-specific authorization.
- **Rationale:** Prevent recursive review and autonomous scope expansion from becoming de facto authorization.
- **Owner decision:** Pending.

## D-004 — Bounded review and evidence discipline

- **Date proposed:** 2026-11-27
- **Status:** PROPOSED — owner decision required
- **Proposal:** Every task must be bounded by explicit scope, exclusions, inputs, deliverable and acceptance criteria. Evidence must be labeled VERIFIED, REPORTED, INFERRED or NOT VERIFIED. Review work must conclude with a disposition rather than automatically spawning another review cycle. Task status, evidence status, deliverable status and owner acceptance remain distinct.
- **Rationale:** Keep review proportional to concrete risk and prevent review loops.
- **Owner decision:** Pending.
