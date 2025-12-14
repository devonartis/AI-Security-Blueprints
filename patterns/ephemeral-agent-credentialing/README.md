# Ephemeral Agent Credentialing

This directory contains the **Ephemeral Agent Credentialing** security pattern for AI agents.

- **Latest version:** [v1.1](./versions/v1.1.md)
- **Previous version:** [v1.0](./versions/v1.0.md)

## What this pattern is about

Ephemeral AI agents often live for minutes, but many teams still grant them credentials that live for **15–60 minutes or longer**, creating a credential exposure window that’s **10–50× larger than the task itself**. This pattern proposes **per-agent unique identity** and **task-scoped, short-lived credentials** that expire with the task, plus revocation and immutable audit logging.

## Status

- v1.1: **Under Review** — Expanded threat model, "secret zero"/attestation, failure modes, and adoption path. Built on production-proven technologies (SPIFFE/SPIRE).
- v1.0: Initial pattern release.

## How to use

1. Start with **v1.1**.
2. If you adopt incrementally, use the **Adoption Path** section as your rollout plan.
3. Pair with guardrails and runtime controls for defense in depth (prompt injection, sandboxing, etc.).

## Pattern Metadata

**Author:** [Devon Artis](https://www.linkedin.com/in/tdevonartis/)
**Reviewer:** _Seeking community review_
**License:** CC BY-SA 4.0

## Feedback

Open an issue using the templates in `.github/ISSUE_TEMPLATE/`.
