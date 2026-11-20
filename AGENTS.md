# FML Agent Contract

Before any work:
1. Read `README.md`, `state/SYSTEM_STATE.yaml`, `state/PROJECT_STATE.yaml`, `operations/TASKS.yaml`, and relevant decision records.
2. Do not ask the operator to repeat information already present in repository state.
3. Identify the single highest-priority unblocked task. Do not invent a new project.
4. State the intended artifact, acceptance criteria, and risk before modifying files.
5. Check repository status and existing work before editing.

During work:
- Make the smallest useful change that advances the active task.
- Preserve existing architecture and decisions unless evidence disproves them.
- Separate FACT, INFERENCE, ASSUMPTION, and UNKNOWN.
- Never overwrite source assets or production deliverables without explicit authorization.
- Never expose secrets or private assets in public repositories.

Before completion:
- Run relevant tests or validation.
- Record exact commands, results, changed files, and commit SHA where available.
- Update task status and technical log.
- If blocked, record the blocker and the exact missing dependency; do not generate another strategy document.

Task states: PROPOSED, SPECIFIED, BUILDING, TESTING, VERIFIED, DEPLOYED, PARKED.
A task is not VERIFIED merely because code was written.
