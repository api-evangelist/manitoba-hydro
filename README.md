# Manitoba Hydro (manitoba-hydro)

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

Manitoba Hydro is the provincial Crown corporation that generates, transmits, and distributes electricity and distributes natural gas across Manitoba, Canada — "Manitoba's publicly owned electricity and natural gas supplier" in its own words, serving 632,117 electric customers and 300,789 natural gas customers, and trading electricity into wholesale markets across the Midwestern U.S. and Canada. It is a vertically integrated monopoly in a province with no retail competition and no consumer energy data mandate: Ontario's Green Button regulation (O. Reg. 633/21) binds Ontario distributors only, Australia's Consumer Data Right does not reach Canada, and the Green Button Alliance states plainly that it has "no information about Green Button deployments in Manitoba." Manitoba Hydro also has no advanced metering infrastructure — its 2006–2009 smart meter pilot was not continued — so there is no interval consumption data for a consumer API to serve in the first place. The API posture is therefore the inverse of a mandated utility: consumer data is entirely closed, reachable only by the customer through a login, while grid and system data is genuinely open and anonymous — public ArcGIS REST and OGC WFS 2.0.0 outage layers refreshed every five minutes, an on-domain ArcGIS Server directory, and a live hydrological monitoring feed. None of it is documented as an API. There is no developer portal, no API keys, and no OpenAPI.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/manitoba-hydro/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/manitoba-hydro/refs/heads/main/apis.yml)

## Tags

- Energy
- Canada
- Utilities
- Electricity
- Gas
- Hydroelectric
- Grid
- Outage Data
- Open Data
- Crown Corporation

## Timestamps

- **Created:** 2026-07-27
- **Modified:** 2026-07-27

## APIs

### Manitoba Hydro Current Power Outages

A hosted Esri feature service published by Manitoba Hydro's ArcGIS Online organization (org id `QoeQkfdOG126FqSi`, org name "Manitoba Hydro", item owner `dcarpenter@hydro.mb.ca`) carrying live unplanned power outage polygons. The item is shared publicly and was queried anonymously with no key, token, or registration — an anonymous `returnCountOnly` query returned 8 active outages at review time. Layer 0 "MH Current Power Outages" exposes `OUTAGE_ID`, `OUTAGE_TYPE`, `TIME_OF_OUTAGE`, `NUM_CUST_NOPOWER`, `ETR`, `CAUSE`, `SUBCAUSE`, `CREW_STATUS` and `DATA_LAST_UPDATE`. Service capabilities are Query only. The same data is also published as an OGC WFS 2.0.0 endpoint. Manitoba Hydro publishes no documentation, terms of use, or rate limits for this surface.

- **Human URL:** [https://www.arcgis.com/home/item.html?id=607ef103b2934e3fbbbc7b05c4c3df34](https://www.arcgis.com/home/item.html?id=607ef103b2934e3fbbbc7b05c4c3df34)
- **Base URL:** `https://services2.arcgis.com/QoeQkfdOG126FqSi/arcgis/rest/services/Manitoba_Hydro_Current_Power_Outages/FeatureServer`

#### Tags

- Outage Data
- Grid
- Electricity
- Geospatial
- ArcGIS REST
- WFS

#### Properties

- [API Reference](https://services2.arcgis.com/QoeQkfdOG126FqSi/arcgis/rest/services/Manitoba_Hydro_Current_Power_Outages/FeatureServer?f=json)
- [API Reference — OGC WFS 2.0.0 GetCapabilities](https://dservices2.arcgis.com/QoeQkfdOG126FqSi/arcgis/services/Manitoba_Hydro_Current_Power_Outages_WFS/WFSServer?service=wfs&request=getcapabilities)
- [Documentation — ArcGIS item](https://www.arcgis.com/home/item.html?id=607ef103b2934e3fbbbc7b05c4c3df34)
- [Documentation — WFS item](https://www.arcgis.com/home/item.html?id=9cd3470a9a8c428185a768dbcc217ce3)
- [Documentation — consumer outage map](https://www.hydro.mb.ca/outages/outage-map/)
- [Standard — OGC WFS](https://www.ogc.org/standards/wfs/)

### Manitoba Hydro Planned Power Outages

A hosted Esri feature service carrying planned outage areas. The item description states the layer "contains planned power outages and the area that will be impacted. Attributes include the scheduled start and end date/time for each outage. This data is updated every 5 minutes." Queried anonymously with no credentials, an unfiltered count returned 48 planned outages at review time. A parallel OGC WFS 2.0.0 endpoint is published for the same layer. No licence or terms of use is attached to the item.

- **Human URL:** [https://www.arcgis.com/home/item.html?id=016914ea3b28449e8205e07c04a92d51](https://www.arcgis.com/home/item.html?id=016914ea3b28449e8205e07c04a92d51)
- **Base URL:** `https://services2.arcgis.com/QoeQkfdOG126FqSi/arcgis/rest/services/Manitoba_Hydro_Planned_Power_Outages/FeatureServer`

#### Tags

- Outage Data
- Grid
- Electricity
- Geospatial
- ArcGIS REST
- WFS

#### Properties

- [API Reference](https://services2.arcgis.com/QoeQkfdOG126FqSi/arcgis/rest/services/Manitoba_Hydro_Planned_Power_Outages/FeatureServer?f=json)
- [API Reference — OGC WFS 2.0.0 GetCapabilities](https://dservices2.arcgis.com/QoeQkfdOG126FqSi/arcgis/services/Manitoba_Hydro_Planned_Power_Outages_WFS/WFSServer?service=wfs&request=getcapabilities)
- [Documentation — ArcGIS item](https://www.arcgis.com/home/item.html?id=016914ea3b28449e8205e07c04a92d51)
- [Documentation — WFS item](https://www.arcgis.com/home/item.html?id=4cc075a46e574c15816b28b93a1f2de3)
- [Documentation — planned outages page](https://www.hydro.mb.ca/outages/planned/)
- [Standard — OGC WFS](https://www.ogc.org/standards/wfs/)

### Manitoba Hydro ArcGIS Server Reference Data

An ArcGIS Server 10.91 REST services directory hosted on Manitoba Hydro's own domain at `maps.hydro.mb.ca`, readable anonymously. The root listing returned nine folders (ARL, ConTrack, DISTAPPS, GDS, JUTA, LEA, Locators, ReferenceData, Utilities); most are empty to an anonymous caller, but `ReferenceData/MH_AdminBoundaries` is fully readable and exposes three query-capable layers — `MH_CustomerServiceCentres` (19 features), `MH_LocateAreas` and `MH_StationAreas`. The site root itself returns HTTP 403; only the `/arcgis/rest/services` tree responds. Recorded here because it is a real, on-domain, anonymously queryable API surface, not because it is offered as one.

- **Human URL:** [https://maps.hydro.mb.ca/arcgis/rest/services?f=json](https://maps.hydro.mb.ca/arcgis/rest/services?f=json)
- **Base URL:** `https://maps.hydro.mb.ca/arcgis/rest/services`

#### Tags

- Geospatial
- ArcGIS REST
- Reference Data
- Grid

#### Properties

- [API Reference — services directory](https://maps.hydro.mb.ca/arcgis/rest/services?f=json)
- [API Reference — MH_AdminBoundaries](https://maps.hydro.mb.ca/arcgis/rest/services/ReferenceData/MH_AdminBoundaries/FeatureServer?f=json)

### Manitoba Hydro Hydrological Data

Manitoba Hydro's near-real-time hydrological monitoring application, a KISTERS WISKI Web Public deployment documented on hydro.mb.ca. The application is documented for humans; its data files are not documented at all, but they are served anonymously as JSON and were verified live — station metadata (169 gauging stations), a layer index of 15 monitored parameters (Water Level, Water Temperature, Air Temperature, Precipitation, Snow Depth, wind speed/direction/gust/peak variants, Relative Humidity, Atmospheric Pressure), and per-parameter observation files. The Water Level file returned 158 stations with readings timestamped the same day as this review. Manitoba Hydro states the data are "preliminary and are being transmitted automatically without verification or review for quality assurance." There is no API documentation, no versioning, and no stated licence. An older parallel tree at `/hydrologicalData/data/` is still served but is frozen at February 2021 readings.

- **Human URL:** [https://www.hydro.mb.ca/corporate/operations/water-levels/hydrological-data/](https://www.hydro.mb.ca/corporate/operations/water-levels/hydrological-data/)
- **Base URL:** `https://www.hydro.mb.ca/hydrologicalData/static/data/`

#### Tags

- Hydrology
- Water Levels
- Hydroelectric
- Open Data
- Monitoring

#### Properties

- [Documentation](https://www.hydro.mb.ca/corporate/operations/water-levels/hydrological-data/)
- [Documentation — water levels & flows](https://www.hydro.mb.ca/corporate/operations/water-levels/)
- [Portal — hydrological data application](https://www.hydro.mb.ca/hydrologicalData/static/)
- [API Reference — station metadata](https://www.hydro.mb.ca/hydrologicalData/static/data/stationdata.json)
- [API Reference — parameter index](https://www.hydro.mb.ca/hydrologicalData/static/data/tsdata.json)

## Common Properties

- [Website](https://www.hydro.mb.ca/)
- [About](https://www.hydro.mb.ca/corporate/)
- [Documentation](https://www.hydro.mb.ca/corporate/operations/water-levels/hydrological-data/)
- [Terms of Service](https://www.hydro.mb.ca/terms-of-use/)
- [Sign Up / Customer Login](https://account.hydro.mb.ca/Portal)
- [Contact Us](https://www.hydro.mb.ca/support/contact/)
- [Security](https://www.hydro.mb.ca/.well-known/security.txt)
- [LinkedIn](https://www.linkedin.com/company/manitoba-hydro)
- [Blog](https://www.hydro.mb.ca/articles/)

## Mandate & Data Posture

| Dimension | Finding |
| --- | --- |
| Mandate regime | `none` — no Manitoba or Canadian federal consumer energy data right |
| Mandate status | `none` — nothing designated, nothing claimed, nothing to verify |
| Data standard | No energy data standard. OGC WFS 2.0.0 and Esri ArcGIS REST for geospatial only |
| Consumer data API | **No** — customer login only, at `account.hydro.mb.ca` |
| Open market/grid data | **Yes** — anonymous ArcGIS REST + OGC WFS outage layers and live hydrological JSON |
| Access gate | `self-serve` — in practice fully anonymous; no key, no signup, no terms |
| Auth model | None on the open surfaces; username/password on the customer portal |
| Developer portal | None |
| OpenAPI harvested | None exists |

Ontario's Green Button regulation binds Ontario distributors and does not reach Manitoba. Australia's CDR is Australian law. The Green Button Alliance's Canadian Initiatives page states verbatim: "We currently have no information about Green Button deployments in Manitoba, New Brunswick, Newfoundland and Labrador, Prince Edward Island, Quebec, or Saskatchewan." Manitoba Hydro's own 2022 article confirms "Manitoba doesn't have AMI right now." See [`review.yml`](review.yml) for every probe, HTTP status, and quotation behind these findings.

## Maintainers

- Kin Lane — kin@apievangelist.com
