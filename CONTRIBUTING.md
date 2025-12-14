# Contributing

Thank you for your interest in contributing to AI Security Blueprints! This guide will help you contribute effectively.

---

## Table of Contents
- [Ways to Contribute](#ways-to-contribute)
- [Proposing a New Pattern](#proposing-a-new-pattern)
- [Improving Existing Patterns](#improving-existing-patterns)
- [Reviewing Patterns](#reviewing-patterns)
- [Pattern Template](#pattern-template)
- [Editorial Guidelines](#editorial-guidelines)
- [Versioning](#versioning)

---

## Ways to Contribute

You can contribute by:

1. **Proposing new patterns** - Share security patterns you've developed or discovered
2. **Improving existing patterns** - Suggest enhancements, corrections, or clarifications
3. **Reviewing patterns** - Provide technical review and validation
4. **Sharing implementation experiences** - Document how you've applied patterns
5. **Reporting issues** - Identify errors, gaps, or areas for improvement

---

## Proposing a New Pattern

### Step 1: Open a Pattern Request Issue

1. Use the [New Pattern Request](.github/ISSUE_TEMPLATE/pattern_request.md) template
2. Describe the security problem and why it matters
3. Outline the proposed solution approach

### Step 2: Create the Pattern Document

1. Fork the repository
2. Create a new directory: `patterns/<pattern-name>/`
3. Use the [Pattern Template](#pattern-template) below
4. Write version `v1.0.md` in the `versions/` subdirectory
5. Create a `README.md` for the pattern overview

### Step 3: Submit Pull Request

1. Create a feature branch: `git checkout -b pattern/<pattern-name>`
2. Include:
   - Pattern document with complete frontmatter
   - Pattern README.md
   - Update to repository CHANGELOG.md
   - Update to main README.md pattern catalog
3. Submit PR with description of what the pattern addresses

---

## Improving Existing Patterns

### For Minor Improvements

1. Open an issue describing the improvement
2. Fork the repo and create a feature branch
3. Make changes to the pattern file
4. Update the `Version History` section
5. Submit a PR

### For Substantive Changes

1. Discuss the change in an issue first
2. Create a new version file (e.g., `v1.2.md`)
3. Update pattern frontmatter (version, last_updated)
4. Document changes in `Version History` section
5. Update pattern README.md to point to new version
6. Update CHANGELOG.md

---

## Reviewing Patterns

We welcome technical reviews from security practitioners, researchers, and engineers.

### How to Become a Reviewer

1. **Comment on a pattern issue or PR** with your technical feedback
2. **Focus on:**
   - Technical accuracy
   - Threat model completeness
   - Implementation feasibility
   - Missing edge cases or failure modes
   - Real-world applicability

### Review Checklist

When reviewing a pattern, consider:

- [ ] **Problem statement** is clear and addresses a real security concern
- [ ] **Threat model** explicitly states what is and isn't defended against
- [ ] **Solution** is implementable with existing technologies
- [ ] **Trade-offs** are honestly documented
- [ ] **Failure modes** are addressed
- [ ] **References** are accurate and accessible
- [ ] **Implementation guidance** is actionable
- [ ] **Frontmatter metadata** is complete and accurate

### Getting Credit as a Reviewer

Once your review is accepted, the pattern author will:
1. Update the pattern's frontmatter `reviewer` field with your name and link
2. Acknowledge your contribution in the version history

---

## Pattern Template

Use this template when creating a new pattern:

```markdown
---
pattern_name: "Your Pattern Name"
category: "Category (e.g., IAM for AI Systems, Data Security, etc.)"
status: "Draft"
version: "1.0"
last_updated: "YYYY-MM-DD"
author: "Your Name"
author_link: "https://linkedin.com/in/yourprofile or personal website"
reviewer: "Seeking community review"
license: "CC BY-SA 4.0"
---

# Pattern Name

**Pattern Name:** Your Pattern Name
**Category:** Category Name
**Status:** Draft
**Version:** 1.0
**Last Updated:** YYYY-MM-DD

---

## Table of Contents
- [Context](#context)
- [Problem](#problem)
- [Solution](#solution)
- [Threat Model](#threat-model)
- [Component Details](#component-details)
- [Benefits](#benefits)
- [Trade-Offs and Limitations](#trade-offs-and-limitations)
- [Implementation Considerations](#implementation-considerations)
- [When to Use This Pattern](#when-to-use-this-pattern)
- [Related Patterns](#related-patterns)
- [References](#references)
- [Version History](#version-history)

---

## Context

Describe the environment and conditions where this pattern applies.

---

## Problem

### Problem Statement
What security challenge does this pattern address?

### Current Inadequate Approaches
What existing solutions fall short, and why?

---

## Solution

### Architectural Principles
Key design principles that guide this pattern.

### Core Components
Main building blocks of the solution.

---

## Threat Model

### Adversaries We Defend Against
Be specific about threat actors and attack scenarios.

### Explicit Non-Goals
What this pattern does NOT address (equally important).

---

## Component Details

Detailed implementation guidance for each component.

---

## Benefits

### Security Benefits
What security improvements does this provide?

### Compliance Benefits
How does this help with regulatory compliance?

---

## Trade-Offs and Limitations

Be honest about:
- Performance impacts
- Complexity costs
- Operational overhead
- What problems this does NOT solve

---

## Implementation Considerations

Practical guidance for implementation:
- Technology options
- Deployment patterns
- Common pitfalls

---

## When to Use This Pattern

### Use This Pattern When:
✅ Clear criteria for when this pattern is appropriate

### Do NOT Use This Pattern When:
❌ Clear criteria for when this pattern is inappropriate

---

## Related Patterns

Patterns this complements, replaces, or relates to.

---

## References

Industry standards, research papers, and related work that informed this pattern.

---

## Pattern Metadata

**Author:** [Your Name](your-link)
**Reviewer:** _Seeking community review_
**License:** CC BY-SA 4.0

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | YYYY-MM-DD | Initial pattern release |

---

**END OF SECURITY PATTERN**
```

---

## Editorial Guidelines

### Writing Style

- **Clear over clever** - Prefer straightforward language
- **Implementable over theoretical** - Provide actionable guidance
- **Honest about limitations** - Don't oversell the pattern
- **Explicit about assumptions** - State your threat model clearly

### Required Sections

Every pattern must include:
- Clear problem statement
- Explicit threat model (including non-goals)
- Implementation guidance
- Trade-offs and limitations
- When to use (and when NOT to use)
- References

### Frontmatter Requirements

All patterns must include YAML frontmatter with:
- `pattern_name` - Full pattern name
- `category` - Pattern category
- `status` - Draft | Under Review | Stable | Deprecated
- `version` - Semantic version
- `last_updated` - Date in YYYY-MM-DD format
- `author` - Author name
- `author_link` - LinkedIn or personal website
- `reviewer` - Reviewer name and link, or "Seeking community review"
- `license` - License (default: CC BY-SA 4.0)

---

## Versioning

We use semantic versioning for patterns:

- **Patch (1.0 → 1.0.1)**: Typo fixes, clarifications, minor updates
- **Minor (1.0 → 1.1)**: New sections, expanded guidance, backward-compatible improvements
- **Major (1.0 → 2.0)**: Fundamental changes to recommendations, breaking changes

### Version File Management

- Each version gets its own file: `versions/v1.0.md`, `versions/v1.1.md`, etc.
- Keep all versions for historical reference
- Update pattern README.md to point to latest version
- Document changes in Version History table

---

## Questions?

- Open a [discussion](../../issues) for questions
- Use [issue templates](.github/ISSUE_TEMPLATE/) for specific proposals
- Check existing patterns for examples

Thank you for contributing to making AI systems more secure!
