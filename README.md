# Regrid (regrid)

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

Regrid is a national land parcel data platform providing REST APIs for querying parcel boundaries, ownership, zoning, assessed values, and deed records across all US counties and Canadian provinces. The platform delivers structured GeoJSON parcel data through a suite of APIs covering parcel search by location, address, APN, owner, and polygon area, as well as tile map services, building footprints, standardized zoning, and daily ownership updates. Self-serve monthly subscriptions are available in Standard and Premium schema tiers, with enterprise custom packages offered for bulk and high-volume use cases.

- APIs.json: [https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/apis.yml)
- Naftiko: [https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=regrid-api-evangelist&utm_content=repo](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=regrid-api-evangelist&utm_content=repo)

## Tags

- Parcels
- Land Data
- Property Data
- GeoJSON
- Real Estate
- Zoning
- Ownership
- Geospatial
- Mapping
- Tiles

## APIs

| Name | Description |
|------|-------------|
| Regrid Parcel API | RESTful API for querying US and Canadian parcel records by location, address, APN, owner, or polygon. Returns GeoJSON with boundaries, ownership, zoning, and deed attributes. |
| Regrid Tile API | Tile Map Service (TMS) delivering interactive vector and raster map layers of the full Regrid parcel dataset. |
| Regrid Matched Building Footprints API | Building footprint geometries matched to parcel records, including square footage and building count. |
| Regrid Standardized Zoning API | Standardized zoning data and classifications for major US metro areas, matched to parcel records. |
| Regrid Daily Ownership Updates API | Current owner information and deeded property details with daily refresh cycles. |

## Plans / Rate Limits / FinOps

| Resource | File |
|----------|------|
| Plans & Pricing | [plans/regrid-plans-pricing.yml](plans/regrid-plans-pricing.yml) |
| Rate Limits | [rate-limits/regrid-rate-limits.yml](rate-limits/regrid-rate-limits.yml) |
| FinOps | [finops/regrid-finops.yml](finops/regrid-finops.yml) |

**Plans:** Free 30-day sandbox trial; Standard Schema (monthly, metered by parcel records); Premium Schema (adds footprints, zoning, USPS flags, Esri enrichments); Enterprise (custom volume/delivery).

**Rate Limits:** 10 concurrent requests per token; approximately 200 requests per minute; up to 1,000 parcel records per request (default 20). HTTP 429 returned on throttle.

**FinOps:** Hybrid billing model — fixed monthly base price covering an included parcel record allocation, with per-record overage charges above the threshold. Monthly spend caps and usage alerts available via account dashboard.

## Timestamps

- Created: 2026-06-12
- Modified: 2026-06-12

## Common Properties

| Type | URL |
|------|-----|
| Website | https://regrid.com |
| Documentation | https://support.regrid.com/api/section/parcel-api |
| Pricing | https://app.regrid.com/api/plans |
| Blog | https://regrid.com/blog |
| Status Page | https://status.regrid.com/ |
| LinkedIn | https://www.linkedin.com/company/regridapp |
| X | https://x.com/regridapp |

## Maintainers

- **Kin Lane** / kin@apievangelist.com
