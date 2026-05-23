# Repository Instructions

## 1. Start with the semantic question

Before adding a file, ask:

- What concept are we trying to define?
- Why does it matter operationally?
- Who owns the meaning?
- Where is the authoritative source?
- Does this concept have different meanings in legacy systems?
- What relationships make the concept useful?

## 2. Prefer small definitions

Avoid large, abstract definitions at first. A useful definition should be narrow enough that engineers can review it and broad enough that it can act as a semantic anchor.

## 3. Preserve legacy semantics

Do not overwrite historical meanings. Capture them under `historical_definitions` or `local_definitions`.

Example:

```yaml
local_definitions:
  - context: Legacy PLM
    definition: How the concept was used in the legacy system.
    source: Legacy training guide or SME interview.
```

## 4. Separate canonical meaning from local meaning

A canonical definition should explain the enterprise-level concept. Local definitions should explain tool-specific, program-specific, or historical meanings.

## 5. Use relationships to create reasoning value

A definition without relationships is mostly a glossary entry. A definition with relationships becomes part of a reasoning graph.

Useful early relationships include:

- satisfies
- allocated_to
- realizes
- verifies
- affects
- owns
- approves
- supersedes
- derived_from

## 6. Add examples and anti-examples

Examples help people understand what belongs in the concept. Anti-examples prevent semantic drift.

## 7. Use pull requests for governance

Every change should be reviewed for semantic clarity, ownership, source of authority, and consistency with existing definitions.

## 8. Do not force one meaning too early

If a term means different things in CAD, PLM, ERP, manufacturing, or certification, capture those meanings explicitly. The goal is governed semantic clarity, not premature normalization.

## 9. Keep the repo tool-independent

The content should be portable to SysML, PLM, graph databases, AI systems, or future ontology tooling.

## 10. Recommended first working session

In the first working session, try to define only these concepts:

- Requirement
- Function
- System
- Part
- Change
- VerificationArtifact

Then define only these relationships:

- satisfies
- allocated_to
- realizes
- verifies
- affects

This small set is enough to begin building a useful digital-thread semantic backbone.
