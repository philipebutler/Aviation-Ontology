This repository is a lightweight, Git-based starting point for capturing an enterprise ontology for product engineering, program execution, business processes, certification artifacts, and legacy semantic context.

The intent is not to create a perfect ontology on day one. The intent is to make implicit engineering meaning explicit, reviewable, version-controlled, and reusable by humans, tools, and AI systems.

## Why this repository exists

Many engineering organizations already have a rich implicit ontology embedded in:

- product structures
- PLM/CAD objects
- requirements documents
- change workflows
- certification artifacts
- naming conventions
- organizational roles
- tribal knowledge
- historical process behavior

This repository provides a simple structure for documenting those concepts in a durable, machine-readable way.

## Guiding principles

1. Start small.
2. Capture operational meaning before formal theory.
3. Treat semantics as configuration-managed assets.
4. Preserve legacy meanings instead of overwriting them.
5. Separate canonical definitions from local or historical definitions.
6. Prefer explicit relationships over prose-only definitions.
7. Keep the content portable and tool-independent.
8. Use Git review workflows for semantic governance.

## Repository structure

```text
ontology/
âââ entities/
â   âââ requirement.yaml
â   âââ function.yaml
â   âââ system.yaml
â   âââ part.yaml
â   âââ change.yaml
â   âââ verification.yaml
â
âââ relationships/
â   âââ satisfies.yaml
â   âââ allocated_to.yaml
â   âââ realizes.yaml
â   âââ verifies.yaml
â
âââ lifecycle/
â   âââ states.yaml
â   âââ workflows.yaml
â
âââ glossary/
â   âââ terminology.md
â
âââ examples/
```

## Recommended starting scope

Begin with a small semantic backbone:

- Organization and ownership
- Program and project context
- Requirements
- Functions
- Logical systems
- Physical parts or assemblies
- Change objects
- Verification and certification evidence

Avoid trying to model the entire enterprise at first.

## How to add a new entity definition

1. Copy `ontology/entities/_entity-template.yaml`.
2. Rename it using lowercase kebab-case, for example `interface-control-document.yaml`.
3. Fill in the canonical definition.
4. Add local or historical definitions where the concept has changed over time.
5. Define attributes, relationships, lifecycle states, owners, source systems, and examples.
6. Submit changes through a pull request.

## How to add a new relationship definition

1. Copy `ontology/relationships/_relationship-template.yaml`.
2. Rename it using a verb phrase, for example `is-certified-by.yaml`.
3. Define the source entity, target entity, meaning, cardinality, and constraints.
4. Include examples and anti-examples.
5. Submit changes through a pull request.

## Review checklist

Before approving a semantic definition, reviewers should ask:

- Is the definition clear and non-circular?
- Is the owning organization identified?
- Is the source of authority identified?
- Are local or historical meanings preserved?
- Are relationships explicit?
- Are lifecycle states defined or referenced?
- Are examples included?
- Are ambiguous terms linked to the glossary?
- Is this concept truly canonical, or is it domain-specific?
- Could an AI or downstream system use this definition without relying on tribal knowledge?

## Semantic modeling pattern

Use this basic pattern:

```text
Canonical Concept
  + Local Definitions
  + Historical Definitions
  + Attributes
  + Relationships
  + Lifecycle Semantics
  + Authority / Source of Truth
  + Examples
```

The goal is not to eliminate semantic diversity. The goal is to make semantic diversity explicit, governed, and computable.

## Suggested Git workflow

- `main`: approved semantic baseline
- `develop`: integration branch for work in progress
- feature branches: individual semantic proposals

Example branch names:

```text
feature/add-verification-artifact
feature/refine-part-definition
feature/add-legacy-change-semantics
```

Use pull requests to review semantic changes just as you would review source code.

## Suggested future extensions

This repository can later be connected to:

- SysML / KerML models
- PLM object models
- requirements tools
- graph databases
- BPMN process models
- knowledge graphs
- AI agents
- certification evidence repositories

Do not start by integrating everything. Start by making the core semantics clear.