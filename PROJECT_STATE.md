# Project state

Last updated: 2026-11-27
Authority: project owner
Document status: current project-level control record; technical project state remains subject to task-scoped verification.
Confidence convention: VERIFIED / REPORTED / INFERRED / NOT VERIFIED

## Project-level structure

- **Shared control repository:** `V0ff/sls-project-control`, public, default branch `main`. **VERIFIED** through GitHub repository metadata.
- **Technical source repository:** `V0ff/sls-core`, private. **VERIFIED** through GitHub repository metadata.
- **Separation:** public control repository is not a mirror of the private technical repository. **ACCEPTED** as the project boundary on 2026-11-27.
- **Rool integration permission:** GitHub App installation access includes both repositories. **VERIFIED** by the installation repository listing on 2026-11-27. This confirms integration-level repository selection only; it does not prove that a Rool runtime or external process can read this repository.
- **Rool runtime read access:** **NOT VERIFIED**. Requires a direct read test from Rool's own runtime.
- **Technical project state:** current active specifications, implementation state, test results and deployment state have not been independently re-verified in this repository. **NOT VERIFIED** here.

## Governance adoption

- **D-001:** public control / private technical source separation — ACCEPTED.
- **D-002:** canonical project-level reference — ACCEPTED by owner on 2026-11-27.
- **D-003:** owner-controlled authorization gates — ACCEPTED by owner on 2026-11-27.
- **D-004:** bounded review and evidence discipline — ACCEPTED by owner on 2026-11-27.
- The four decisions above establish the adopted project-control rules. Individual task deliverables still require owner acceptance.
- **Priority sequence:** SLS-001 → SLS-002 → SLS-003, approved as the current planning order on 2026-11-27. This does not activate any task.

## Current work status

- **SLS-001:** REVIEW — initial control repository and documents await final task acceptance; Rool runtime access remains unverified.
- **SLS-002:** PROPOSED — read-only S2 inventory only.
- **SLS-003:** PROPOSED — read-only modular architecture inventory.
- **Active tasks:** none.
- **Technical implementation/test/deployment authorization:** none granted.

## Evidence and authority rules

For every material claim, retain source, date, exact object identity and verification method where applicable. Distinguish a reported claim from an independently verified fact. A task's status does not by itself prove that its deliverable exists, that its evidence is verified, that the owner accepted it, or that a subsequent gate is authorized.

## Immediate next step

Complete SLS-001's remaining read-access verification from Rool's own runtime. After that evidence is recorded, the owner can accept SLS-001 and separately activate SLS-002. SLS-003 remains later in the recommended sequence and requires its own activation.

## Known limitations

- Public visibility is intentional for the control documents only. Review every proposed commit for accidental disclosure.
- GitHub integration access does not imply Rool's local runtime has network access or that a private repository is readable anonymously.
- No current technical claim should be treated as verified solely because it appears in an earlier conversation summary.
