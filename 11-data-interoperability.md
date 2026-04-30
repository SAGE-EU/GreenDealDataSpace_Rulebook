# Data Interoperability

## Data Models

In the GDDS, data models are the foundation for semantic interoperability, ensuring that shared data is interpreted consistently by all participants. A data model provides the semantic “dictionary” for a data product or service, defining data elements, their relationships, and their meaning.

Using shared or compatible data models allows data providers and consumers to “speak the same language” when exchanging information. This is essential for avoiding misunderstandings, enabling automated processing, and ensuring that data from multiple sources can be combined meaningfully.

The GDDS will encourage reusing existing semantic standards where possible, extending them when needed, and creating new models only as a last resort. All models should be published in a common **Vocabulary Service**, making them discoverable and accessible within the GDDS, and ideally across other data spaces, using standardised formats and metadata.

**Design Considerations**

  - > **Balance between uniformity and flexibility**: Uniform models help ensure data consistency, but flexibility is needed to accommodate sector-specific needs.

  - > **Federated discoverability**: Participants should be able to find and evaluate models from other domains or data spaces.

  - > **Lifecycle governance**: Models evolve; governance must ensure they remain relevant, accurate, and aligned with broader standards.

**Core Capabilities**

1.  > **Model** **Development** – Reuse or create models to meet GDDS needs, aligning with recognised standards.

2.  > **Model Governance** – Define processes, roles, and tools for maintaining models over time.

3.  > **Model Integration** – Ensure every GDDS data offering is linked to an agreed data model.

4.  > **Abstraction Management** – Support different representation levels (vocabulary, ontology, application profile, schema) and smooth transitions to technical exchange formats.

5.  > **Cross-Data Space Interoperability** – Enable standardised discovery and reuse of models from other data spaces.

*Further content will be added after co-creation sessions.*

## Data Exchange

The Data Exchange building block defines how data is actually transmitted between GDDS participants, ensuring technical interoperability, reliability, and alignment with the Trust Framework, Access & Usage Policies, and agreed Data Models.

It covers the Data Plane (the actual transmission) and its integration with the Control Plane (identification, authorisation, policy enforcement, and transaction state management).

Data exchange in GDDS may take many forms, from dataset downloads to continuous streaming, algorithm-to-data execution, or triggered updates. Whatever the mode, the process should be secure, standardised, and discoverable.

### **Design Principles**

  - > Protocol Flexibility, with Preferred Set – Support multiple industry-standard protocols while defining a recommended set for quick and interoperable onboarding.

  - > Linkage to Semantics – All data exchanged must reference the agreed semantic models for clarity and interoperability.

  - > Federation-Readiness – Protocols should support exchange both inside GDDS and across other data spaces.

  - > Quality of Service – Ensure reliability, error handling, and completeness of data transfers.

### **Core Capabilities**

1.  > Protocol Definition & Publication – Agree on allowed protocols (generic and domain-specific) and publish them in the GDDS service catalogue.

2.  > Transmission Methods – Support push, pull, and streaming modes for finite and continuous datasets.

3.  > Querying & Retrieval – Enable querying of complex datasets, geoquerying, historical data retrieval, and triggered updates.

4.  > Federation Interoperability – Maintain an inventory of accepted protocols and versions for cross-data-space exchange.

5.  > Version & Change Management – Track versions of protocols to maintain backward compatibility when needed.

*Further content will be added after co-creation sessions.*

## Provenance & Traceability

The Provenance & Traceability building block ensures that all relevant metadata and logs, from data origin to usage, are recorded, auditable, and shareable under agreed governance rules.

It supports compliance with regulations (e.g., AI Act, GDPR, sectoral laws), contractual obligations, and business agreements, while also building trust among participants.

Two main aspects are addressed:

  - > **Provenance (Backward-looking)** – Evidence of data origin, ownership, custody, and processing history.

  - > **Traceability (Forward-looking)** – Evidence of how shared data has been used, transformed, or combined after delivery.

Observability, which is the monitoring of Control Plane activities (e.g., contract negotiation, publication/discovery), is part of this block and complements provenance and traceability for compliance and operational transparency.

### **Design Principles**

  - > **Compliance-Driven** – Requirements stem from legal, contractual, and business rules.

  - > **Standards-Based** – Reuse existing models (e.g., W3C PROV-O, PAV) with domain-specific extensions.

  - > **Decentralised Where Possible** – Avoid single points of control; enable participant-managed and federated observability services.

  - > **Trust Management** – Ensure that any 3rd-party observers are themselves trusted and bound by agreed policies.

  - > **Value-Oriented** – Treat provenance data as a data product, enabling value creation beyond compliance.

### **Core Capabilities**

1.  > **Requirements Identification** – Map regulatory, contractual, and business drivers for provenance and traceability.

2.  > **Data Modelling** – Define and publish data models for provenance and traceability; link to domain ontologies.

3.  > **Storage & Processing** – Decide on decentralised vs. centralised storage and processing; set retention policies.

4.  > **Access & Usage Control** – Apply identity and policy enforcement to provenance datasets.

5.  > **Observability Services** – Define scope, granularity, and format of monitored activities; protect observability data.

6.  > **Audit & Certification** – Enable verifiable records for compliance audits and certifications.

*Further content will be added after co-creation sessions.*
