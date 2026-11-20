---
name: fml-operator
description: Coordinate FML and VOIDCORE work through the canonical Git repository. Use when planning, implementing, troubleshooting, reviewing, or handing off any FML project. Prevent repeated context transfer, duplicate architecture work, and unverified completion claims.
---

# FML Operator

## Mandatory startup
Read the repository's `AGENTS.md`, `state/SYSTEM_STATE.yaml`, `state/PROJECT_STATE.yaml`, `operations/TASKS.yaml`, and relevant entries in `operations/DECISIONS.md`.

Treat repository state as the shared source of truth, not the latest chat transcript.

## Execution loop
1. **Orient:** identify active project, state, current blocker, and last verified artifact.
2. **Select:** choose one existing unblocked task. Respect priority and capacity lock.
3. **Plan:** define the smallest concrete change and measurable acceptance criteria.
4. **Execute:** modify the real artifact or run the actual workflow; do not substitute advice for execution.
5. **Verify:** run tests, inspect outputs, and independently validate deliverables where appropriate.
6. **Record:** update task state, evidence, changed files, and technical log.
7. **Handoff:** leave a concise machine-readable status so another agent can continue without the operator copying a conversation.

## Non-negotiable rules
- No redesigning settled architecture without contradictory evidence.
- No parallel expansion of unrelated projects.
- No claim of success without an artifact and verification.
- No repeated requests for facts already recorded.
- No secrets, private media, unreleased material, or personal data in public repositories.
- Distinguish what the current agent can actually access from what another agent or machine might access.
- If an integration is not configured, mark it NOT_CONNECTED; never imply that repository presence equals live synchronization.
- Ask the operator only for a decision, permission, credential, or physical action that cannot be safely inferred or performed.

## Output contract
Every completed task records:
- task ID and objective
- files/artifacts changed
- commands and test results
- verification status
- remaining blocker
- next executable action

Use the task states defined in `AGENTS.md`.
