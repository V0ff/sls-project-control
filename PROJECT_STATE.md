# Project state

Last updated: 2026-11-27
Authority: project owner
Confidence convention: VERIFIED / REPORTED / INFERRED / NOT VERIFIED

## Project-level structure

- **Shared control repository:** `V0ff/sls-project-control`, public, default branch `main`. **VERIFIED** through GitHub repository metadata.
- **Technical source repository:** `V0ff/sls-core`, private. **VERIFIED** through GitHub repository metadata.
- **Separation:** public control repository is not a mirror of the private technical repository. **DECIDED** as the operating boundary for this control setup.
- **Rool access:** GitHub App installation access now includes both repositories. **VERIFIED** by the installation repository listing on 2026-11-27. This confirms repository-level integration access, not that every Rool runtime or external process can read it.
- **Technical project state:** current active specifications, implementation state, test results and deployment state have not been independently re-verified in this repository. **NOT VERIFIED** here.

## Current operating constraints

1. This repository is the canonical shared reference for priorities, decisions, task mandates and project-level status.
2. `sls-core` remains private; do not expose its contents through this repository.
3. No technical implementation or test execution is authorized by the creation of this repository.
4. Project owner approval is required before a proposal becomes an active task or an implementation/test/deployment gate is opened.
5. Evidence must retain its source, date, exact object identity and verification status where applicable.

## Immediate next step

Owner review of this repository's initial control documents. After acceptance, create or activate narrowly scoped read-only inventory tasks for the S2 material and modular architecture work. Those inventories must establish exact active file paths, revisions, hashes and statuses from the source environment before drawing conclusions.

## Known limitations

- Public visibility is intentional for the control documents only. Review every proposed commit for accidental disclosure.
- GitHub integration access does not imply Rool's local runtime has network access or that a private repository is readable anonymously.
- No current technical claim should be treated as verified solely because it appears in an earlier conversation summary.
