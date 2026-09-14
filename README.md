# UnderStack Shield OS

> A privacy-first, Linux-based security operating-system concept. **Pre-development repository:** it intentionally contains no product code.

UnderStack Shield OS is a future desktop operating-system initiative for people who want local control, clear security boundaries, and security that can explain its decisions. Its design direction is a hardened, immutable/atomic Linux base with privacy and user agency as defaults.

## Status

This repository is the project foundation: product intent, decision records, security and privacy models, and collaboration workflow. It is not a runnable system and does not make implementation commitments.

## Product direction

- Local-first operation; no mandatory telemetry.
- Atomic, recoverable system base and verified boot path.
- Full-disk encryption, boot integrity, and least privilege.
- Shield Core coordinating app, device, network, and AI-facing protections.
- App sandboxing, Security Spaces, Lockdown, and an explainable forensic timeline.
- Defense-in-depth using Linux facilities such as eBPF, LSM and SELinux where appropriate after technical validation.
- Local AI / Pocket integration only under explicit, revocable user control; an Agent Firewall and prompt-injection defenses are core design concerns.

## Documentation map

| Area | Starting point |
| --- | --- |
| Vision and scope | [docs/vision.md](docs/vision.md) |
| Architecture | [docs/architecture/overview.md](docs/architecture/overview.md) |
| Threat model | [docs/security/threat-model.md](docs/security/threat-model.md) |
| Privacy model | [docs/privacy/privacy-model.md](docs/privacy/privacy-model.md) |
| Security principles | [docs/security/principles.md](docs/security/principles.md) |
| Contribution workflow | [CONTRIBUTING.md](CONTRIBUTING.md) |
| Roadmap | [docs/roadmap/roadmap.md](docs/roadmap/roadmap.md) |
| Architectural decisions | [docs/architecture/adr/README.md](docs/architecture/adr/README.md) |

## Repository workflow

`main` is the protected source of truth. `develop` is the integration branch once implementation begins. Work proceeds in short-lived branches and is merged through reviewed pull requests. See [docs/workflows/development-workflow.md](docs/workflows/development-workflow.md).

## Current boundaries

This repository must not contain application, kernel, agent, installer, CI build, telemetry, or deployment code until those proposals are reviewed. Documentation and configuration checks are allowed.

## Governance

The repository owner retains final control over `main`. Maintainers and ownership mappings will be added only after real identities and responsibilities are confirmed.

## Security reporting

Please do not disclose potential vulnerabilities in public issues. Follow [SECURITY.md](SECURITY.md).

## License

No license has been selected yet. Until one is explicitly added, all rights are reserved.
