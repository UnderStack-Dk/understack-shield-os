# Privacy model

## Default posture

Shield OS is designed around local-first processing. No mandatory telemetry is part of the product direction. Any future networked service, diagnostics export, model download, or remote AI interaction must be explicit, granular, revocable, and documented before implementation.

## Data principles

- Collect only data needed for a user-visible capability.
- Process locally where practical.
- Keep sensitive events and forensic material protected at rest.
- Make access, retention and export choices visible to the user.
- Separate data across Security Spaces where the architecture supports it.
- Do not use security events for advertising, profiling, or sale of data.

## AI and Pocket integration

Local AI is the intended default direction. A future remote model or Pocket connection must pass through the Agent Firewall, honor user-defined permissions, and make its data scope and destination clear. Prompt content is untrusted input; it must not silently authorize tool actions or data access.

## Open design questions

Retention periods, backup architecture, account model, update metadata, and optional crash reporting are explicitly deferred to ADRs and a data-flow review.
