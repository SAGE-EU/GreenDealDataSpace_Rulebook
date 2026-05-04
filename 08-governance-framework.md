# Governance Framework 

The GDDS Governance Framework defines the set of rules, policies, and procedures that guide the functioning of the Green Deal Data Space. It establishes how governance is exercised, how participants interact with the data space, and how trust, compliance, and operational integrity are maintained across the ecosystem.

In the context of a data space, the governance framework defines how roles, responsibilities, and decision-making procedures are structured and how these internal arrangements influence the data space’s interaction with participants and service providers.

The GDDS Governance Framework distinguishes between:

  - > **Internal governance rules**, which regulate relationships and responsibilities within the governance authority and its operational structures.

  - > **External governance policies**, which define how the data space interacts with participants, service providers, and other stakeholders.

Operational agreements such as participation contracts, service agreements, or data-sharing agreements are **not part of the governance framework itself, they are described in the Legal Framework later**.

Within this GDDS Rulebook, the governance framework is structured across three operational governance layers that complement the institutional governance model described earlier:

1.  > **Trust & Participation Governance -** defining how organisations participate in the data space and how trust between participants is ensured.

2.  > **Data Sovereignty & Technical Governance** - defining how data exchange is governed and technically enabled.

3.  > **Certification & Conformity Governance -** defining how compliance with governance rules and standards is monitored and enforced.

These governance layers define how organisations participate in the data space, how data exchange is governed, and how compliance with governance rules is monitored and enforced.

## Participation, Roles & Trust Framework

The Participation & Trust Framework defines how organisations and individuals become participants in the Green Deal Data Space and how their rights, responsibilities, and access privileges are governed throughout the lifecycle of their participation.

Participation in GDDS is open to organisations that commit to the governance framework defined in this Rulebook and comply with the eligibility and trust requirements established by the data space. The framework ensures that all actors operating within GDDS are properly identified, verified, and authorised to perform their roles in a secure, transparent, and accountable manner.

The purpose of the Participation & Trust Framework is to ensure that all actors operating within the data space are properly identified, verified, and authorised to perform their roles in a secure and transparent manner. This framework establishes the conditions under which organisations may join, operate within, and withdraw from the data space.

Participation management therefore includes the following core processes:

1.  > **identification and eligibility assessment of candidate participants**

2.  > **participant onboarding and admission procedures**

3.  > **assignment of roles and access rights**

4.  > **monitoring of participant compliance with governance rules**

5.  > **suspension, revocation, or voluntary withdrawal procedures**

By defining clear participation rules and lifecycle processes, the Participation & Trust Framework ensures that data exchange takes place in a trusted environment where responsibilities, permissions, and accountability are clearly defined.

### GDDS Roles

Participants in the GDDS shall operate under clearly defined roles, which determine their rights and obligations within the data space. These roles are context-dependent, and a single organisation may assume multiple roles depending on the specific data transaction or service.

The primary participant roles within GDDS include:

**Data Providers**  
Organisations that supply data to the data space by publishing datasets or data services that can be accessed by other participants.

**Data Recipients**  
Organisations that consume data from the data space for purposes such as analytics, decision-making, or the development of data-driven services.

**Data Rights Holders**  
Entities that hold legal rights over specific data assets and determine the conditions under which such data may be shared or reused.

**Intermediaries and Service Providers**  
Actors that facilitate data exchange by providing services such as connectors, interoperability infrastructure, registries, trust services, or analytics tools.

**Auditors and Verifiers**  
Independent actors responsible for assessing compliance with governance rules, certification requirements, or technical standards.

Participants may assume multiple roles within the data space depending on the context of specific data exchange.

### GDDS Participants

Participants are entities that have formally joined the GDDS and committed to the governance framework defined in this Rulebook. They hold rights and obligations within the data space and are authorised to engage in data exchange and service provision in accordance with defined rules and policies.

Participants shall comply with the GDDS governance, legal, and technical requirements and shall align their internal data governance processes, including data rights management, quality assurance, and compliance mechanisms, with the GDDS framework.

Participants may assume one or more of the roles defined in the GDDS Roles section, depending on the context of their activities within the data space.

### Participation Management

Participation in GDDS follows a defined lifecycle that includes:

1.  > **participant identification and eligibility assessment,**

2.  > **onboarding and admission procedures,**

3.  > **assignment of roles and access rights,**

4.  > **compliance monitoring and governance enforcement,**

5.  > **suspension, revocation, and voluntary withdrawal procedures.**

These lifecycle processes are supported through a combination of governance procedures and technical mechanisms such as participant registries, identity services, and onboarding tooling.

*Editor's note: Further content will be added in the next version of the Rulebook after co-creation sessions by WP4, WP3.*

#### **1. Participant identification and eligibility assessment**

##### Identity Paths and Credential Enrichment in GDDS

Participation in GDDS follows a layered interaction model. Participants are discovered and validated through registries, authenticated via external trusted identity providers, and subsequently authorised based on enriched identity context. This context is progressively built from identity provider attributes, registry information, and verifiable credentials, and is used to enforce access control policies and support data exchange through GDDS connectors.

Efficient participation in GDDS requires participants to identify themselves and obtain credentials that define their rights to access and use specific data and services. GDDS anticipates **three primary identity pathways** for participation, each corresponding to a type of stakeholder:

###### 1\. Organisational Participants with Their Own Identity Systems

Organisations such as municipalities, real estate companies, consultancies, or research labs may wish to participate using their existing identity infrastructure.

  - > These organisations must first **register themselves as official participants** of GDDS using a recognised organisational identifier (e.g., **LEI** or other trusted digital IDs).

  - > Upon successful registration, the organisation determines **which individuals may represent it** within GDDS and defines the roles and credentials these individuals will receive.

  - > Organisational representatives may then act on behalf of their entity to:
    
      - > Manage datasets
    
      - > Input or extract data
    
      - > Administer services (e.g. onboarding of sub-participants)

  - > **Role-based credentials** are assigned internally and can be enriched further via GDDS processes (see Section 4).

###### 2\. Academic Participants

Individuals working within academic institutions (e.g. universities, applied research centres) may participate via their **existing academic credentials**, such as institutional logins compliant with eduGAIN or national federation protocols.

  - > The **level of access** will depend on the authentication assurances provided by the institution.

  - > If an academic participant requires higher assurance or greater access rights than their institution offers, they may proceed via the **individual pathway** (see below).

###### 3\. Individual Participants

Individuals (e.g. freelancers, private consultants, independent researchers) may:

  - > Access GDDS anonymously — but only to view open resources visible to unauthenticated users.

  - > Use low-assurance digital IDs (e.g. Google, LinkedIn) for limited access, where permitted.

  - > Register using **eIDAS 1.0 -compliant** digital identities from trusted EU providers. These identities can enable secure and verifiable participation in the data space.

###### 4\. Credential Enrichment & Attribute-Based Access

To enable finer-grained access control, participants may enrich their identity by adding **verifiable credentials** to their digital identity wallet. These could include:

  - > Nationality or region of residence (e.g. Bavarian residency for access to regional health data)

  - > Employment or professional role

  - > Diploma or educational attainment

  - > Property ownership or professional certifications

  - > eIDAS 2.0-aligned verified attributes

GDDS will define a **credential ontology** and maintain a list of **trusted credential issuers** for access-related attributes. Data providers must:

  - > Define the **access rules** for their datasets/services

  - > Work with GDDS to identify which credentials are required and from which issuers

  - > Ensure that these mechanisms are operational **before the data is onboarded** into GDDS

#### In addition to user-level identity enrichment, GDDS supports the exchange of verifiable credentials between system components (e.g. connectors) using protocols such as DCP. This occurs during data exchange interactions, enabling secure machine-to-machine communication and enforcement of data access and usage policies.

###### 5\. Group-Based Membership Systems

GDDS may implement **Data User Groups** (similar to virtual organisations or thematic circles), where:

  - > Organisations or individuals may apply for membership

  - > Rules for group membership may be evaluated automatically or through human validation

  - > This model supports flexible data access schemes (e.g. a group of certified consultants)

###### 6\. Human-in-the-Loop (HITL) Approvals

Initially, some access requests may rely on manual validation by data providers — especially where no automated attribute-based access rules have yet been established.

  - > This **non-scalable model** can serve as a practical transition path

  - > GDDS will provide technical and governance support to help data providers **evolve toward automated access control systems**

*Editor's note: Further content will be added in the next version of the Rulebook after co-creation sessions by WP4, WP3.*

#### **2. Onboarding and admission procedures**

#### **3. Assignment of roles and access rights** 

#### **4. Compliance monitoring and governance enforcement,** 

#### **5. Suspension, revocation, and voluntary withdrawal procedures.**

## Data Sovereignty & Technical Governance

Data Sovereignty & Technical Governance defines how data exchange within the GDDS ecosystem is governed and technically enabled.

A key principle of the GDDS governance framework is that **data providers retain sovereignty over their data**. This means that data providers determine the conditions under which their data may be accessed, shared, and reused by other participants.

The governance framework, therefore, establishes the rules and technical mechanisms necessary to ensure that data exchange occurs in a secure, interoperable, and policy-compliant manner.

This governance layer defines policies and operational mechanisms related to:

  - > data access governance and policy enforcement

  - > technical interoperability standards

  - > registry and discovery services

  - > data provenance and traceability

  - > governance of APIs, connectors, and interoperability components.

Technical governance ensures that data exchange within GDDS aligns with recognised interoperability frameworks and European data space standards.

Participants are responsible for ensuring that their internal data governance practices align with the GDDS governance framework. Internal governance processes should address aspects such as:

  - > management of data rights and permissions

  - > data quality assurance

  - > monitoring and observability of data transactions

  - > traceability and provenance of shared data

  - > regulatory compliance.

By combining governance rules with interoperable technical infrastructure, GDDS enables secure data sharing while preserving data sovereignty and operational flexibility for participants.

## Certification & Conformity Framework

The Certification & Conformity Framework ensures that participants, services, and technical components operating within GDDS comply with the governance rules, technical standards, and regulatory obligations defined in the Rulebook.

This framework establishes mechanisms for assessing whether actors and services meet the requirements necessary to participate in the data space.

The Certification & Conformity Framework may include:

  - > certification requirements for specific participant roles

  - > conformity assessment procedures for services and infrastructure components

  - > auditing and monitoring mechanisms

  - > procedures for remediation, suspension, or revocation in cases of non-compliance.

Certification and conformity assessments may be conducted by authorised verification bodies or by governance bodies responsible for oversight within the data space.

Compliance monitoring ensures that participants continue to operate in accordance with the governance framework throughout their participation lifecycle.

In cases of non-compliance, corrective actions may include:

  - > remediation measures,

  - > temporary suspension of participation rights,

  - > revocation of credentials or certifications.

These mechanisms ensure that the GDDS ecosystem maintains a high level of trust, security, and interoperability while remaining aligned with applicable European regulations and recognised technical standards.

