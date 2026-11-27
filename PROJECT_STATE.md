# Project state

Last updated: 2026-11-27
Authority: project owner
Document status: working draft; proposed governance rules await owner acceptance.
Confidence convention: VERIFIED / REPORTED / INFERRED / NOT VERIFIED

## Project-level structure

- **Shared control repository:** `V0ff/sls-project-control`, public, default branch `main`. **VERIFIED** through GitHub repository metadata.
- **Technical source repository:** `V0ff/sls-core`, private. **VERIFIED** through GitHub repository metadata.
- **Separation:** public control repository is not a mirror of the private technical repository. **ACCEPTED** as the project boundary on 2026-11-27.
- **Rool integration permission:** GitHub App installation access includes both repositories. **VERIFIED** by the installation repository listing on 2026-11-27. This confirms integration-level repository selection only; it does not prove that a Rool runtime or external process can read this repository.
- **Rool runtime read access:** **NOT VERIFIED**. Requires a direct read test from Rool's own runtime.
- **Technical project state:** current active specifications, implementation state, test results and deployment state have not been independently re-verified in this repository. **NOT VERIFIED** here.

## Governance adoption

- **D-001:** public control / private technical source separation — accepted.
- **D-002:** canonical project-level reference — proposed, pending owner acceptance.
- **D-003:** owner-controlled authorization gates — proposed, pending owner acceptance.
- **D-004:** bounded review and evidence discipline — proposed, pending owner acceptance.
- The initial control documents have not yet been accepted as a complete governance model.
- The queue order and task priorities have not been approved by the owner.

## Current work status

- **SLS-001:** REVIEW — initial control repository and documents await owner acceptance; Rool runtime access remains unverified.
- **SLS-002:** PROPOSED — read-only S2 inventory only.
- **SLS-003:** PROPOSED — read-only modular architecture inventory; independent of SLS-002 unless the owner later defines a dependency.
- **Active technical tasks:** none.
- **Technical implementation/test/deployment authorization:** none granted by creation or correction of this control repository.

## Evidence and authority rules proposed for adoption

For every material claim, retain source, date, exact object identity and verification method where applicable. Distinguish a reported claim from an independently verified fact. A task's status does not by itself prove that its deliverable exists, that its evidence is verified, that the owner accepted it, or that a subsequent gate is authorized.

## Immediate next step

Owner review of the consolidated control-document correction branch. After the owner accepts the governance model and chooses the work order, Rool may perform a narrowly scoped read-access check. Only then should the owner activate one inventory task at a time.

## Known limitations

- Public visibility is intentional for the control documents only. Review every proposed commit for accidental disclosure.
- GitHub integration access does not imply Rool's local runtime has network access or that a private repository is readable anonymously.
- No current technical claim should be treated as verified solely because it appears in an earlier conversation summary.
