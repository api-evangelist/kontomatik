# Kontomatik (kontomatik)

Kontomatik is a Warsaw- and Vilnius-based PSD2-licensed open banking provider delivering bank data aggregation, KYC, credit scoring, income verification, transaction labeling, and PDF statement parsing across Central and Eastern Europe (Poland, Czech Republic, Romania, Lithuania, Latvia, Estonia) and Iberia (Spain, Portugal). The platform combines an Account Information Service (AIS) with Single, Multiple, and Mixed access modes, Polish-bank PDF parsing in standard and trusted modes, and an analytical stack (labeling, vendor recognition, scoring, profiling, data summary, income confirmation) plus the Kontomatik Report. Operations are managed through the Insight client portal with API-key issuance, IP whitelisting, role-based access, and 2FA.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Open Banking
- PSD2
- AIS
- Bank Data Aggregation
- CEE
- KYC
- Credit Scoring
- Transaction Labeling
- PDF Parsing

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Kontomatik Account Information Service API

PSD2-regulated Account Information Service for connecting end-user bank accounts across Poland, Czech Republic, Spain, Portugal, Romania, Lithuania, Latvia, and Estonia. Supports Single Access (one-time fetch), Multiple Access (up to 180-day consent tokens), and Mixed Access. Includes redirection SignIn Flow, background import commands, consent revocation, and a KontoBank mock-bank sandbox.

- **Human URL:** [https://developer.kontomatik.com/docs/](https://developer.kontomatik.com/docs/)

#### Tags

- Open Banking
- PSD2
- AIS
- Bank Data

#### Properties

- [Documentation](https://developer.kontomatik.com/first-steps/api-overview/)
- [Documentation](https://developer.kontomatik.com/docs/)
- [OpenAPI](openapi/kontomatik-ais-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kontomatik-ais-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kontomatik-ais-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/kontomatik-owner-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/kontomatik-account-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/kontomatik-transaction-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/kontomatik-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Kontomatik PDF Parsing API

Extract structured owner, account, and transaction data from Polish bank statement and transaction confirmation PDFs. Offers standard mode (rejects on verification failures) and trusted mode (returns data even when verification fails), plus a per-owner history endpoint and the PDF coverage catalog.

- **Human URL:** [https://developer.kontomatik.com/docs/](https://developer.kontomatik.com/docs/)

#### Tags

- PDF Parsing
- Document AI
- Bank Statements
- Poland

#### Properties

- [Documentation](https://developer.kontomatik.com/docs/)
- [OpenAPI](openapi/kontomatik-pdf-parsing-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kontomatik-pdf-parsing-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kontomatik-pdf-parsing-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/kontomatik-pdf-statement-example.json)

### Kontomatik Data Analysis API

ML-powered analytical services on top of imported bank data — transaction labeling, vendor recognition (beta), credit scoring with repayment probability, behavioral profiling (beta), owner features, data summaries by category, income confirmation across four configurable timespans, external-data labeling for non-bank transactions, cross-source aggregation, and owner data deletion.

- **Human URL:** [https://developer.kontomatik.com/docs/](https://developer.kontomatik.com/docs/)

#### Tags

- Transaction Labeling
- Credit Scoring
- Income Verification
- Profiling
- Machine Learning

#### Properties

- [Documentation](https://developer.kontomatik.com/docs/)
- [OpenAPI](openapi/kontomatik-data-analysis-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kontomatik-data-analysis-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kontomatik-data-analysis-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/kontomatik-score-example.json)
- [JSON Structure](json-structure/kontomatik-owner-graph-structure.json)

### Kontomatik Report API

Create, list, and retrieve shareable Kontomatik Report tokens that bundle imported AIS and PDF data together with the analytical outputs into authenticated, time-bound deliverables (beta).

- **Human URL:** [https://developer.kontomatik.com/docs/](https://developer.kontomatik.com/docs/)

#### Tags

- Reporting
- Beta
- Bank Data

#### Properties

- [Documentation](https://developer.kontomatik.com/docs/)
- [OpenAPI](openapi/kontomatik-report-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kontomatik-report-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/kontomatik-report-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://kontomatik.com)
- [Documentation](https://developer.kontomatik.com/)
- [Documentation](https://developer.kontomatik.com/docs/)
- [Getting Started](https://developer.kontomatik.com/first-steps/)
- [Documentation](https://developer.kontomatik.com/first-steps/api-overview/)
- [Documentation](https://developer.kontomatik.com/first-steps/getting-api-access/)
- [Documentation](https://developer.kontomatik.com/first-steps/insight/)
- [Documentation](https://developer.kontomatik.com/user-guides/)
- [Support](https://developer.kontomatik.com/faq/)
- [Sign Up](https://insight.kontomatik.com/)
- [Support](https://kontomatik.com/contact)
- [Sign Up](https://calendly.com/dominik-wolski-kontomatik/demo-call)
- [LinkedIn](https://www.linkedin.com/company/kontomatik)
- [GitHub Organization](https://github.com/kontomatik)
- [Blog](https://kontomatik.com/blog)
- [Plans](plans/kontomatik-plans-pricing.yml)
- [Rate Limits](rate-limits/kontomatik-rate-limits.yml)
- [Fin Ops](finops/kontomatik-finops.yml)
- [Vocabulary](vocabulary/kontomatik-vocabulary.yml)
- [Spectral Rules](rules/kontomatik-rules.yml)
- [Coverage](undefined)
- [Features](undefined)
- [Office](undefined)
- [Email](undefined)
- [Compliance](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
