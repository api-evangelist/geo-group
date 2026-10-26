# The GEO Group

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
