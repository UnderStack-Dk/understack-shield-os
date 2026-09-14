# Security and privacy review checklist

Use this lightweight checklist for design proposals and future implementation changes. It guides review; it is not a claim that the system is secure.

## Context and boundaries

- What user problem is solved, and what remains out of scope?
- Which assets, identities, devices, networks, processes or AI contexts are affected?
- Which trust boundaries are crossed or introduced?

## Security

- What could an attacker influence, observe, escalate, persist, or exfiltrate?
- Which controls prevent, detect, contain and recover from misuse?
- What is the safe failure mode?
- Which assumptions need testing or an ADR?

## Privacy and AI

- What data exists, where does it flow, and how long is it retained?
- Is local processing possible? If not, is the destination explicit and revocable?
- Could an agent, prompt or external content gain authority it should not have?
- Is consent meaningful, specific and understandable?

## Evidence and follow-up

- What validation would meaningfully reduce uncertainty?
- What residual risks remain, and who must accept them?
- Which documents, ADRs or issues need updating?
