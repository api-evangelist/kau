# King Abdulaziz University (kau)

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

King Abdulaziz University (KAU) is a large public research university in Jeddah, Saudi Arabia, serving over 100,000 students across 30 faculties and institutes including a branch campus at Rabigh. This repository catalogs KAU's public developer/API footprint as an [APIs.json](https://apisjson.org) profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/kau/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=kau-api-evangelist&utm_content=repo

## Type

University / Public Research University / Index

## Tags

University, Higher Education, Education, Research, Open Data, Research Repository, Identity Federation, Learning Management, Saudi Arabia, Middle East

## Who operates what

A university is a federation of buyers, not a producer, so every surface below carries an
operator. `x-operator` says who runs the thing, which for a university is rarely the same
answer as whose name is on it.

### Institution-operated — KAU's own engineering

- **KAU Open Data API** — `https://opendata.kau.edu.sa/api/StudentsData` — aggregate student
  enrollment and graduation counts as JSON, broken down by faculty, department, level, study
  type, gender, nationality and admission cohort. Eight unauthenticated GET invocations
  published by KAU on its own Open Data page, no credential required, no personal data in the
  payload. Specification: [openapi/kau-open-data-api-openapi.yml](openapi/kau-open-data-api-openapi.yml).
- **KAU SAML 2.0 Identity Provider** — `https://iam.kau.edu.sa/oamfed/idp/samlv20` — Oracle
  Access Manager Federation, self-hosted in KAU's own address block with no managed-IdP vendor
  underneath. Detail: [identity-federation/kau-identity-federation.yml](identity-federation/kau-identity-federation.yml).

### Tenant — real relationships, vendor contracts NOT claimed as KAU's

- **KAU Journals on Elsevier Digital Commons** — `kauj.researchcommons.org`, with a working
  OAI-PMH 2.0 data provider back to 2000. The best machine-readable surface associated with this
  university, and it is Elsevier's engineering — `adminEmail` is `dc-support@elsevier.com`.
- **Blackboard Learn** — `lms.kau.edu.sa`, a Blackboard SaaS tenancy in eu-central-1. The Learn
  REST API and LTI endpoints are provisioned and gated.
- **King Abdulaziz Scientific Platform** — `libsp.kau.edu.sa`, an Al Manhal tenancy.

### Registry — memberships, never the registry's contract

- **Crossref** — member 2709 (KAU Scientific Publishing Centre, DOI prefix 10.4197, 1,920 DOIs)
  and member 53473; Funder ID 501100004054.
- **ROR** — [https://ror.org/02ma4wv74](https://ror.org/02ma4wv74), domain kau.edu.sa.

## What KAU does not have

No developer portal. No API key, client registration or self-service onboarding of any kind. No
official GitHub organisation. No KAU-published OpenAPI — the specification here is derived by API
Evangelist from KAU's published endpoints and a real response body. No DataCite account, despite
1,249 DataCite DOIs carrying KAU's ROR as an author affiliation. No ORCID member organisation and
no Shibboleth. And no membership of Maeen, Saudi Arabia's national identity federation, or of
eduGAIN — although 38 Saudi entities including King Saud University, KFUPM, KAUST and King Khalid
University are registered there. KAU runs SAML for itself and does not federate outward.

## Artifacts

- OpenAPI: [openapi/kau-open-data-api-openapi.yml](openapi/kau-open-data-api-openapi.yml) (pristine copy in [openapi/_original/](openapi/_original/))
- JSON Schema: [json-schema/kau-students-data-schema.json](json-schema/kau-students-data-schema.json)
- Vocabulary: [vocabulary/kau-open-data-vocabulary.yml](vocabulary/kau-open-data-vocabulary.yml)
- Examples: [examples/index.yml](examples/index.yml)
- Authentication: [authentication/kau-authentication.yml](authentication/kau-authentication.yml)
- Conformance (`education` regime): [conformance/kau-conformance.yml](conformance/kau-conformance.yml)
- Identity federation: [identity-federation/kau-identity-federation.yml](identity-federation/kau-identity-federation.yml)
- Plans & Pricing: [plans/kau-plans-pricing.yml](plans/kau-plans-pricing.yml)
- Rate Limits: [rate-limits/kau-rate-limits.yml](rate-limits/kau-rate-limits.yml)
- FinOps: [finops/kau-finops.yml](finops/kau-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Common Properties

- Website: https://www.kau.edu.sa/en
- Open Data: https://www.kau.edu.sa/page/open-data
- Research Repository (tenant): https://kauj.researchcommons.org/
- Library / Discovery (tenant): https://libsp.kau.edu.sa/
- LinkedIn: https://www.linkedin.com/school/king-abdulaziz-university
- Twitter/X: https://x.com/kauedu_sa

## Notes

Re-profiled 2026-09-01 under the API Evangelist university pipeline. The 2026-06-03 profile
described KAU's Open Data page as an empty beta placeholder with no datasets or endpoints; that
was wrong, and the correction is the main result of this pass.

Every host in KAU's self-hosted `192.162.72.0/24` block — `opendata`, `sso`, `iam`, `research`,
`journals` — refused connections on 443 from two independent network egresses during this run,
while KAU's CloudFront-fronted `www` host and all three vendor tenancies answered normally. That
pattern reads as a geographic restriction on KAU's own estate, not a dead service and not a block
on us. The SAML IdP was proven live indirectly, by a signed AuthnRequest KAU's own Blackboard
tenancy generated during the run. The Open Data API's last verified HTTP 200 is an Internet
Archive capture of 2025-04-17 returning 1,886 records, corroborated by seven further 200 captures
across 2024; artifacts derived from it are marked `derived`, not probed-live.

Separately, the dataset downloads KAU links from its own Open Data page are broken: every
`GetFile.aspx` URL returns 404 after the site's migration to Next.js. The spreadsheet half of the
open data programme is dead while the API half is not.

No endpoints, datasets, credentials or conformances were fabricated, and no vendor contract is
saved under this institution's name.

## Maintainers

- Kin Lane — kin@apievangelist.com
