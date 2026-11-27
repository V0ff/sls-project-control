# Work queue and priority order

Last updated: 2026-11-27

The order below is the recommended execution sequence, approved by the project owner as the current planning order. It does not itself activate any task or grant permission to access private technical sources, edit files, run tests, implement changes or deploy.

## Active work

None.

## Recommended sequence

| Order | Task | Status | Purpose | Rationale / gate |
|---:|---|---|---|---|
| 1 | [SLS-001 — Establish project control point](work/SLS-001.md) | REVIEW | Close acceptance of the control repository and verify Rool's read access from its own runtime. | Finish the shared operating foundation first. Do not mark complete until the Rool runtime read test is directly evidenced and the owner accepts the control deliverable. |
| 2 | [SLS-002 — Read-only S2 status inventory](work/SLS-002.md) | PROPOSED | Establish exact current S2 source objects and their verified status without editing or testing. | Establish a bounded, evidence-based S2 baseline before moving to adjacent architecture work. Requires explicit owner activation and an approved route to the necessary source material. |
| 3 | [SLS-003 — Read-only modular architecture inventory](work/SLS-003.md) | PROPOSED | Establish exact current architecture documents, decisions and implementation status without expanding scope. | Run after the S2 inventory so the architecture inventory can distinguish S2 facts from broader architectural status. This is a recommended sequence, not an asserted technical dependency. Requires separate owner activation. |

## Queue rules

- Only the project owner changes the approved order or activates tasks.
- Maximum two `ACTIVE` tasks; default to one until parallel work is demonstrably useful.
- A blocked task must name the exact blocker, evidence needed and who can resolve it.
- Do not add a task merely to re-review an existing review. First determine whether it contains a new, concrete decision or evidence gap.
- A task is `DONE` only after the owner accepts its deliverable.
- Priority and dependency are separate attributes. A dependency must be stated and evidenced; it must not be inferred from row order.
- Priority order is planning guidance only. It is not authorization to begin a task.
