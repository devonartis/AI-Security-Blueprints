# AI Security Blueprints

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

A curated collection of **security patterns, architectures, and topologies** for AI and ML systems—practical, implementation-oriented guidance designed to help teams build secure, resilient AI applications.

## About This Repository

As AI systems become increasingly autonomous and widespread, traditional security approaches often fall short. This repository provides practical security blueprints specifically designed for:

- **Autonomous AI agents** that make decisions and take actions
- **Multi-agent systems** requiring secure coordination
- **LLM-powered applications** with unique threat models
- **Hybrid AI/traditional architectures** with complex security boundaries
- **ML pipelines and training infrastructure** requiring protection

This repository includes:
- **Security Patterns** - Reusable solutions to common AI security problems
- **Secure Topologies** - Reference architectures for AI system deployment
- **Implementation Guides** - Step-by-step guidance for securing AI systems
- **Educational Resources** - Learning materials for AI security practitioners

---

## Blueprint Catalog

### Security Patterns

| Pattern | Category | Version | Last Updated | Description |
|---------|----------|---------|--------------|-------------|
| [Ephemeral Agent Credentialing](./patterns/ephemeral-agent-credentialing/) | IAM for AI Systems | v1.4 | 2026-04-23 | Secure authentication and authorization for short-lived AI agents using unique identities, task-scoped credentials, delegation chain verification, and operational observability. Technical Edition + Executive Edition. |

### Secure Topologies

_Coming soon - Reference architectures for deploying AI systems securely_

### Implementation Guides

_Coming soon - Step-by-step guides for implementing AI security controls_

### Educational Resources

_Coming soon - Learning materials and documentation for AI security practitioners_

> [!NOTE]
> Blueprints in this repository are **under active development** and community review. They represent emerging practices rather than established standards. Review carefully and adapt to your specific context.

---

## Quick Start

### Browse Blueprints

Navigate to `patterns/<pattern-name>/` to explore security patterns. Each pattern directory contains:

- **README.md** - Overview and latest version link
- **versions/** - All pattern versions with change history
- Pattern document with:
  - Problem statement and context
  - Detailed solution architecture
  - Implementation guidance
  - Threat model and limitations
  - References and related work

### Contribute

We welcome contributions from security practitioners, researchers, and engineers!

**Ways to contribute:**
- 📝 [Propose a new pattern](CONTRIBUTING.md#proposing-a-new-pattern) using the [pattern template](PATTERN_TEMPLATE.md)
- ✏️ [Improve existing patterns](CONTRIBUTING.md#improving-existing-patterns)
- 🔍 [Review patterns](CONTRIBUTING.md#reviewing-patterns) and provide technical feedback
- 🐛 Report issues or suggest improvements

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines, including:
- Pattern template with required frontmatter
- Review process and checklist
- Versioning conventions
- How to get credit as a reviewer

### Use a Blueprint

1. **Read the blueprint** - Understand the problem, solution, and tradeoffs
2. **Review the threat model** - Ensure it matches your security requirements
3. **Check the implementation guide** - Assess feasibility for your stack
4. **Adapt to your context** - Blueprints are templates, not rigid rules
5. **Share feedback** - Open an issue with your experience

---

## What Makes a Good Security Blueprint?

Blueprints in this repository follow these principles:

- **Implementation-oriented** - Actionable guidance, not just theory
- **Explicit about tradeoffs** - Clear about what is and isn't addressed
- **Threat-model driven** - Specific about attacks defended against
- **Production-informed** - Based on real-world experience and proven technologies
- **Versioned and evolving** - Updated as practices mature

---

## Repository Structure

```
AI-Security-Blueprints/
├── patterns/
│   └── <pattern-name>/
│       ├── README.md              # Pattern overview
│       └── versions/
│           ├── v1.0.md           # Initial release
│           ├── v1.1.md           # Threat model, bootstrap problem
│           ├── v1.2.md           # Delegation chains, CIMD, LangGrinch
│           ├── v1.3.md           # Previous version (retired)
│           ├── v1.4-technical.md # Latest — Technical Edition
│           └── v1.4.md           # Latest — Executive Edition
├── .github/
│   └── ISSUE_TEMPLATE/           # Issue templates
├── CONTRIBUTING.md               # Contribution guidelines
├── PATTERN_TEMPLATE.md           # Template for new patterns
├── CHANGELOG.md                  # Repository change log
├── LICENSE                       # CC BY-SA 4.0
├── SECURITY.md                   # Security policy
└── README.md                     # This file
```

---

## Conventions

- **Pattern filenames** are versioned (e.g., `v1.1.md`)
- **Changes** are made via pull requests
- **Version history** is maintained within each pattern
- **CHANGELOG.md** tracks repository-level changes

---

## Blueprint Development Stages

Blueprints in this repository may be at different maturity levels:

- **Draft** - Initial proposal, seeking feedback
- **Under Review** - Community review in progress
- **Stable** - Reviewed and validated, recommended for adoption
- **Deprecated** - Superseded by newer approaches

> [!IMPORTANT]
> Blueprint maturity indicates community review status, not production readiness for your specific use case. Always perform your own security assessment.

---

## Related Resources

- [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [OWASP Top 10 for Agentic Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework)
- [NIST IR 8596 - Cyber AI Profile](https://www.nist.gov/publications)
- [Cloud Security Alliance - AI Security](https://cloudsecurityalliance.org/research/topics/ai-security)
- [SPIFFE/SPIRE Documentation](https://spiffe.io/)
- [IETF WIMSE Working Group](https://datatracker.ietf.org/wg/wimse/about/)

---

## License

Unless otherwise stated, all patterns are licensed under [**CC BY-SA 4.0**](LICENSE).

You are free to:
- **Share** - Copy and redistribute the material
- **Adapt** - Remix, transform, and build upon the material

Under the following terms:
- **Attribution** - Give appropriate credit
- **ShareAlike** - Distribute contributions under the same license

---

## Feedback and Contact

- **Issues**: Use [GitHub Issues](.github/ISSUE_TEMPLATE/) for bugs, questions, or pattern proposals
- **Discussions**: Share implementation experiences and ask questions
- **Security**: Report security concerns via [SECURITY.md](SECURITY.md)

---

**Built by the community, for the community.**
Help us make AI systems more secure. [Contribute today](CONTRIBUTING.md).
