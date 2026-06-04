# University of Sussex (university-of-sussex)

The University of Sussex is a research-intensive public university near Brighton, United Kingdom, ranked #247 in the QS World University Rankings 2025. This repository catalogs the institution's public developer and API footprint as an APIs.json provider profile.

- APIs.json: [apis.yml](https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/apis.yml)
- Run with Naftiko: [naftiko/fleet](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-sussex-api-evangelist&utm_content=repo)

## Type

- Index / Consumer / 3rd-Party

## Tags

- Education
- Higher Education
- University
- Research
- Open Access
- United Kingdom

## APIs

- **University of Sussex Research Repository (Figshare)** — Research outputs (publications, data, theses, artefacts) hosted on Figshare, accessible via the public Figshare v2 REST API. Docs: [docs.figshare.com](https://docs.figshare.com/) · Portal: [sussex.figshare.com](https://sussex.figshare.com/)
- **University of Sussex Single Sign-On (Okta)** — Okta-based OAuth2 / OpenID Connect identity and access management for university applications. Gated to staff/students. Docs: [sussex.ac.uk/its/services/sso](https://www.sussex.ac.uk/its/services/sso)

## Plans

- [plans/university-of-sussex-plans-pricing.yml](plans/university-of-sussex-plans-pricing.yml)

## Rate Limits

- [rate-limits/university-of-sussex-rate-limits.yml](rate-limits/university-of-sussex-rate-limits.yml)

## FinOps

- [finops/university-of-sussex-finops.yml](finops/university-of-sussex-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.sussex.ac.uk/
- GitHub: https://github.com/universityofsussex (exists, no public repositories)
- LinkedIn: https://www.linkedin.com/school/university-of-sussex/

## Notes

- Verification discipline: only APIs and properties confirmed live are listed; nothing fabricated.
- The Figshare research repository portal and the public Figshare v2 REST API host (`api.figshare.com/v2`) are live; the API host returns HTTP 400 on a deliberately malformed query, confirming it is responding.
- The former Sussex Research Online EPrints OAI-PMH endpoint (`sro.sussex.ac.uk/cgi/oai2`) is decommissioned and now redirects (HTTP 301) to a non-OAI HTML publications page that points to Figshare.
- Okta SSO is gated to staff/students with @sussex.ac.uk credentials and is not an openly documented third-party developer API.
- No public course/timetable/SIS or open-data developer API was confirmed.

## Maintainers

- Kin Lane — kin@apievangelist.com
