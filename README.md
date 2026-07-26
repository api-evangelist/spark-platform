# Spark Platform (spark-platform)

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
