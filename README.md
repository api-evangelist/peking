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

Peking University (北京大学, PKU) is a public research university in Beijing. This repository catalogs its public developer/API footprint as an APIs.json profile, profiled under the API Evangelist **university pipeline**, where every surface carries an `x-operator` saying who actually runs the thing the contract describes. No vendor contract is attributed to Peking University in this repo.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=peking-api-evangelist&utm_content=repo

## Type

- Type: university (Public Research University)
- Position: Consumer
- Access: 3rd-Party

## Tags

University, Higher Education, Education, China, Public Research University, C9 League, Research Repository, Identity Federation, Research Data, Open Data, Research Computing, OAI-PMH

## APIs

All entries below are `x-operator: institution` — Peking University operates them.

- **PKU Institutional Repository REST API** — unauthenticated JSON API over communities, collections, items, Dublin Core metadata, bitstreams and Handle resolution under the repository's own prefix 20.500.11897. Base: `https://ir.pku.edu.cn/rest` — [OpenAPI](openapi/peking-institutional-repository-rest-openapi.yml)
- **PKU Institutional Repository OAI-PMH API** — OAI-PMH 2.0 harvesting, twelve metadata formats, sets per PKU faculty. Base: `https://ir.pku.edu.cn/oai` — [OpenAPI](openapi/peking-institutional-repository-oai-pmh-openapi.yml)
- **PKU Institutional Repository OpenSearch Feed** — OpenSearch 1.1 Atom feed. Base: `https://ir.pku.edu.cn/open-search/`
- **PKU Shibboleth Identity Provider (SAML 2.0 metadata)** — live federated identity metadata, entityID `https://idp.pku.edu.cn/idp/shibboleth`, in eduGAIN production since 2019-06-18.
- **CARSI — CERNET Authentication and Resource Sharing Infrastructure** — China's national research-and-education identity federation, operated by the Peking University Computer Center, full eduGAIN member, registration authority for 1,042 federated entities.
- **OpenSCOW / CraneSched research-computing APIs** — HPC portal and scheduler authored at Peking University, APIs defined in ~40 Protocol Buffer files. Self-hosted software; no public base URL is claimed.
- **PKU Open Research Data Platform (Dataverse REST + OAI-PMH)** — verified live 2026-06-03; unreachable over HTTPS during the 2026-08-19 pass. Marked `x-availability: unreachable`, not removed.

## Artifacts

- OpenAPI: [openapi/](openapi/) (with pristine copies in [openapi/_original/](openapi/_original/))
- JSON Schema: [json-schema/](json-schema/)
- Examples (live captures): [examples/](examples/)
- Authentication: [authentication/peking-authentication.yml](authentication/peking-authentication.yml)
- OAuth Scopes (records an absence): [scopes/peking-scopes.yml](scopes/peking-scopes.yml)
- Conformance: [conformance/peking-conformance.yml](conformance/peking-conformance.yml)
- Errors: [errors/peking-errors.yml](errors/peking-errors.yml)
- Lifecycle: [lifecycle/peking-lifecycle.yml](lifecycle/peking-lifecycle.yml)
- Vocabulary: [vocabulary/peking-vocabulary.yml](vocabulary/peking-vocabulary.yml)
- Plans: [plans/peking-plans-pricing.yml](plans/peking-plans-pricing.yml)
- Rate Limits: [rate-limits/peking-rate-limits.yml](rate-limits/peking-rate-limits.yml)
- FinOps: [finops/peking-finops.yml](finops/peking-finops.yml)

Every artifact carries `generated`, `method` and `source`. Nothing here is credited to Peking University that it did not publish.

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-19

## Common Properties

- Website: https://www.pku.edu.cn/ (English: https://english.pku.edu.cn/)
- Research Repository: https://ir.pku.edu.cn/
- Open Data: https://opendata.pku.edu.cn/
- Identity Federation: https://www.carsi.edu.cn/
- Library: https://lib.pku.edu.cn/
- Course Catalog / registrar: https://dean.pku.edu.cn/
- Research Computing: https://hpc.pku.edu.cn/
- AI Policy (school-level): PKU School of Transnational Law AI Policy, Fall 2024
- GitHub: https://github.com/PKUHPC
- LinkedIn: https://www.linkedin.com/school/peking-university/
- Authentication (gated SSO): https://iaaa.pku.edu.cn/
- Review: [review.yml](review.yml)

## Notes

- No general-purpose institutional developer portal, no published OpenAPI, no `llms.txt` and no `.well-known/security.txt` were found on any Peking University host.
- Two defects were found and recorded rather than smoothed over: an unrecognised OAI-PMH verb returns HTTP 500 instead of the protocol's `badVerb` error element, and `/rest/items/{id}` returns 500 while the same item resolves through `/rest/handle`.
- `opendata.pku.edu.cn` completed TLS on PKU's own certificate and answered a 301 on port 80 but never returned an HTTPS response across seven attempts on 2026-08-19, while every other `pku.edu.cn` host answered normally. Recorded as unreadable from our vantage point, not as absent.
- IAAA is a gated CAS/SSO unified-authentication system, not a public developer API.
- PKUHPC is Peking University's High Performance Computing group; there is no single university-wide official GitHub organisation.
- No endpoints were fabricated. Every status code in this profile came from a probe run on 2026-08-19.

## Maintainers

- Kin Lane — kin@apievangelist.com
