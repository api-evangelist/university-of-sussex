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

The University of Sussex is a research-intensive public university at Falmer near Brighton, United Kingdom, ranked #247 in the QS World University Rankings 2025. This repository catalogs the institution's public developer and API footprint as an APIs.json provider profile.

- APIs.json: [apis.yml](https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/apis.yml)
- Run with Naftiko: [naftiko/fleet](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-sussex-api-evangelist&utm_content=repo)

## Type

- university / Public Research University / Index / Consumer / 3rd-Party

## Tags

- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Public Research University
- Identity Federation
- Research Repository
- Library
- Learning Management
- Research
- Open Access

## Who operates what

Every surface below carries an operator. `institution` means Sussex runs the thing the contract
describes. `tenant` means Sussex owns the account and the data but a vendor wrote the contract and
runs the platform — the contract is scored against that vendor's own profile, not against Sussex.

| Surface | Operator | Evidence |
|---|---|---|
| [Shibboleth IdP SAML 2.0 metadata](https://idp.sussex.ac.uk/idp/shibboleth) | **institution** | 200; `entityID=https://idp.sussex.ac.uk/shibboleth`, `shibmd:Scope=sussex.ac.uk`; host CNAMEs to `uos-idp-shib-prod.uksouth.cloudapp.azure.com` |
| [Okta SSO (OIDC discovery)](https://okta.sussex.ac.uk/.well-known/openid-configuration) | tenant | 200; issuer `https://okta.sussex.ac.uk`; host CNAMEs to `sussexac.customdomains.okta.com` |
| [Canvas VLE](https://canvas.sussex.ac.uk/api/lti/security/jwks) | tenant | `/api/v1/*` 401; LTI 1.3 JWKS 200; host CNAMEs to `universityofsussex-vanity.instructure.com` |
| [Figshare research repository](https://sussex.figshare.com/) | tenant | AWS WAF challenge (202); DataCite client `FIGSHARE.SUSSEX`, domains `sussex.figshare.com` |
| [Ex Libris Primo discovery](https://sussex.primo.exlibrisgroup.com/discovery/search?vid=44SUS_INST:44SUS_VU1) | tenant | 200; institution view `44SUS_INST` on the vendor's shared host |

## Correction — 2026-08-30

This profile previously listed **ten OpenAPI definitions** under Sussex's name
(`altmetric`, `articles`, `authors`, `collections`, `institutions`, `oauth`, `other`, `profiles`,
`projects`, `symplectic`) and **thirty-eight artifacts derived from them**. All ten were the same
document: Figshare's generic v2 API contract, `info.title` beginning "Figshare", `info.contact`
`support.figshare.com`, and an **empty `servers` block** — the same contract eleven other
institutions in this catalog also shipped under their own names. None of it was Sussex's
engineering, and all of it has been removed, along with the JSON Schemas, JSON Structures,
examples, Postman/OpenCollection collections, Spectral rulesets, vocabulary, JSON-LD context,
agentic-access classification and capability map that inherited its provenance.

What replaced it is smaller and true: Sussex's own Shibboleth identity provider, four recorded
tenant relationships, and probed conformance against the education regime's domain standards.

## Artifacts

- [conformance/university-of-sussex-domain-standards.yml](conformance/university-of-sussex-domain-standards.yml) — probed `shibboleth`, `saml`, `lti`, `datacite`; `oai-pmh` blocked
- [authentication/university-of-sussex-authentication.yml](authentication/university-of-sussex-authentication.yml) — probed
- [scopes/university-of-sussex-scopes.yml](scopes/university-of-sussex-scopes.yml) — probed
- [security/university-of-sussex-domain-security.yml](security/university-of-sussex-domain-security.yml)
- [plans/university-of-sussex-plans-pricing.yml](plans/university-of-sussex-plans-pricing.yml)
- [rate-limits/university-of-sussex-rate-limits.yml](rate-limits/university-of-sussex-rate-limits.yml)
- [finops/university-of-sussex-finops.yml](finops/university-of-sussex-finops.yml)
- [review.yml](review.yml)

There is no `openapi/` directory. Sussex publishes no OpenAPI of its own, and none has been
generated to fill the gap.

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.sussex.ac.uk/
- GitHub: https://github.com/universityofsussex (exists, zero public repositories)
- LinkedIn: https://www.linkedin.com/school/university-of-sussex/
- Course catalog: https://www.sussex.ac.uk/study/undergraduate/courses
- Research computing (HPC): https://www.sussex.ac.uk/its/services/research/highperformance
- IT service catalogue: https://www.sussex.ac.uk/its/about/servicedescriptions

## Notes

- Verification discipline: only surfaces confirmed live are listed; nothing fabricated.
- Sussex operates **no public developer portal and no institution-authored API contract**. That is
  a correct measurement of a university, not a gap in this profile.
- `data.sussex.ac.uk` and `api.sussex.ac.uk` do not resolve. `www.sussex.ac.uk/llms.txt` is a 404.
- `sussex.figshare.com` sits behind an AWS WAF challenge (HTTP 202, `x-amzn-waf-action: challenge`)
  that answers every request with an empty body, so the Figshare tenant's OAI-PMH endpoint could
  not be confirmed. That is a blocked probe, not a dead host.
- The former Sussex Research Online EPrints OAI-PMH endpoint (`sro.sussex.ac.uk/cgi/oai2`) is
  decommissioned and redirects to an HTML publications page.

## Maintainers

- Kin Lane — kin@apievangelist.com
