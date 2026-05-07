# Attest & Proxy Issuance Model

**Pattern:** Ephemeral Agent Credentialing v1.3 (NEW)
**Back to:** [Pattern Document](../versions/v1.3.md#the-attest--proxy-issuance-model-new-in-v13)

---

The v1.3 issuance model separates attestation from credential signing to prevent private key sprawl. Only the Central Authority holds signing keys.

**Key steps:**
1. **Secure Bootstrap** — Orchestrator injects a one-time launch token via platform-native mechanisms (K8s projected SA, tmpfs, Nitro Enclaves). Environment variables must NOT be used.
2. **Attest & Sign** — Sidecar generates an ephemeral key pair locally, sends attestation evidence + public key to Central Authority, which validates and signs.
3. **Credential Delivery** — Sidecar provides signed SVID + JWT to the agent process. Private key never leaves the sidecar.
4. **Operate** — Agent uses credentials for authenticated resource access.
5. **Crash Recovery** — On restart, full re-attestation with a new instance ID. Old credentials are implicitly revoked.

![Attest & Proxy Model](05-attest-and-proxy.png)
