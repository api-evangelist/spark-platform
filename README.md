# Spark Platform

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Spark Platform is the MLS data platform built by FBS, a 100% employee-owned company in Fargo, North Dakota that has served the US Multiple Listing Service industry for over 30 years and operates the Flexmls MLS system for more than 120 MLS organizations. Spark sits in the distribution layer of US residential real estate: it takes MLS content out of Flexmls and exposes it to third-party developers through two documented interfaces — the proprietary Spark API (https://sparkapi.com/v1, SparkQL filtering, listings, contacts, saved searches, market statistics, portals/VOW accounts) and a RESO Web API implementation at the /Reso/OData endpoint (https://replication.sparkapi.com/Version/3/Reso/OData/) serving Property, Member, Office, Media, OpenHouse, Room, Unit, GreenVerification, PowerProduction and Lookup resources against the RESO Data Dictionary. FBS is a RESO Certified technology provider (Unique Organization Identifier T00000052, status "Certified Current") and appears as the certifying provider on RESO Web API Core 2.0.0 and Data Dictionary 1.7 / 2.0 endorsements for 138 MLS organizations plus one commercial board in the public RESO organizations feed; FBS itself additionally holds RESO webhooks 1.0.0 and RESO Common Format 2.0 endorsements. The API posture must be stated honestly: the documentation is genuinely public and unusually complete, developer registration is a free public form, and the endpoints are live — but they are not open. Every probed data endpoint, including the OData $metadata document, returns HTTP 401 "Invalid API key and/or request signed improperly" anonymously. Real data requires a Developer Agreement with FBS, an MLS-approved data plan purchased through the Spark Datamart under an IDX, VOW or Private role, and a per-MLS fee. Certification here is real and verifiable; reachability is licensed. Home market is the United States.

**Areas:** Real Estate · United States · MLS · RESO · Property Listings · IDX · PropTech · Listing Data Infrastructure · OData

## Spark Platform on APIs.io

Everything profiled for Spark Platform is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/spark-platform/](https://apis.io/providers/spark-platform/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [Spark API](https://apis.io/apis/spark-platform/spark-api/) — FBS's proprietary REST API over Flexmls MLS content. Documented services include Listings (plus photos, documents, floor plans, videos, virtual tours, open…
- [Spark RESO Web API](https://apis.io/apis/spark-platform/spark-reso-web-api/) — Spark's implementation of the RESO Web API, exposed as an OData service at the /Reso/OData endpoint and serving data shaped by the RESO Data Dictionary.…
- [Spark Webhooks](https://apis.io/apis/spark-platform/spark-webhooks/) — Outbound webhook delivery from the Spark platform. When a Property, Member or Office record changes in an upstream MLS, Spark POSTs a RESO Web API Entity…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Spark Platform Webhooks](https://apis.io/asyncapis/spark-platform/spark-platform-webhooks/)

#### Collections (1)

Postman and Open Collection request collections.

- [Spark Web API Queries](https://apis.io/collections/spark-platform/postman-spark-platform-spark-web-api-queries/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Spark Platform Authentication](https://apis.io/security/spark-platform/spark-platform-authentication/)
- [Spark Platform Domain Security](https://apis.io/security/spark-platform/spark-platform-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Spark Platform Scopes](https://apis.io/scopes/spark-platform/spark-platform-scopes/)

#### Rate limits (1)

Published request limits.

- [Spark Platform Rate Limits](https://apis.io/rate-limits/spark-platform/spark-platform-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.sparkapi.io/)
- [Documentation](https://sparkplatform.com/docs)
- [Getting started](https://sparkplatform.com/docs/overview/set_up_access)
- [API reference](https://sparkplatform.com/docs/api_services/read_first)
- [Pricing](https://www.sparkapi.io/developers/)
- [Sign up](https://sparkplatform.com/register/developers)
- [Support](https://www.sparkapi.io/contact/)
- [Blog](https://www.sparkapi.io/blog/)
- [Compliance](https://services.reso.org/orgs?showStats=true&showEndorsements=true)
- [Terms of service](https://sparkplatform.com/docs/terms_of_use/developer_agreement_and_terms_of_use)
- [Privacy policy](https://sparkplatform.com/docs/terms_of_use/privacy)
- [GitHub](https://github.com/sparkapi)

## API Evangelist rating

**Kin Score 54.8** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 45.3 |
| Contract governance | 18.2 |
| Operational transparency | 42.1 |
| Developer ergonomics | 69.0 |
| Access clarity | 52.6 |

**Agent readiness 26.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 39.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/spark-platform/](https://apis.io/providers/spark-platform/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Spark Platform: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/spark-platform/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
