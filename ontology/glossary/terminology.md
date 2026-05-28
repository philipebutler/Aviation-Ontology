# Glossary

Use this glossary to define commonly used terms and prevent semantic drift.

## Canonical concept

An enterprise-level concept intended to serve as a stable semantic anchor across domains, tools, and historical contexts.

## Local definition

A tool-specific, department-specific, program-specific, or process-specific meaning of a concept.

## Historical definition

A meaning that was valid during a past period but may not match current enterprise usage.

## Source of authority

The system, artifact, organization, or process that is treated as authoritative for a concept or relationship.

## Semantic owner

The person or organization responsible for the meaning, governance, and evolution of a semantic definition.

## System of record

The operational system that officially stores or manages instances of a concept.

## Product structure

The managed arrangement of product elements, usually represented through assemblies, parts, configurations, and relationships. Product structure is often a reflection of an implicit organizational ontology, not the full ontology itself.

## ISO 10303 / STEP

The ISO standard family for computer-interpretable product data representation and exchange, including integrated resources and domain application protocols.

## Application Protocol (AP)

A domain-specific implementation profile in STEP, such as AP203, AP214, AP233, AP239, or AP242, that constrains and applies integrated resources for practical interoperability.

## AP203

Configuration-controlled 3D design exchange protocol in ISO 10303 focused on mechanical design representation and management.

## AP214

Core data protocol in ISO 10303 for automotive mechanical design processes, including product data exchange across design and manufacturing toolchains.

## AP233

Systems engineering data exchange protocol in ISO 10303 for requirements, functional, and architectural model interoperability.

## AP239

Product lifecycle support protocol in ISO 10303 used for lifecycle traceability, support analysis, and in-service data interoperability.

## AP242

Managed model-based 3D engineering protocol in ISO 10303 that supports geometry, product manufacturing information (PMI), and configuration-aware digital thread exchange.

## Product (STEP)

In ISO 10303, a stable product identity concept that is separated from versioned formations and contextual technical definitions.

## Variant

A governed alternative of a Product, aligned to STEP AP242 configuration-management patterns that distinguish approved product alternatives and may carry variant-specific version lineages.

## Product definition formation

A STEP concept used to represent controlled revision/version progression of a product identity.

## Product definition

A STEP concept that captures contextual technical meaning of a product version, often bound to design, manufacturing, or support contexts.

## Product Definition Context

A STEP context construct paired with product_definition to declare the discipline or lifecycle viewpoint (for example, design, manufacturing, or support) in which a definition is valid.

## EXPRESS schema

The formal ISO 10303 data-model definition written in the EXPRESS language, where entities, attributes, and constraints are specified for interoperable product data.

## product (EXPRESS entity)

The ISO 10303 identity entity for an item, typically carrying identifiers and descriptive metadata independent of versioned formations and contextual definitions.

## product_definition_formation (EXPRESS entity)

The ISO 10303 entity representing a specific formation/version of a product identity, commonly used for revision-controlled progression.

## product_definition_formation_with_specified_source (EXPRESS entity)

An ISO 10303 specialization of product_definition_formation that adds a source classification (for example, made, bought, or not known).

## product_definition (EXPRESS entity)

The ISO 10303 entity that captures the governed technical definition of a product formation within a declared context.

## product_definition_context (EXPRESS entity)

The ISO 10303 context entity defining the application discipline and lifecycle viewpoint attached to a product_definition.

## Next assembly usage occurrence

A STEP concept representing a specific parent-child usage link in product structure, commonly used for assembly/BOM semantics.

## Product definition shape

A STEP construct linking product definition semantics to representational shape information.

## Shape representation

A STEP representation construct for geometric/topological/presentation form, including use in AP242 model-based definition exchange.

## Advanced B-Rep Shape Representation

A STEP geometric representation subtype used to encode boundary-representation solids and topology for high-fidelity product model exchange.
