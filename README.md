# Regrid (regrid)

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
