# Manitoba Hydro

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

Manitoba Hydro is the provincial Crown corporation that generates, transmits, and distributes electricity and distributes natural gas across Manitoba, Canada — "Manitoba's publicly owned electricity and natural gas supplier" in its own words, serving 632,117 electric customers and 300,789 natural gas customers, and trading electricity into wholesale markets across the Midwestern U.S. and Canada. It is a vertically integrated monopoly in a province with no retail competition, no independent system operator of its own, and no consumer energy data mandate: Ontario's Green Button regulation (O. Reg. 633/21) binds Ontario distributors only, Australia's Consumer Data Right does not reach Canada, and the Green Button Alliance states plainly that it has "no information about Green Button deployments in Manitoba." Manitoba Hydro also has no advanced metering infrastructure — its 2006-2009 smart meter pilot was not continued — so there is no interval consumption data for a consumer API to serve in the first place. The API posture is therefore the inverse of a mandated utility: consumer data is entirely closed, reachable only by the customer through a login at account.hydro.mb.ca, while grid and system data is genuinely open and anonymous. Manitoba Hydro runs a public ArcGIS Online organization whose current and planned power outage layers are queryable without a key over both the Esri ArcGIS REST API and OGC WFS 2.0.0, refreshed every five minutes; an on-domain ArcGIS Server REST directory at maps.hydro.mb.ca; and a live KISTERS hydrological monitoring application whose station and time-series JSON at hydro.mb.ca is served anonymously and was observed carrying same-day readings. None of it is documented as an API. There is no developer portal, no API keys, no OpenAPI, and no terms of use for data reuse — the open surface exists as a by-product of public map publishing rather than as an API program.

**Areas:** Energy · Canada · Utilities · Electricity · Gas · Hydroelectric · Grid · Outage Data · Open Data · Crown Corporation

## Manitoba Hydro on APIs.io

Everything profiled for Manitoba Hydro is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/manitoba-hydro/](https://apis.io/providers/manitoba-hydro/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Manitoba Hydro Current Power Outages](https://apis.io/apis/manitoba-hydro/manitoba-hydro-current-power-outages/) — A hosted Esri feature service published by Manitoba Hydro's ArcGIS Online organization (org id QoeQkfdOG126FqSi, org name "Manitoba Hydro", item owner…
- [Manitoba Hydro Planned Power Outages](https://apis.io/apis/manitoba-hydro/manitoba-hydro-planned-power-outages/) — A hosted Esri feature service published by the same Manitoba Hydro ArcGIS Online organization carrying planned outage areas. The item description states the…
- [Manitoba Hydro ArcGIS Server Reference Data](https://apis.io/apis/manitoba-hydro/manitoba-hydro-arcgis-server-reference-data/) — An ArcGIS Server 10.91 REST services directory hosted on Manitoba Hydro's own domain at maps.hydro.mb.ca, readable anonymously. The root listing returned…
- [Manitoba Hydro Hydrological Data](https://apis.io/apis/manitoba-hydro/manitoba-hydro-hydrological-data/) — Manitoba Hydro's near-real-time hydrological monitoring application, a KISTERS WISKI Web Public deployment documented on hydro.mb.ca and reachable at…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### JSON Schema (6)

The data models the API reads and writes.

- [Manitoba Hydro — MH Current Power Outages (feature attributes)](https://apis.io/schemas/manitoba-hydro/manitoba-hydro-current-power-outages.schema/)
- [Manitoba Hydro — MH Customer Service Centres (feature attributes)](https://apis.io/schemas/manitoba-hydro/manitoba-hydro-customer-service-centres.schema/)
- [Manitoba Hydro — hydrological parameter observation file (KISTERS WISKI Web Public)](https://apis.io/schemas/manitoba-hydro/manitoba-hydro-hydrological-timeseries.schema/)
- [Manitoba Hydro — MH Locate Areas (feature attributes)](https://apis.io/schemas/manitoba-hydro/manitoba-hydro-locate-areas.schema/)
- [Manitoba Hydro — MH Planned Power Outages (feature attributes)](https://apis.io/schemas/manitoba-hydro/manitoba-hydro-planned-power-outages.schema/)
- [Manitoba Hydro — MH Station Areas (feature attributes)](https://apis.io/schemas/manitoba-hydro/manitoba-hydro-station-areas.schema/)

#### Examples (6)

Example requests and responses.

- [Manitoba Hydro Arcgis Error Response](https://apis.io/examples/manitoba-hydro/manitoba-hydro-arcgis-error-response/)
- [Manitoba Hydro Current Power Outages Layer Metadata](https://apis.io/examples/manitoba-hydro/manitoba-hydro-current-power-outages-layer-metadata/)
- [Manitoba Hydro Current Power Outages Query Response](https://apis.io/examples/manitoba-hydro/manitoba-hydro-current-power-outages-query-response/)
- [Manitoba Hydro Hydrological Parameter Index](https://apis.io/examples/manitoba-hydro/manitoba-hydro-hydrological-parameter-index/)
- [Manitoba Hydro Planned Power Outages Layer Metadata](https://apis.io/examples/manitoba-hydro/manitoba-hydro-planned-power-outages-layer-metadata/)
- [Manitoba Hydro Planned Power Outages Query Response](https://apis.io/examples/manitoba-hydro/manitoba-hydro-planned-power-outages-query-response/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Manitoba Hydro Authentication](https://apis.io/security/manitoba-hydro/manitoba-hydro-authentication/)
- [Manitoba Hydro Domain Security](https://apis.io/security/manitoba-hydro/manitoba-hydro-domain-security/)
- [Manitoba Hydro Vulnerability Disclosure](https://apis.io/security/manitoba-hydro/manitoba-hydro-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.hydro.mb.ca/)
- [Documentation](https://www.hydro.mb.ca/corporate/operations/water-levels/hydrological-data/)
- [Sign up](https://account.hydro.mb.ca/Portal)
- [Support](https://www.hydro.mb.ca/support/)
- [Blog](https://www.hydro.mb.ca/articles/)
- [Security](https://www.hydro.mb.ca/.well-known/security.txt)
- [Terms of service](https://www.hydro.mb.ca/terms-of-use/)
- [Privacy policy](https://www.hydro.mb.ca/terms-of-use/#privacy)

## API Evangelist rating

**Kin Score 31.9** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 15.2 |
| Contract governance | 18.2 |
| Operational transparency | 10.5 |
| Developer ergonomics | 45.2 |
| Access clarity | 34.2 |

**Agent readiness 4.5** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 23.4** — Energy & Utilities

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/manitoba-hydro/](https://apis.io/providers/manitoba-hydro/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Manitoba Hydro: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/manitoba-hydro/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
