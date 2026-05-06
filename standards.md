# Standards & API Reference

> Project: Environmental Compliance Manager · Generated: 2026-05-04

## Industry Standards & Specifications

### ISO Standards

**ISO 14001:2015 / ISO 14001:2026 — Environmental Management Systems**
- URL: https://www.iso.org/standard/60857.html
- The primary international standard for Environmental Management Systems (EMS). Defines the framework for identifying, managing, monitoring, and improving an organisation's environmental impact. Most commercial EHS compliance platforms align their module structure directly to ISO 14001 requirements. ISO 14001:2026 is the current revision, replacing ISO 14001:2015.

**ISO 14031:2021 — Environmental Performance Evaluation**
- URL: https://www.iso.org/standard/78374.html
- Provides guidelines for designing and using environmental performance evaluation processes and selecting environmental performance indicators. Directly relevant to the metrics, dashboards, and KPI tracking features of a compliance manager.

**ISO 14040:2006 / ISO 14044:2006 — Life Cycle Assessment**
- URL: https://www.iso.org/standard/37456.html
- ISO 14040 establishes principles and framework for Life Cycle Assessment (LCA) covering all stages from raw material extraction to disposal. ISO 14044 provides detailed requirements and guidelines. Relevant when the compliance manager needs to track product environmental footprint alongside permit compliance.

**ISO 14064 — Greenhouse Gas Accounting and Verification**
- URL: https://www.iso.org/standard/66453.html
- Three-part standard: 14064-1 (organisational GHG inventory), 14064-2 (project-level GHG emissions), 14064-3 (verification and validation). Directly relevant to Scope 1/2/3 emissions tracking modules. Aligns closely with GHG Protocol.

**ISO 50001:2018 — Energy Management Systems**
- URL: https://www.iso.org/standard/69426.html
- Establishes requirements for energy management systems, focused on energy performance indicators and energy baselines. Overlaps with ISO 14001 for organisations managing energy as an environmental aspect. Relevant to energy consumption tracking in compliance platforms.

**ISO 19650 — Information Management / BIM (for facilities)**
- URL: https://www.iso.org/standard/68078.html
- Relevant for compliance managers that need to track environmental conditions tied to physical assets and facilities, particularly when integrating with building information models for large industrial sites.

---

### W3C & IETF Standards

**RFC 7231 — HTTP/1.1 Semantics and Content**
- URL: https://datatracker.ietf.org/doc/html/rfc7231
- Foundational standard for REST API design. All HTTP-based environmental compliance APIs (EPA, Intelex, Cority, Sphera) rely on HTTP semantics for request/response interactions, status codes, and content negotiation.

**RFC 6749 — OAuth 2.0 Authorization Framework**
- URL: https://datatracker.ietf.org/doc/html/rfc6749
- The standard authorization framework used for secure API access delegation. Intelex v6.6.7+ and Sphera both use OAuth 2.0 client credentials flows for their REST APIs. Essential for any third-party integrations connecting enterprise ERP or HR systems to a compliance manager.

**RFC 8288 — Web Linking**
- URL: https://datatracker.ietf.org/doc/html/rfc8288
- Defines `Link` header semantics used for pagination and HATEOAS patterns in REST APIs. Relevant for large compliance data exports (e.g., paginating through thousands of facility records in EPA Envirofacts).

**W3C PROV — Provenance Data Model**
- URL: https://www.w3.org/TR/prov-overview/
- Standard for representing provenance information (who produced data, when, and how). Highly relevant to compliance audit trails and chain-of-custody documentation for environmental monitoring data.

**ETSI NGSI-LD (ETSI GS CIM 009)**
- URL: https://www.etsi.org/deliver/etsi_gs/CIM/001_099/009/
- ETSI standard for context information management via a linked-data API. Used for IoT sensor integration in smart environments, including environmental monitoring stations. Relevant when a compliance manager ingests real-time air quality, water discharge, or temperature sensor data.

---

### Data Model & API Specifications

**GHG Protocol — Corporate Accounting and Reporting Standard**
- URL: https://ghgprotocol.org/corporate-standard
- The world's most widely used greenhouse gas accounting standard, used by 92% of Fortune 500 companies reporting to CDP. Defines Scope 1 (direct), Scope 2 (purchased energy), and Scope 3 (value chain) emissions. Any compliance manager's GHG module must follow this data model. The GHG Protocol is directly referenced in IFRS S2.

**GHG Protocol — Scope 3 Standard**
- URL: https://ghgprotocol.org/scope-3-standard
- Extension of the corporate standard covering 15 categories of value chain emissions. Increasingly required by CSRD and IFRS S2 disclosures.

**OpenAPI Specification 3.1**
- URL: https://spec.openapis.org/oas/v3.1.0
- The standard for describing REST APIs in a machine-readable format. All major EHS platforms (Intelex, Sphera, EPA ECHO) publish or reference OpenAPI-compatible documentation. An open-source compliance manager should publish its own OpenAPI 3.1 spec to facilitate integration.

**XBRL / iXBRL — eXtensible Business Reporting Language**
- URL: https://www.xbrl.org/
- Machine-readable format mandated by CSRD for digital tagging of sustainability disclosures. The ESRS XBRL Taxonomy was developed by EFRAG and handed to ESMA for regulation. Any compliance manager targeting EU CSRD reporting must support XBRL export. XBRL tagging will also become mandatory under SEC sustainability disclosure rules.

**ESRS XBRL Taxonomy (EFRAG)**
- URL: https://www.efrag.org/en/sustainability-reporting/esrs-workstreams/digital-reporting-with-xbrl
- Specific taxonomy developed by EFRAG for digitally tagging ESRS sustainability disclosures under CSRD. Companies must categorise sustainability data based on ESRS in structured, machine-readable format.

---

### Regulatory Frameworks & Reporting Standards

**EU CSRD — Corporate Sustainability Reporting Directive**
- URL: https://finance.ec.europa.eu/capital-markets-union-and-financial-markets/company-reporting-and-auditing/company-reporting/corporate-sustainability-reporting_en
- EU directive requiring large companies to publish detailed reports on environmental and social impact. Reporting must follow European Sustainability Reporting Standards (ESRS) and be digitally tagged in XBRL format. First companies applied rules for 2024 financial year, with reports due in 2025.

**ESRS — European Sustainability Reporting Standards**
- URL: https://www.efrag.org/en/sustainability-reporting/esrs-standards
- Ten topic-specific standards under CSRD including 5 environmental topics (climate change, pollution, water, biodiversity, resource use). Any compliance manager targeting European enterprise clients must map to ESRS data requirements.

**IFRS S2 — Climate-related Disclosures (ISSB)**
- URL: https://www.ifrs.org/issued-standards/ifrs-sustainability-standards-navigator/ifrs-s2-climate-related-disclosures/
- ISSB standard for climate-related financial disclosures, effective for periods beginning on or after 1 January 2024. Built on TCFD recommendations. Requires GHG emissions reporting in accordance with GHG Protocol. Increasingly mandatory across jurisdictions.

**EU EMAS — Eco-Management and Audit Scheme**
- URL: https://green-business.ec.europa.eu/eco-management-and-audit-scheme-emas_en
- EU voluntary environmental management tool (Regulation EC No 1221/2009). Exceeds ISO 14001 requirements with mandatory regulatory compliance verification, employee engagement, and public environmental reporting. Over 4,600 organisations and 7,900 sites registered.

**EPA NPDES — National Pollutant Discharge Elimination System**
- URL: https://www.epa.gov/npdes/electronic-reporting-epas-npdes-general-permits
- US federal program requiring electronic permit reporting for water discharges. The NPDES Electronic Reporting Rule mandates electronic DMR (Discharge Monitoring Report) submission via NetDMR or state equivalents. Key data interchange requirement for water compliance modules.

**EPA GHGRP — Greenhouse Gas Reporting Program**
- URL: https://www.epa.gov/ghgreporting
- US federal program requiring large GHG emission sources to report to the EPA via the e-GGRT web-based tool. Defines calculation methodologies at 40 CFR Part 98. Any compliance manager targeting large US facilities must integrate with e-GGRT submission workflows.

**EPA RCRA / RCRAInfo — Hazardous Waste Reporting**
- URL: https://rcrainfo.epa.gov/
- US hazardous waste management system. Facilities submit RCRA Notifications, Biennial Reports, and manifest data through RCRAInfo and MyRCRAID. Key compliance obligation for any facility handling hazardous waste.

**OSHA Electronic Injury Reporting (ITA API)**
- URL: https://www.osha.gov/injuryreporting/
- OSHA's Injury Tracking Application requires electronic submission of Form 300A, 300, and 301 data. Effective January 2024, high-hazard industries must submit electronically. OSHA provides an API for automated recordkeeping system transmission.

---

### Security & Authentication Standards

**OAuth 2.0 (RFC 6749) — API Authorization**
- The standard authorization framework used across EHS platform APIs. Intelex uses client credentials flow for secure token-based access. Essential for integrating compliance data with enterprise systems without sharing credentials.

**OpenID Connect 1.0**
- URL: https://openid.net/connect/
- Identity layer on top of OAuth 2.0. Used for SSO integration in enterprise EHS deployments connecting to corporate identity providers (Azure AD, Okta).

**TLS 1.3 — Transport Layer Security**
- URL: https://datatracker.ietf.org/doc/html/rfc8446
- Current minimum standard for securing API data in transit. EHS compliance data involves sensitive facility and emissions data; TLS 1.3 with AES-256 encryption is the baseline security requirement.

**NIST SP 800-53 — Security and Privacy Controls**
- URL: https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final
- US federal framework for security controls. Relevant for compliance managers deployed in regulated industries or government contexts where FedRAMP compliance may be required.

---

## Similar Products — Developer Documentation & APIs

### EPA Envirofacts Data Service API

- **Description:** RESTful data service providing programmatic access to ~20 EPA environmental databases including RCRA, TRI, SDWIS, ECHO, and RadNet. Allows querying, filtering, sorting, and paginating across regulated facility data.
- **API Documentation:** https://www.epa.gov/enviro/envirofacts-data-service-api
- **Base URL:** `https://data.epa.gov/efservice/[table]/[column][operator][value]/[format]`
- **SDKs/Libraries:** None official; RESTful HTTP calls; supports JSON, CSV, XML, Excel, Parquet output
- **Developer Guide:** https://www.epa.gov/enviro/envirofacts-data-developer-services
- **Standards:** REST, HTTP; no authentication required for public data
- **Authentication:** None (public dataset)

### EPA ECHO Web Services

- **Description:** Enforcement and Compliance History Online provides compliance and enforcement data for ~800,000 EPA-regulated facilities. Covers CAA, CWA, RCRA, SDWA, and TRI programs including inspection history, violations, enforcement actions, and penalties.
- **API Documentation:** https://echo.epa.gov/tools/web-services
- **SDKs/Libraries:** Map Services (GIS), Quick Search Widget (embeddable), bulk data downloads
- **Developer Guide:** https://echo.epa.gov/resources/general-info/tool-guide
- **Standards:** REST/JSON, GIS Map Services
- **Authentication:** None (public dataset)

### EPA AirData AQS (Air Quality System) API

- **Description:** Provides access to air quality monitoring data collected at thousands of monitoring stations across the US. Returns ambient air quality readings for regulated pollutants including PM2.5, ozone, NO2, SO2, and CO.
- **API Documentation:** https://aqs.epa.gov/aqsweb/documents/data_api.html
- **SDKs/Libraries:** R package (`RAQSAPI`), Python wrapper available from community
- **Developer Guide:** https://aqs.epa.gov/aqsweb/documents/data_api.html
- **Standards:** REST/JSON
- **Authentication:** API Key (registered via aqs.epa.gov)

### Intelex REST API

- **Description:** Full-featured REST API for the Intelex EHS platform, providing create/read/update/delete access to all application objects including incidents, permits, audits, tasks, and environmental measurements. The same API used internally by the Intelex web application.
- **API Documentation:** https://developers.intelex.com/
- **SDKs/Libraries:** Code examples in JavaScript and C#; no official SDK
- **Developer Guide:** https://developers.intelex.com/
- **Standards:** REST/JSON, OpenAPI-compatible; OData query options for filtering
- **Authentication:** Basic Auth, API Key, OAuth 2.0 client credentials (v6.6.7+)

### Cority Enviance API

- **Description:** REST API for the Cority Enviance environmental data management platform, providing access to environmental monitoring data, permit conditions, compliance calculations, and facility records. Described by Cority as "the most robust API available in our industry."
- **API Documentation:** https://api.enviance.com/
- **SDKs/Libraries:** Full SDK available; Swagger UI available at `/swagger`
- **Developer Guide:** https://api.enviance.com/ (requires Cority Enviance Connectors licence)
- **Standards:** REST/JSON, Swagger/OpenAPI
- **Authentication:** API Key (Enviance Connectors licence required)

### Sphera SpheraCloud REST API

- **Description:** REST API for the SpheraCloud EHS and sustainability platform, supporting integrations for operational risk, environmental accounting (Scope 1/2/3), and product stewardship. Uses Sphera Exchange (Azure API Management) to expose REST and SOAP APIs.
- **API Documentation:** https://platformscdevdocs.z21.web.core.windows.net/
- **SDKs/Libraries:** Sphera Exchange SDK; integration via Logic Apps and Service Bus
- **Developer Guide:** https://platformscdevdocs.z21.web.core.windows.net/general/guidance/sphera-exchange.html
- **Standards:** REST/JSON, SOAP; Azure API Management
- **Authentication:** OAuth 2.0

### ArcGIS REST API (Esri)

- **Description:** Geospatial API platform used for environmental compliance spatial analysis — overlaying facility permits with ecological data layers (wetlands, flood zones, habitat areas). Used by environmental regulators and compliance teams for spatial permit review and monitoring.
- **API Documentation:** https://developers.arcgis.com/rest/
- **SDKs/Libraries:** ArcGIS Maps SDK for JavaScript, Python (`arcgis`), .NET, Java, Swift, Kotlin, Qt
- **Developer Guide:** https://developers.arcgis.com/documentation/
- **Standards:** REST/JSON, OGC-compliant, OpenAPI 3.0 for select services
- **Authentication:** API Key or OAuth 2.0 (ArcGIS Identity)

### OSHA Injury Tracking Application (ITA) API

- **Description:** API for automated electronic submission of OSHA recordkeeping data (Forms 300, 300A, 301) to the OSHA ITA. Mandatory for high-hazard industry establishments from January 2024.
- **API Documentation:** https://www.osha.gov/injuryreporting/
- **SDKs/Libraries:** None official; direct REST submission
- **Developer Guide:** https://www.osha.gov/injuryreporting/
- **Standards:** REST/JSON
- **Authentication:** API Key (via OSHA ITA registration)

### CDP API (Carbon Disclosure Project)

- **Description:** API for submitting corporate climate and environmental disclosures to the CDP platform. Benchmark Gensuite supports direct CDP submission via API. CDP data is used by investors and customers assessing corporate environmental performance.
- **API Documentation:** https://www.cdp.net/en/guidance/guidance-for-companies
- **SDKs/Libraries:** Limited; used by EHS platforms for direct disclosure submission
- **Standards:** REST/JSON
- **Authentication:** CDP account credentials

---

## Notes

**Emerging standards gap:** There is no single universal data interchange format for environmental permit conditions and compliance obligations across jurisdictions. The EPA CDX and EU EMAS use different data models, and state/provincial regulatory agencies frequently have their own submission formats. An open-source compliance manager could provide significant value by abstracting these differences behind a normalised internal data model.

**XBRL adoption curve:** XBRL tagging for CSRD/ESRS disclosures is mandatory for EU companies from 2025 onwards and is expected to become mandatory under SEC rules for US companies. This is still a largely unsolved integration problem for most mid-market EHS platforms.

**AI opportunity with regulatory text:** No current standard exists for machine-readable regulatory obligation extraction from permit documents. This is the core gap an AI-native compliance manager could address by automatically parsing permit conditions into structured compliance calendars.

**GHG Protocol revision in progress:** As of 2024–2025, the GHG Protocol is undergoing a major revision of its Corporate Standard, with the updated version expected to change Scope 3 category definitions. Any compliance manager implementing GHG tracking should design for schema evolution.
