# SLS — Project Control

This repository is the shared, public control point for project priorities, decisions, task mandates and verified status.

It is deliberately separate from `sls-core`, which remains private. This repository must not contain source code, raw product or price data, credentials, personal data, private infrastructure details, internal file paths, or material whose publication has not been explicitly approved.

## Operating model

- The project owner is the sole authority for scope, priority, acceptance and permission to implement.
- ChatGPT provides analysis, structured options, reviews and draft changes.
- Rool provides technical inspection, evidence and execution within an explicitly approved task.
- Neither assistant may silently expand scope, promote a proposal to an approved decision, or treat an unverified claim as a fact.
- This repository is the canonical shared reference for project-level state. The GitHub Project board, if used, is a view and not an independent source of truth.

## Workflow rules

1. Read the current state, priorities, decisions and relevant task file before acting.
2. Every task must state its scope, exclusions, required inputs, deliverable and acceptance criteria.
3. Distinguish **verified**, **reported**, **inferred** and **not verified** evidence.
4. Preserve predecessor documents and decision history. Record changes; do not silently rewrite history.
5. Do not create a new review or correction plan merely in response to another review or correction plan.
6. A review cycle must end in a concrete disposition: accept, reject, defer, or identify a specific blocking evidence gap.
7. No implementation, test run, deployment or modification of project data without explicit owner approval for that task and gate.
8. Keep no more than two tasks in `ACTIVE` status at once.

## Task statuses

- `PROPOSED` — suggested, not approved to start.
- `READY` — scope and inputs are clear; awaiting activation.
- `ACTIVE` — explicitly authorized and in progress.
- `BLOCKED` — a specific dependency or evidence gap prevents progress.
- `REVIEW` — deliverable exists and awaits owner acceptance.
- `DONE` — acceptance criteria met and accepted by the owner.
- `PARKED` — intentionally paused.
- `REJECTED` — explicitly declined.

A status change must be reflected in the task file and `PROJECT_STATE.md` / `PRIORITIES.md` as applicable.

## Files

- `PROJECT_STATE.md` — concise current state and evidence confidence.
- `PRIORITIES.md` — authoritative ordered work queue.
- `DECISIONS.md` — durable project-level decisions.
- `WORK_LOG.md` — append-only summary of material work and changes.
- `work/` — task mandates and deliverables.

## Change protocol

Propose changes as a concise diff or complete replacement text with rationale. The project owner approves changes to priorities, decisions, task scope and authorization. Technical evidence may be added by an agent only within an active task's mandate. Never publish private technical material here merely to make it accessible to another tool.
