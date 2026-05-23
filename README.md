# The GEO Group

The GEO Group, Inc. (NYSE: **GEO**) is a publicly traded private corrections and community supervision company headquartered in Boca Raton, Florida. Founded in 1984 as Wackenhut Corrections Corporation (WCC), the company rebranded to its current name in 2004 after management repurchased the holdings of G4S. As of September 2024, GEO Group "owned or managed 80,000 beds at 99 facilities, making it the largest prison operator in the United States" and reported $2.424 billion in revenue for fiscal year 2024 (Wikipedia, GEO Group). The company also operates internationally in Australia, the United Kingdom and South Africa, and its own corporate site reports 95 facilities worldwide and approximately 20,000 employees (geogroup.com).

This repository is part of the [API Evangelist Network](https://github.com/api-evangelist). It exists to document a major federal contractor's complete absence of a public API surface, in line with the network's coverage of sensitive sectors where opacity is itself a policy choice.

## What GEO Group does

GEO operates through two primary divisions and a technology subsidiary:

- **GEO Secure Services** designs, builds, finances and operates secure correctional and ICE detention facilities under contracts with federal, state and international government agencies. In 2019, federal-government agencies generated 53% of the company's revenue.
- **GEO Care** delivers community-based residential reentry, "temporary housing, cognitive behavioral treatment, substance abuse treatment," electronic monitoring, and post-release case-management services. The corporate website reports approximately 31,500 daily participants in evidence-based programs.
- **GEO Transport Inc.** provides secure detainee and inmate transportation, including ICE removal staging.
- **BI Incorporated**, acquired by GEO in 2011, is the electronic-monitoring technology subsidiary and the operator of ICE's Intensive Supervision Appearance Program (ISAP).

## BI Incorporated — the technology arm

BI Incorporated, headquartered in Boulder, Colorado, is GEO's electronic-monitoring subsidiary and the primary contractor for ICE's ISAP program. Its product portfolio is the closest thing GEO Group has to a "platform," but it is sold to supervising agencies, not to developers, and none of it exposes a documented public API:

| Product | Function |
|---|---|
| **BI VeriWatch 2** | Wrist-worn GPS device with "one minute location acquisition" |
| **BI SmartLINK** | Smartphone monitoring app for supervised clients, used widely in ISAP |
| **BI SmartBAND 1.0** | Bluetooth Low Energy wearable paired with SmartLINK as a "wireless tether" |
| **BI HomeGuard 20\|20** | Radio-frequency home monitoring base/anklet system |
| **BI SoberTech** | Handheld alcohol-detection breathalyzer |
| **BI TotalAccess** | Officer case-management web platform "consolidating data in one online platform" |
| **BI Agency Assist** | Centralized administrative back-office for probation and parole agencies |

People supervised on ISAP interact with GEO's software whether or not they consented in any meaningful sense; supervising officers interact with BI TotalAccess. There is no third-party developer API, no OpenAPI spec, no SDK, no GitHub organization, and no public schema for any of this telemetry.

## API surface — none

| Surface | Status |
|---|---|
| Public developer API | **None** |
| OpenAPI / AsyncAPI spec | **None** |
| GitHub organization | **None** (the GitHub handle `geogroup` belongs to an unrelated Chinese academic researcher) |
| SDKs / CLIs | **None** |
| Inmate / detainee locator API | **None** (contrast: U.S. Bureau of Prisons publishes a web inmate locator) |
| Facility data feed | **None** |
| Status page | **None** |
| Public changelog | **None** |
| Webhooks | **None** |
| RSS / Atom feed | **None** beyond press-release page |

Because there is no real machine-readable surface, this repository contains only `apis.yml` and this README. No `openapi/`, `capabilities/`, `json-schema/`, `examples/`, `rules/`, `plans/`, `rate-limits/` or `finops/` directories are present, per the API Evangelist Network rule against placeholder artifacts.

## Why this profile exists — the controversy ledger

GEO Group is a publicly-listed firm whose revenue depends almost entirely on federal and state incarceration and immigration-detention contracts. Documenting it in the API Evangelist Network is a deliberate choice: in 2025+ the U.S. federal government has dramatically expanded ICE detention capacity, and GEO is one of the two firms (alongside CoreCivic) absorbing that expansion. The absence of an API is not a neutral fact; it is the operating condition that lets a private operator hold tens of thousands of people in federal custody without machine-readable accountability.

Documented controversies (sourced from Wikipedia's GEO Group article and contemporary reporting):

- **Detainee labor / wage litigation (Washington State).** A jury awarded detainees at the Northwest ICE Processing Center in Tacoma "$17.3 million" in compensation and the State of Washington "$5.9 million" over violations of state minimum-wage law in the facility's "Voluntary Work Program" (where ICE detainees were paid $1/day).
- **Threats of solitary for refusing unpaid work.** A 2014 lawsuit alleged immigrant detainees were "threatened with solitary confinement if they refused to work without pay," later expanding into class-action litigation covering roughly 60,000 current and former detainees.
- **Walnut Grove / Mississippi.** GEO lost Mississippi contracts following a 2012 settlement over conditions at Walnut Grove Youth Correctional Facility, with related federal investigations examining "kickback and bribery schemes."
- **Deaths in custody.** Multiple in-custody deaths at GEO-operated ICE facilities (including Adelanto, CA and the Northwest ICE Processing Center) have prompted DHS Office of Inspector General reports and federal lawsuits over inadequate medical care.
- **Trump 2.0 expansion.** In February 2025 GEO announced plans to reopen **Delaney Hall** in Newark, New Jersey, as an ICE detention facility with capacity for 1,000 people — one of the first publicly announced reactivations under the second Trump administration's mass-detention buildout.
- **ISAP scale.** Through BI Incorporated, GEO operates the federal program that places tens of thousands of immigrants on ankle monitors, GPS, voice verification or the SmartLINK app while their cases proceed — a parallel surveillance footprint to physical detention, again with no public reporting API.
- **Lobbying and political donations.** GEO has been a consistent direct corporate donor to federal campaigns and a sustained federal lobbying spender — atypical for a firm of its size and a longstanding focus of divestment campaigns.

## Structure of this repository

```
geo-group/
├── apis.yml      ← Index entry for the API Evangelist Network
└── README.md     ← This file
```

No artifact subfolders are present, because GEO Group publishes no machine-readable artifacts. If that ever changes — if GEO or BI ever publishes an OpenAPI spec for a customer-facing portal, or if an ICE detention-data API is mandated by Congress — this repository will be the place to land it.

## Sources

- The GEO Group corporate site — https://www.geogroup.com
- The GEO Group "About Us" — https://www.geogroup.com/About-Us
- BI Incorporated — https://bi.com
- Wikipedia: The GEO Group — https://en.wikipedia.org/wiki/GEO_Group

## Maintainer

Kin Lane — [kin@apievangelist.com](mailto:kin@apievangelist.com)
