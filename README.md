# Spark Platform (spark-platform)

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

Spark Platform is the MLS data platform built by FBS, a 100% employee-owned company in Fargo, North Dakota that has served the US Multiple Listing Service industry for over 30 years and operates the Flexmls MLS system for more than 120 MLS organizations. Spark sits in the distribution layer of US residential real estate, exposing MLS content to third-party developers through a proprietary Spark API and a RESO Web API OData implementation. FBS is a RESO Certified technology provider (UOI T00000052) and is the certifying provider on RESO Web API Core 2.0.0 and Data Dictionary 1.7 / 2.0 endorsements for 138 MLS organizations. The documentation is fully public and the endpoints are live, but every data endpoint — including the OData `$metadata` contract — returns HTTP 401 without an MLS-approved key. Certification here is real; reachability is licensed.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/spark-platform/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/spark-platform/refs/heads/main/apis.yml)

## Tags

- Real Estate
- United States
- MLS
- RESO
- Property Listings
- IDX
- PropTech
- Listing Data Infrastructure
- OData

## Timestamps

- **Created:** 2026-07-26
- **Modified:** 2026-07-26

## APIs

### Spark API

FBS's proprietary REST API over Flexmls MLS content — listings and their photos, documents, floor plans, videos, virtual tours, open houses, rooms, units, history and rules, plus contacts, saved searches, listing carts, portals/VOW accounts, market statistics, overlays, standard and custom field metadata, system info, and a developers service for keys, roles, domains and usage. Filtering uses SparkQL. Anonymous requests return HTTP 401.

- **Human URL:** [https://sparkplatform.com/docs/overview/api](https://sparkplatform.com/docs/overview/api)
- **Base URL:** `https://sparkapi.com/v1`

#### Tags

- MLS
- Property Listings
- Real Estate
- IDX

#### Properties

- [Documentation](https://sparkplatform.com/docs)
- [API Reference](https://sparkplatform.com/docs/api_services/read_first)
- [Documentation](https://sparkplatform.com/docs/api_services/listings)
- [Documentation](https://sparkplatform.com/docs/api_services/market_statistics)
- [Documentation](https://sparkplatform.com/docs/supporting_documentation/sparkql_grammar)
- [Documentation](https://sparkplatform.com/docs/supporting_documentation/search_and_paging_syntax)
- [Authentication](https://sparkplatform.com/docs/authentication/access_token)
- [Sign Up](https://sparkplatform.com/register/developers)
- [Terms of Service](https://sparkplatform.com/docs/terms_of_use/developer_agreement_and_terms_of_use)

### Spark RESO Web API

Spark's implementation of the RESO Web API, exposed as an OData service at the `/Reso/OData` endpoint against the RESO Data Dictionary. Resources are Property, Member, Office, Media, OpenHouse, Room, Unit, Green Verification, Power Production and Lookup. The `$metadata` document is the machine-readable contract but returned HTTP 401 on 2026-07-26.

- **Human URL:** [https://sparkplatform.com/docs/reso/overview](https://sparkplatform.com/docs/reso/overview)
- **Base URL:** `https://replication.sparkapi.com/Version/3/Reso/OData/`

#### Tags

- RESO
- OData
- MLS
- Property Listings
- Real Estate

#### Properties

- [Documentation](https://sparkplatform.com/docs/reso/overview)
- [API Reference](https://sparkplatform.com/docs/reso/properties)
- [Documentation](https://sparkplatform.com/docs/reso/request_parameters)
- [Documentation](https://sparkplatform.com/docs/reso/reso_replication)
- [Documentation](https://sparkplatform.com/docs/supporting_documentation/reso_dictionary)
- [Authentication](https://sparkplatform.com/docs/authentication/access_token)

### Spark Webhooks

Outbound webhook delivery. When a Property, Member or Office record changes in an upstream MLS, Spark POSTs a RESO Web API Entity Event payload over HTTPS, signed with HMAC-SHA256 in a `Signature` header, with up to 3 retries and a roughly 2-second response timeout. FBS holds a RESO webhooks 1.0.0 certification endorsement for this surface.

- **Human URL:** [https://sparkplatform.com/docs/webhooks/webhooks](https://sparkplatform.com/docs/webhooks/webhooks)

#### Tags

- Webhooks
- RESO
- MLS
- Real Estate

#### Properties

- [Documentation](https://sparkplatform.com/docs/webhooks/webhooks)

## Common Properties

- [Website](https://www.sparkapi.io/)
- [Documentation](https://sparkplatform.com/docs)
- [Sign Up](https://sparkplatform.com/register/developers)
- [GitHub Organization](https://github.com/sparkapi)
- [Authentication](https://sparkplatform.com/docs/authentication/authentication)
- [OpenID Connect Discovery](authentication/spark-platform-openid-configuration.json)
- [JSON Web Key Set](authentication/spark-platform-openid-jwks.json)
- [Terms of Service](https://sparkplatform.com/docs/terms_of_use/developer_agreement_and_terms_of_use)
- [Privacy Policy](https://sparkplatform.com/docs/terms_of_use/privacy)
- [Pricing](https://www.sparkapi.io/developers/)
- [Certification](https://services.reso.org/orgs?showStats=true&showEndorsements=true)

## RESO Posture

- **Certified:** yes, via FBS as the certifying technology provider (RESO UOI `T00000052`, status "Certified Current").
- **Endorsements held by FBS itself:** RESO webhooks 1.0.0 (Certified) and RESO Common Format 2.0 (Certified).
- **Endorsements where FBS is the recorded provider:** 140 organizations (138 MLSs, 1 commercial board, FBS itself) — Web API Core 2.0.0 (115 Certified / 24 Passed), Data Dictionary 1.7 (110 / 19) and Data Dictionary 2.0 (72 / 17).
- **Evidence:** the RESO Organizations and Endorsements feed at `https://services.reso.org/orgs?showStats=true&showEndorsements=true` (HTTP 200, generated 2026-07-26).
- **Reachability:** the live OData service root and the `$metadata` document both return HTTP 401 `Invalid API key and/or request signed improperly`. Certified, not callable.

## Access Gate

- **Classification:** `licence-agreement`.
- Stage one is free and self-serve: a public registration form at `https://sparkplatform.com/register/developers`, reviewed and activated within three business days, yielding demo credentials.
- Stage two is licensed: a signed FBS Developer Agreement, an IDX / VOW / Private role assignment binding the developer to that MLS's rules, and enrolment in an MLS-specific data plan through the Spark Datamart via a "PURCHASE WITH APPROVAL" action the MLS must approve. Where no plan exists, the developer must contact the MLS directly.
- **Published pricing:** a flat 50 USD per month per MLS.
- **Open data:** none. All listing content is licensed MLS Content.

## Maintainers

- Kin Lane — kin@apievangelist.com
