# Zero-Trust Validation Pipeline

**Pattern:** Ephemeral Agent Credentialing v1.3
**Back to:** [Pattern Document](../versions/v1.3.md#component-3-zero-trust-enforcement)

---

The complete validation decision tree executed by resource servers on every request. Every check must pass or access is denied and logged with a why-denied reason.

**Validation layers:**
- **Transport** — mTLS certificate validation
- **Token** — JWT signature, expiration, and scope matching
- **Revocation** — Standard (cached) or High-Assurance (online introspection) based on resource sensitivity
- **Delegation** — Chain signature verification, scope attenuation, and per-agent revocation check

**Color key:** Green = Access Granted, Red = Access Denied, Amber = Audit Log

![Zero-Trust Validation](03-zero-trust-validation.png)
