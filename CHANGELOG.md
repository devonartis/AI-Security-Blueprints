# Changelog

All notable changes to this repository will be documented in this file.

## Unreleased

- Added Ephemeral Agent Credentialing v1.3 (latest)
  - New Component 8: Operational Observability (RFC 7807 errors, KPIs, why-denied tracing)
  - Architectural principles: Privacy by Design, Secure Credential Injection
  - Attest & Proxy issuance model, session resumption/crash recovery, one-time launch token bootstrap
  - Token renewal for long-running agents, semantic scopes (ABAC), token bloat management
  - Clock skew tolerance, high-assurance introspection for critical agents
  - Tamper-evident hash chaining, data sanitization, log aggregation for high-volume reads
  - Secure discovery binding, heartbeat and liveness monitoring
  - OWASP NHI Top 10 (2025) standards alignment
- Archived Ephemeral Agent Credentialing v1.2
- Added Ephemeral Agent Credentialing v1.2
  - Component 7: Delegation Chain Verification for multi-agent authorization chains
  - MCP CIMD as alternative bootstrap/attestation approach alongside SPIFFE
  - CVE-2025-68664 (LangGrinch) case study demonstrating pattern value
  - Commercial solutions landscape (Okta/Auth0, Microsoft Entra Agent ID, CyberArk, HashiCorp Vault 1.21)
  - Updated standards references: OWASP Agentic Top 10 (2026), NIST IR 8596, IETF WIMSE
  - Open source AI agent identity projects (AIM, kagent)
  - Enhanced threat model addressing delegation exploitation
  - 6-phase adoption path (expanded from 5 phases)
- Archived Ephemeral Agent Credentialing v1.1
- Repository renamed from "Security-Patterns" to "AI-Security-Blueprints" to better reflect broader scope
- Enhanced README.md with blueprint catalog structure for patterns, topologies, guides, and educational resources
- Comprehensive CONTRIBUTING.md with pattern template, review process, and frontmatter requirements
- Added PATTERN_TEMPLATE.md for new contributions
- Added author and reviewer metadata to all patterns
- Updated pattern status from "Production-Ready" to "Under Review" to reflect community review process
- Initial repo scaffolding and import of the Ephemeral Agent Credentialing pattern (v1.0, v1.1)

## 2025-11-26

- Added Ephemeral Agent Credentialing v1.1 (latest).
- Archived Ephemeral Agent Credentialing v1.0.
