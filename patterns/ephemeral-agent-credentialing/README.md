# Ephemeral Agent Credentialing

This directory contains the **Ephemeral Agent Credentialing** security pattern for AI agents.

- **Latest version (Technical):** [v1.4 Technical Edition](./versions/v1.4-technical.md)
- **Latest version (Executive Brief):** [v1.4 Executive Edition](./versions/v1.4.md)
- **Previous versions:** [v1.3](./versions/v1.3.md) | [v1.2](./versions/v1.2.md) | [v1.1](./versions/v1.1.md) | [v1.0](./versions/v1.0.md)

## What this pattern is about

Ephemeral AI agents often live for minutes, but many teams still grant them credentials that live for **15–60 minutes or longer**, creating a credential exposure window that's **10–50× larger than the task itself**. This pattern proposes **per-agent unique identity** and **task-scoped, short-lived credentials** that expire with the task, plus revocation, immutable audit logging, and delegation chain verification for multi-agent workflows.

## Status

- v1.4 Technical Edition: **Production-Ready** — Full implementation spec for security architects, platform engineers, and identity teams. Companion to the Executive Edition.
- v1.4 Executive Edition: **Production-Ready** — Decision-maker brief for CISOs, CIOs, CFOs, Boards, and Risk Committees. Companion to the Technical Edition.
- v1.3: Retired — Added Component 8 (Operational Observability), Privacy by Design, Secure Credential Injection, Attest & Proxy model, token renewal, semantic scopes, tamper-evident hash chaining, heartbeat monitoring, OWASP NHI Top 10 alignment.
- v1.2: Retired — Delegation chain verification, MCP CIMD, LangGrinch case study, commercial solutions landscape.
- v1.1: Retired — Threat model, "secret zero"/attestation, failure modes, adoption path.
- v1.0: Retired — Initial pattern release.

## How to use

1. Start with **v1.4 Technical Edition** for implementation guidance, or **v1.4 Executive Edition** for a decision-maker brief.
2. If you adopt incrementally, use the **Adoption Path** section as your rollout plan.
3. Pair with guardrails and runtime controls for defense in depth (prompt injection, sandboxing, etc.).

## Pattern Metadata

**Author:** [Devon Artis](https://www.linkedin.com/in/tdevonartis/)
**Reviewer:** _Seeking community review_
**License:** CC BY-SA 4.0

## Feedback

Open an issue using the templates in `.github/ISSUE_TEMPLATE/`.
