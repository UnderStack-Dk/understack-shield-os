# Operating model

UnderStack Shield OS uses a **security-led, documentation-first discovery model**. The goal is not ceremony; it is to make irreversible decisions visible early, small enough to review, and grounded in evidence.

## The working loop

| Stage | Purpose | Output |
| --- | --- | --- |
| Frame | Define the user problem and desired outcome. | Issue with scope and non-goals. |
| Discover | Research constraints, alternatives and dependencies. | Short proposal or research note. |
| Challenge | Review security, privacy, misuse and recovery implications. | Threat/privacy impact notes. |
| Decide | Record significant trade-offs before implementation. | ADR or owner decision. |
| Deliver | Make the smallest coherent, reviewable change. | Pull request. |
| Learn | Validate the result and capture follow-ups. | Updated docs, risks or backlog. |

## Ways of working

### 1. Outcome-oriented planning

Issues describe a problem, user outcome, constraints, and evidence of completion—not a vague implementation task. A proposed solution remains a hypothesis until reviewed.

### 2. Small-batch delivery

One pull request should express one coherent decision or change. Large proposals are split by trust boundary or decision point, not merely by file count.

### 3. Security and privacy by design

Every proposal identifies affected assets, data flow, trust boundary, potential misuse, and the safe failure mode. “No impact identified” is acceptable only when briefly justified.

### 4. Decision hygiene

Use an ADR when a choice is costly to reverse or changes security, privacy, compatibility, user control, or long-term maintenance. ADRs record alternatives, not just the winner.

### 5. Owner-led governance, contributor-led evidence

Contributors bring research, alternatives and reviewable proposals. The owner retains the final decision and merge authority for `main`. Roles and code ownership will be assigned only after real collaborators and responsibilities are confirmed.

## Cadence without bureaucracy

- **Discovery review:** inspect new proposals, risks and open questions.
- **Decision review:** accept, defer, or reject high-impact ADRs.
- **Repository health review:** keep documentation, labels, board and workflow accurate.

Cadence and meeting schedules are intentionally not prescribed yet; the team should add them when the actual working rhythm is known.
