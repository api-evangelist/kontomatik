# Kontomatik (kontomatik)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
