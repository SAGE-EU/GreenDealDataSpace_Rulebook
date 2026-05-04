# Intermediaries and Operators

In GDDS, intermediaries and operators play a crucial enabling role, making data accessible, trustworthy, and compliant with EU regulations. They help reduce complexity and lower barriers to entry for participants.

Key responsibilities may include:

  - > **Identity and Access Management** (e.g. authenticating participants, issuing credentials);

  - > **Data and Service brokerage** (e.g. data search and matchmaking);

  - > **Compliance assurance** (e.g. ensuring data usage aligns with CSRD, EPBD, or GDPR);

  - > **Onboarding and support** for participants, especially SMEs and municipalities. (- Connectors?)

Operators might include neutral industry bodies, domain-specific hubs, or trusted IT providers. In GDDS, multiple operators can coexist under federated rules, enabling sectoral specialization while ensuring interoperability through shared frameworks (e.g. iSHARE, Gaia-X compliance).

## Catalogue and Data Brokerage Services

A dedicated [**<span class="underline">Catalogue portal</span>**](https://beta.catalogue.gdds.eu/search/all_collection?q=) has been developed to significantly enhance dataset discovery within the GDDS ecosystem by leveraging deep integration with the Federated Catalogue API. The Catalogue, based on the CYFRONET technical solution, provides a unified and intuitive search interface that allows users to efficiently explore a wide range of metadata resources. Advanced filtering capabilities and faceted search capabilities enable users to refine queries based on multiple criteria, including the possibility to restrict results to selected underlying catalogues. By exposing harmonised and standardized metadata and supporting structured navigation across federated resources, the Catalogue improves visibility and accessibility of datasets while reducing fragmentation between catalogue services. Upon selecting a dataset, users are seamlessly redirected to the Federated Catalogue dashboard, where detailed metadata can be reviewed and where access negotiation and subsequent data transfer can be initiated in accordance with governance frameworks.

From a technical perspective, the Catalogue is implemented as a modular web application consisting of a Python FastAPI backend and an Angular frontend, supported by Apache Solr as the search engine and PostgreSQL database. Metadata records are retrieved from the Federated Catalogue API and synchronised into the search index through a dedicated transformer service, also implemented in Python using FastAPI, which ensures consistent metadata structure and efficient indexing. This architecture enables scalable ingestion, fast querying, and flexible filtering of metadata across multiple catalogues.

In parallel, the integration of the iSHARE Trust Framework components is currently underway. This integration will enable federated authentication via trusted identity providers (e.g. based on Keycloak) operated by or on behalf of organisations registered within the data space. As a result, users will benefit from a single sign-on experience, allowing them to authenticate once and seamlessly move between the Catalogue portal and Federated Catalogue dashboard without repeated logins. This ensures a secure, compliant, and user-friendly interaction with GDDS data assets while maintaining strict adherence to trust and identity management principles.

Through these combined capabilities, the Catalogue portal reinforces the role of intermediaries within the GDDS framework. It facilitates trusted data discovery, supports efficient access brokerage, and promotes interoperability across distributed data services. Ultimately, it contributes to a more integrated, scalable, and user-centric data-sharing environment.

## Identity and Access Management

### Overview

Identity and Access Management (IAM) represents a foundational component of the GDDS, providing the mechanisms required to securely identify users and control their access to services, data, and computational resources. IAM covers the full lifecycle of digital identities for both natural persons (e.g. researchers, data stewards) and legal entities (e.g. participating organisations, data providers). This lifecycle ranges from initial registration and onboarding of users and services, through authentication and authorization, to the management, renewal, and revocation of credentials.

### IAM Architecture and Components

The IAM framework relies on a combination of external and internal components to manage identities, authenticate users and services, and control access to resources across the GDDS. Specifically, it leverages existing external trusted identity providers to authenticate users acting on behalf of participant organisations and establish appropriate levels of assurance\[1\] regarding their identities. In addition, GDDS uses internal or federated data space registries to manage and validate participant metadata, including status, roles, and entitlements within the ecosystem. These registries support trust establishment and authorisation decisions but are not involved in the authentication process itself.

### Standards and Interoperability

To ensure technical interoperability, GDDS adopts established standards for authentication and federation (e.g. OAuth 2.0, OpenID Connect, SAML), allowing users to reuse existing credentials where possible and reducing duplication of identities:

  - > Academic and research users may authenticate via eduGAIN-connected identity providers.

  - > Business and government participants may rely on corporate identity providers, eIDAS-compliant identities, or other trusted authentication schemes, depending on regulatory and assurance requirements.

###  Access Control and Authorisation

The IAM framework also includes the management of user attributes, roles, and group memberships, which are used to enforce fine-grained access control policies aligned with organizational, legal, and regulatory requirements. By supporting role-based and attribute-based access control models, IAM enables flexible and scalable permission management across diverse user communities and service providers.

### Federation, Trust and Security Mechanisms

In addition, IAM plays a critical role in enabling secure collaboration in federated and distributed environments. It supports interoperability between multiple identity federations and infrastructures, allowing users to access services across organizational and national boundaries using a single digital identity (Single Sign-On). The framework incorporates trust and security mechanisms such as federated authentication, credential assurance levels, logging, and auditing, ensuring compliance with applicable policies and standards.

The Identity and Access Management framework of the GDDS will be developed with a focus on establishing the core IAM architecture, defining governance and trust policies, integrating suitable identity providers, and implementing robust authentication and authorization mechanisms to support secure and interoperable access for all participating stakeholders.

The framework follows an evolutionary approach. GDDS has adopted the Decentralised Claims Protocol (DCP) and Verifiable Credentials (VCs) to support trust, delegation, and authorisation across the data space. These complement existing federation-based approaches (e.g. OAuth 2.0 / OpenID Connect and SAML), which continue to be used for user authentication and service integration. Access decisions are based on the verification of claims issued by trusted authorities and evaluated against trusted registries and policies, enabling fine-grained delegation and interoperability with emerging European frameworks such as eIDAS 2.0.

#
