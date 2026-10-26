# 4Info

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

4INFO, Inc. was a San Mateo, California advertising-technology company founded in 2004 by Pankaj
Shah and Zaw Thet. It started as an SMS content and alerting service — Nielsen called it the
largest business-to-consumer SMS content provider in North America in 2008 — and pivoted in 2010
into mobile display advertising with the **AdHaven** platform (mobile ad server, audience
data-management and analytics). Its final product was an **identity graph** that statistically
resolved mobile devices, set-top boxes and connected TVs back to a household for cross-screen
targeting and measurement.

mBlox acquired the legacy SMS business in 2015. **Cadent acquired 4INFO in January 2020** and
folded the identity and cross-screen technology into its advanced-TV platform.

## Why this profile is thin

4INFO no longer operates as an independent company, and **there is no 4Info web surface left to
profile**. Probed 2026-09-05:

| Probe | Result |
|---|---|
| `https://4info.com/` | `000` — no A/AAAA record; DNS resolution fails |
| `https://www.4info.com/` | `000` — no A/AAAA record |
| 11 `/.well-known/*`, `/llms.txt`, `/openapi.json`, `/swagger.json` paths × 2 hosts | all `000` |
| Last Internet Archive capture of the site | 2023-02-02; the next capture (2023-05-28) is a `404` |
| `github.com/4info` | `200` — org exists ("4info Organization (Cadent)"), 1 public repo, a fork of `aerospike-loader` |
| npm / PyPI | no 4Info-published packages |

The domain is still delegated to Route 53 and carries live Proofpoint MX, SPF and DMARC records —
it is retained for **email only**. That posture is captured in
[`security/4info-domain-security.yml`](security/4info-domain-security.yml), and the recorded
absence of every discovery document in
[`well-known/4info-well-known.yml`](well-known/4info-well-known.yml).

The `forgeglobal.com/4info_stock/` URL this record was harvested from is a third-party
secondary-market venue listing, **not** 4Info's web presence, so it is recorded as
`x-harvest-source-url` rather than as a `Website` pointer.

`x-coverage: none / defunct`
