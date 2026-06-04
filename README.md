# Peking University (peking)

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
