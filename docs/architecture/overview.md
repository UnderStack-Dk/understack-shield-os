# Architecture overview

This is a conceptual model, not an implementation specification. Technology choices remain subject to ADRs and threat-model review.

```mermaid
flowchart TB
  U[User] --> UX[UnderStack experience]
  UX --> SC[Shield Core]
  SC --> PE[Policy engine]
  SC --> RE[Risk and event engine]
  RE --> FT[Forensic timeline]
  PE --> AG[App Guard / sandbox boundary]
  PE --> NG[Network Guard]
  PE --> DG[Device Guard]
  PE --> AF[Agent Firewall]
  AF --> AI[Local AI / Pocket integration]
  AG --> SS[Security Spaces]
  PE --> LK[Lockdown]
  SC --> LB[Immutable / atomic Linux base]
  LB --> BI[Boot integrity + full-disk encryption]
```

## Design layers

| Layer | Intended responsibility |
| --- | --- |
| Immutable base | Minimize drift, support atomic update and recovery concepts. |
| Shield Core | Coordinate events, policy, risk signals and explanations. |
| Guards | Mediate app, network, device and agent trust-boundary crossings. |
| Security Spaces | Separate sensitive contexts and reduce blast radius. |
| User experience | Present choices, consent, containment and forensic information clearly. |

## Linux security direction

The project will evaluate eBPF for observability, LSM/SELinux for mandatory access control, and sandboxing mechanisms for workload isolation. These are candidate mechanisms, not present commitments to a particular implementation.
