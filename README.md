# SLS — Project Control

This repository is intended to become the shared control point for project priorities, decisions, task mandates and verified project-level status.

It is deliberately separate from `sls-core`, which remains private. This repository must not contain source code, raw product or price data, credentials, personal data, private infrastructure details, internal file paths, or material whose publication has not been explicitly approved.

## Current adoption status

- **D-001 — public control / private technical source separation:** accepted as the project boundary.
- **D-002 through D-004 — operating and governance rules:** proposals pending explicit project-owner acceptance.
- Until the owner accepts the proposed governance model, these documents are a working draft, not proof that every listed rule has been adopted.
- This repository is the proposed canonical reference for project-level state. The GitHub Project board, if used, is intended as a presentation/workflow view only.

## Proposed operating model

- The project owner is the sole authority for scope, priority, acceptance and permission to implement.
- ChatGPT provides analysis, structured options, reviews and draft changes.
- Rool provides technical inspection, evidence and execution within an explicitly approved task.
- Neither assistant may silently expand scope, promote a proposal to an approved decision, or treat an unverified claim as a fact.

## Proposed workflow rules

1. Read the current state, priorities, decisions and relevant task file before acting.
2. Every task must state its scope, exclusions, required inputs, deliverable and acceptance criteria.
3. Distinguish **VERIFIED**, **REPORTED**, **INFERRED** and **NOT VERIFIED** evidence.
4. Preserve predecessor documents and decision history. Record changes; do not silently rewrite history.
5. Do not create a new review or correction plan merely in response to another review or correction plan.
6. A review cycle must end in a concrete disposition: accept, reject, defer, or identify a specific blocking evidence gap.
7. Implementation, test execution, deployment and modification of project data require separate, explicit owner approval for the relevant task and gate.
8. Keep no more than two tasks in `ACTIVE` status at once.

## Proposed task statuses

- `PROPOSED` — suggested, not approved to start.
- `READY` — scope and inputs are clear; awaiting activation.
- `ACTIVE` — explicitly authorized and in progress.
- `BLOCKED` — a specific dependency or evidence gap prevents progress.
- `REVIEW` — deliverable exists and awaits owner acceptance.
- `DONE` — acceptance criteria met and accepted by the owner.
- `PARKED` — intentionally paused.
- `REJECTED` — explicitly declined.

A status change must be reflected in the task file and `PROJECT_STATE.md` / `PRIORITIES.md` as applicable. Task status, evidence status, deliverable status and owner acceptance are separate facts and must not be conflated.

## Files

- `PROJECT_STATE.md` — concise current state and evidence confidence.
- `PRIORITIES.md` — proposed work queue; order remains unapproved until the owner sets it.
- `DECISIONS.md` — durable project-level decisions and pending proposals.
- `WORK_LOG.md` — append-only summary of material work and changes.
- `work/` — task mandates and deliverables.

## Proposed change and permission protocol

- Read access is permitted where repository access allows it.
- Agents may prepare proposed changes as diffs or replacement text in the conversation.
- No agent may write directly to `main`.
- Creating commits on a named working branch requires explicit owner authorization identifying the task or correction scope and the permitted files.
- The project owner alone approves merges to `main` and changes to priorities, decisions, task scope, task activation and acceptance.
- Technical evidence may be added only within an `ACTIVE` task mandate and only when that task includes explicit permission to write the relevant evidence artifact.
- Changes to `sls-core`, test execution, implementation and deployment each require separate, explicit authorization. Authorization for this public control repository does not imply authorization for technical work.
- Never publish private technical material here merely to make it accessible to another tool.
