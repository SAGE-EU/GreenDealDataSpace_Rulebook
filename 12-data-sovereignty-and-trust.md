# Data Sovereignty and Trust

## Identity & Attestation Management

The Identity & Attestation Management building block provides a trusted foundation for onboarding, verifying, and maintaining participants’ credentials within the GDDS ecosystem.

It ensures that every actor and asset is uniquely identifiable, authenticated, and authorized before engaging in data transactions, while preserving sovereignty over identity data.

By combining machine-readable rulebooks, standardized credential formats, and secure exchange protocols, GDDS enables participants to present and verify attestations, such as membership, compliance, or sector-specific qualifications, across multiple domains and jurisdictions.

This capability is essential for:

  - > Trust & Compliance – Verifying that participants meet the GDDS baseline requirements and any sector-specific rules.

  - > Interoperability – Enabling credential federation across other recognised data spaces and trust frameworks.

  - > Efficiency – Reducing onboarding time and transaction costs through reusable, portable credentials.

### **Core Capabilities**

  - > Trusted Legal & Natural Person Identification – Support for both organisational and human identities, aligned with EU-recognised schemes (eIDAS, Qualified Trust Service Providers).

  - > Secure Credential Lifecycle Management – Issuance, renewal, revocation, and validation of credentials in compliance with GDDS governance.

  - > Conformity Assessment Integration – Alignment with the GDDS Rulebook and automated compliance checks.

  - > Credential Portability & Federation – Interoperable with other ecosystems through open standards (W3C Verifiable Credentials, DIDs, OIDC4VC).

  - > Attestation Diversity – Support for multiple attestation types, including identity, membership, and compliance attestations.

### **Design Principles**

  - > Self-Sovereign Identity (SSI) – Allow participants to control their identity attributes while meeting governance requirements.

  - > Standards-First Approach – Prioritise open, widely adopted technical and governance standards.

  - > Federation over Centralisation – Enable multiple trust domains to coexist with GDDS as the trust anchor.

  - > Policy-Linked Identity – Ensure access and usage rights are tied to verified identities.

  - > Credential Reuse – Encourage interoperability with existing compliance certifications to minimise duplication.

*Further content will be added after co-creation sessions.*

## Trust Framework

The Trust Framework defines the rules, roles, and mechanisms that underpin confidence in all GDDS interactions. It ensures that participants, services, and transactions can be validated against a common rulebook, making trust decisions faster, more transparent, and interoperable across sectors.

The framework serves as the connective tissue between governance requirements and technical enablers, linking identity verification, attestation management, access control, and compliance into one coherent system. By setting clear acceptance criteria for trust anchors, and trust service providers, GDDS can guarantee the authenticity, integrity, and security of both participants and the data they share.

Where possible, GDDS can adopt and extend existing trust frameworks (e.g., Gaia-X, iSHARE, IDSA) to ensure European alignment while tailoring rules to Green Deal–specific use cases.

### **Core Capabilities**

  - > Participant & Service Verification – Ensure all participants and services are verifiable against governance requirements and technical standards.

  - > Governance Enforcement – Apply the GDDS Rulebook to enforce organisational, technical, and semantic interoperability.

  - > Trust Entity Management – Define, accredit, and maintain the registry of Trust Anchors, Trust Service Providers, Conformity Assessment Bodies, and Notaries.

  - > Registry Integration – Store the Rulebook, accreditation lists, revoked trust entities, and compliance schemas in the GDDS registry for public reference.

  - > Multi-Level Trust – Define different assurance levels based on source reliability, credential type, or attestation scope.

*Further content will be added after co-creation sessions.*

## Access & Usage Policies Enforcement

The Access & Usage Policies Enforcement building block defines the rules, processes, and technical mechanisms that govern how data can be accessed, used, and shared within the GDDS ecosystem. It ensures that:

  - > Access is granted only to authorised parties.

  - > Data usage follows explicitly agreed purposes and obligations.

  - > Consent is managed transparently and revocably.

  - > Compliance is verifiable and enforceable in both organisational and technical terms.

It acts as the operational layer of data sovereignty, linking identity management, trust rules, and legal agreements into actionable, machine-readable policies.

### **Core Capabilities**

1.  > Access Control Policies
    
      - > Define who can access which data and under what circumstances (role-, attribute-, or context-based).
    
      - > Enforce pre-access checks through Policy Enforcement Points (PEP) and Policy Decision Points (PDP).

2.  > Usage Control Policies
    
      - > Define what actions (e.g., analyse, share, modify) are permitted once access is granted.
    
      - > Apply continuous usage checks where obligations or prohibitions change over time.

3.  > Consent Management Policies
    
      - > Manage data subject consent and legal permissions.
    
      - > Support opt-in/opt-out and revocation workflows.
    
      - > Maintain audit trails for compliance proof.

4.  > Policy Transformation & Interoperability
    
      - > Translate agreements into machine-readable formats (e.g., ODRL).
    
      - > Ensure semantic interoperability between participants’ systems.

5.  > Compliance Tracking & Enforcement Proof
    
      - > Log and audit every access and usage event.
    
      - > Provide verifiable enforcement evidence for trust and dispute resolution.

*Further content will be added after co-creation sessions.*
