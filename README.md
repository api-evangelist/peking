# Peking University (peking)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Peking University (PKU) is a major public research university in Beijing, China, ranked #25 in the QS World University Rankings 2025. This repository catalogs its public developer/API footprint as an APIs.json profile. The clearest public, machine-readable surface is the Dataverse-based PKU Open Research Data Platform, which exposes a native REST API and a live OAI-PMH 2.0 endpoint.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=peking-api-evangelist&utm_content=repo

## Type

- Type: Index
- Position: Consumer
- Access: 3rd-Party

## Tags

Education, Higher Education, University, Research Data, Open Data, China

## APIs

- **PKU Open Research Data Platform (Dataverse REST API)** — Native Dataverse REST API for dataverses, datasets, and files. Docs: https://guides.dataverse.org/en/latest/api/ — Platform: https://opendata.pku.edu.cn/
- **PKU Open Research Data Platform (OAI-PMH)** — Live OAI-PMH 2.0 metadata harvesting endpoint (base `https://opendata.pku.edu.cn/oai`). Docs: https://guides.dataverse.org/en/latest/api/oai.html

## Plans / Rate Limits / FinOps

- Plans: [plans/peking-plans-pricing.yml](plans/peking-plans-pricing.yml)
- Rate Limits: [rate-limits/peking-rate-limits.yml](rate-limits/peking-rate-limits.yml)
- FinOps: [finops/peking-finops.yml](finops/peking-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://english.pku.edu.cn/
- GitHub: https://github.com/PKUHPC
- LinkedIn: https://www.linkedin.com/school/peking-university/
- Authentication (gated SSO): https://iaaa.pku.edu.cn/
- Source Code (Dataverse customization): https://github.com/pengchengluo/Peking-University-Open-Research-Data-Platform
- Review: [review.yml](review.yml)

## Notes

- No general-purpose institutional developer portal was found at review time.
- The OAI-PMH Identify verb was verified live (HTTP 200). The Dataverse REST `/api/info/version` path returned HTTP 403 to the review fetcher (likely user-agent/WAF filtering), which does not confirm absence; the REST surface is documented upstream by the Dataverse project.
- IAAA is a gated CAS/SSO unified-authentication system, not a public developer API.
- PKUHPC is a real, verified PKU-affiliated GitHub organization (High Performance Computing Platform); there is no single university-wide official GitHub org. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
