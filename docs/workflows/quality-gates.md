# Quality gates

Quality gates protect the project’s standards while keeping early work lightweight. They are proportional to impact.

## Ready to start

A proposal is ready when it has:

- A clearly stated problem, intended outcome and non-goals.
- A defined trust boundary or a reason that none changes.
- Privacy and security considerations.
- Alternatives or an explanation of why discovery is still needed.
- An owner decision path for consequential choices.

## Ready to review

A pull request is ready when it is narrow in scope and includes:

- Linked context (issue, proposal, or ADR) where relevant.
- Updated documentation, diagrams or decision records.
- Explicit impact notes for security and privacy.
- Evidence of the applicable checks.
- No credentials, personal data, opaque binaries, or unapproved product code.

## Ready to merge

| Gate | Current expectation |
| --- | --- |
| Documentation check | Passing required check. |
| Review | At least one approval under branch protection. |
| Discussion | All review conversations resolved. |
| Decision | Owner accepts material security/privacy/architecture decisions. |
| Scope | Change matches the approved intent and current pre-development boundary. |

## Definition of done for this phase

The work is complete when a future contributor can understand the decision, its context, its trade-offs, and its next validation step without relying on private chat history.
