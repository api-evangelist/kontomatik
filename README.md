# Kontomatik (kontomatik)

Kontomatik is a Warsaw- and Vilnius-based, PSD2-licensed open banking provider delivering bank data aggregation, KYC, credit scoring, income verification, transaction labeling, and PDF statement parsing across Central and Eastern Europe (Poland, Czech Republic, Romania, Lithuania, Latvia, Estonia) and Iberia (Spain, Portugal). The platform combines an Account Information Service (AIS) with Single, Multiple, and Mixed access modes, Polish-bank PDF parsing in standard and trusted modes, and an analytical stack (labeling, vendor recognition, scoring, profiling, data summary, income confirmation) plus the Kontomatik Report. Operations are managed through the Insight client portal with API-key issuance, IP whitelisting, role-based access, and 2FA.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Open Banking, PSD2, AIS, Bank Data Aggregation, CEE, KYC, Credit Scoring, Transaction Labeling, PDF Parsing

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Coverage

| Country | Code | Banks |
|---|---|---|
| Poland | PL | 32 |
| Spain | ES | 24 |
| Portugal | PT | 22 |
| Czech Republic | CZ | 10 |
| Romania | RO | 8 |
| Lithuania | LT | 6 |
| Latvia | LV | 5 |
| Estonia | EE | 5 |

PDF parsing is Poland-only; AIS and analytical services are country-agnostic across the supported targets.

## APIs

### Kontomatik Account Information Service API
PSD2 AIS connecting end-user bank accounts across 8 CEE / Iberian markets. Supports Single, Multiple (up to 180-day consent), and Mixed access modes, redirection SignIn Flow, background import commands, consent revocation, and a KontoBank mock-bank sandbox.

**Human URL:** [https://developer.kontomatik.com/docs/](https://developer.kontomatik.com/docs/)

- [Documentation — API Overview](https://developer.kontomatik.com/first-steps/api-overview/)
- [Documentation — Unified Docs](https://developer.kontomatik.com/docs/)
- [OpenAPI](openapi/kontomatik-ais-api-openapi.yml)
- [JSON Schema — Owner](json-schema/kontomatik-owner-schema.json)
- [JSON Schema — Account](json-schema/kontomatik-account-schema.json)
- [JSON Schema — Transaction](json-schema/kontomatik-transaction-schema.json)
- [JSON-LD](json-ld/kontomatik-context.jsonld)
- [Naftiko Capability — AIS](capabilities/ais-account-information.yaml)
- [Example — Default Import Result](examples/kontomatik-default-import-example.json)

### Kontomatik PDF Parsing API
Extracts structured owner, account, and transaction data from Polish bank statement and confirmation PDFs in standard or trusted mode, with a per-owner history endpoint and PDF coverage catalog.

**Human URL:** [https://developer.kontomatik.com/docs/](https://developer.kontomatik.com/docs/)

- [OpenAPI](openapi/kontomatik-pdf-parsing-api-openapi.yml)
- [Naftiko Capability — PDF Parsing](capabilities/pdf-statement-parsing.yaml)
- [Example — Statement](examples/kontomatik-pdf-statement-example.json)

### Kontomatik Data Analysis API
ML-powered analytical services on top of imported bank data — labeling, vendor recognition (beta), credit scoring, behavioral profiling (beta), owner features, data summary, income confirmation across four timespans, external-data labeling, cross-source aggregation, and owner data deletion.

**Human URL:** [https://developer.kontomatik.com/docs/](https://developer.kontomatik.com/docs/)

- [OpenAPI](openapi/kontomatik-data-analysis-api-openapi.yml)
- [Naftiko Capability — Labeling](capabilities/transaction-labeling.yaml)
- [Naftiko Capability — Scoring](capabilities/credit-scoring.yaml)
- [Naftiko Capability — Income Confirmation](capabilities/income-confirmation.yaml)
- [Naftiko Capability — Profiling](capabilities/owner-profiling.yaml)
- [JSON Structure — Owner Graph](json-structure/kontomatik-owner-graph-structure.json)
- [Example — Score](examples/kontomatik-score-example.json)

### Kontomatik Report API
Create, list, and retrieve shareable Kontomatik Report tokens (beta) that bundle imported and analyzed data into authenticated, time-bound deliverables.

**Human URL:** [https://developer.kontomatik.com/docs/](https://developer.kontomatik.com/docs/)

- [OpenAPI](openapi/kontomatik-report-api-openapi.yml)
- [Naftiko Capability — Reporting](capabilities/report-generation.yaml)

## Authentication & Environments

- Auth: `X-Api-Key` header issued via the Insight portal; requests must originate from a whitelisted server.
- Production base URL: `https://api.kontomatik.com/v1/`
- Test base URL: `https://test.api.kontomatik.com/v1/`
- Sandbox: KontoBank mock bank session via `/v1/mock-session.xml`.

## Operational Artifacts

- [Plans](plans/kontomatik-plans-pricing.yml) — contract-driven; no public list pricing.
- [Rate Limits](rate-limits/kontomatik-rate-limits.yml) — IP whitelisting, X-Api-Key, contractual volumes, 180-day consent window, 24-hour default retention.
- [FinOps](finops/kontomatik-finops.yml) — B2B invoicing aligned to AIS imports, PDFs parsed, analysis calls, and active Multiple Access consents.
- [Vocabulary](vocabulary/kontomatik-vocabulary.yml)
- [Spectral Rules](rules/kontomatik-rules.yml)

## Compliance

- ISO 27001 certified information security management
- PSD2 licensed AIS provider
- GDPR compliant (24-hour default data retention)

## Contact

- General: contact@kontomatik.com
- Sales: sales@kontomatik.com
- Support: support@kontomatik.com
- Compliance: compliance@kontomatik.com
- Warsaw HQ: Kontomatik sp. z o.o., Bonifraterska 17, 00-203 Warsaw, Poland
- Vilnius: Kontomatik UAB, Didžioji 18, LT-01128 Vilnius, Lithuania
- Insight portal: https://insight.kontomatik.com/
- Book a demo: https://calendly.com/dominik-wolski-kontomatik/demo-call
