# University of Sussex (university-of-sussex)

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
