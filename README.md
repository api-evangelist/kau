# King Abdulaziz University (kau)

King Abdulaziz University (KAU) is a large public research university in Jeddah, Saudi Arabia, ranked #149 in the QS World University Rankings 2025, serving over 100,000 students across 33+ faculties and institutes. This repository catalogs KAU's public developer/API footprint as an [APIs.json](https://apisjson.org) profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/kau/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=kau-api-evangelist&utm_content=repo

## Type

Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, Saudi Arabia, Middle East

## APIs

- **KAU Single Sign-On / Identity Federation** — Institutional SSO portal (sso.kau.edu.sa) and Oracle Access Manager federation login (iam.kau.edu.sa/oamsso-bin/login-fed.pl). Gated institutional identity service, not a publicly documented developer API. Docs: https://www.kau.edu.sa/en

No openly documented, self-service developer API, API reference, or developer portal was found for KAU. The institution's "Open Data" page exists but is a beta placeholder with no datasets or endpoints.

## Plans, Rate Limits, FinOps

- Plans & Pricing: [plans/kau-plans-pricing.yml](plans/kau-plans-pricing.yml)
- Rate Limits: [rate-limits/kau-rate-limits.yml](rate-limits/kau-rate-limits.yml)
- FinOps: [finops/kau-finops.yml](finops/kau-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.kau.edu.sa/en
- Developer Portal (Open Data, beta): https://www.kau.edu.sa/page/open-data
- LinkedIn: https://www.linkedin.com/school/king-abdulaziz-university
- Twitter/X: https://x.com/kauedu_sa
- Authentication (SSO): https://sso.kau.edu.sa/

## Notes

Findings were verified via web search and live fetching where possible. The official website (kau.edu.sa) and its beta Open Data page were confirmed live (HTTP 200). The library portal, scientific platform, SSO, and IAM federation hosts exist per search results but could not be fetched live from the review environment (connection refused / 403 / timeout); their statuses are recorded as 0 in the review where they did not resolve. No API endpoints, datasets, or developer credentials were fabricated. No official KAU GitHub organization exists — only a student-run Google Developer Student Club and individual academic projects appear on GitHub.

## Maintainers

- Kin Lane — kin@apievangelist.com
