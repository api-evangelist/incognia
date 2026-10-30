# Incognia

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

Incognia is a location identity and device fingerprinting platform for fraud prevention, providing real-time risk assessments for user onboarding, login, and payment transactions. Its API returns low_risk / high_risk / unknown_risk verdicts by combining privacy-first device recognition, location behavior analysis, and tamper detection, and accepts feedback events (chargebacks, account takeover, identity fraud, accepted/declined outcomes) that continuously tune the risk model. Incognia is used across financial services, fintech, marketplaces, delivery, and gaming to stop account takeover, new-account fraud, and payment fraud while reducing friction for trusted users. Authentication is OAuth 2.0 client credentials, exchanged for short-lived bearer tokens; official SDKs ship for Node.js, Python, Ruby, Java, and Go.

**Areas:** Company · Cybersecurity · Fraud Prevention · Device Fingerprinting · Location Identity · Identity Verification · Risk Assessment · Authentication · Fintech

## Incognia on APIs.io

Everything profiled for Incognia is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/incognia/](https://apis.io/providers/incognia/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Incognia Authentication API](https://apis.io/apis/incognia/incognia-authentication-api/) — OAuth 2.0 client-credentials token exchange
- [Incognia Feedback API](https://apis.io/apis/incognia/incognia-feedback-api/) — Report labeled events to tune the risk model
- [Incognia Onboarding API](https://apis.io/apis/incognia/incognia-onboarding-api/) — Signup risk assessment
- [Incognia Transactions API](https://apis.io/apis/incognia/incognia-transactions-api/) — Login and payment risk assessment

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [incognia](https://apis.io/servers/incognia/incognia/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Incognia Agentic Access](https://apis.io/agentic-access/incognia/incognia-agentic-access/)

#### Collections (4)

Postman and Open Collection request collections.

- [Incognia Authentication API](https://apis.io/collections/incognia/open-incognia-authentication-api/)
- [Incognia Authentication Feedback API](https://apis.io/collections/incognia/open-incognia-feedback-api/)
- [Incognia Authentication Onboarding API](https://apis.io/collections/incognia/open-incognia-onboarding-api/)
- [Incognia Authentication Transactions API](https://apis.io/collections/incognia/open-incognia-transactions-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Incognia Openapi Overlay](https://apis.io/overlays/incognia/incognia-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Incognia Authentication](https://apis.io/security/incognia/incognia-authentication/)
- [Incognia Domain Security](https://apis.io/security/incognia/incognia-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Incognia Scopes](https://apis.io/scopes/incognia/incognia-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.incognia.com/)
- [Documentation](https://developer.incognia.com/docs/)
- [Getting started](https://developer.incognia.com/docs/us/v5/apis/incognia-libraries/)
- [API reference](https://developer.incognia.com/docs/us/v5/apis/)
- [Pricing](https://www.incognia.com/pricing)
- [Blog](https://www.incognia.com/blog)
- [Trust centre](https://trust.incognia.com/)
- [Terms of service](https://www.incognia.com/terms-of-use)
- [Privacy policy](https://www.incognia.com/policies/)
- [GitHub](https://github.com/inloco)
- [Status](https://status.incognia.com/)

## API Evangelist rating

**Kin Score 26.2** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 0.0 |
| Contract governance | 4.5 |
| Operational transparency | 18.4 |
| Developer ergonomics | 23.2 |
| Access clarity | 31.6 |

**Agent readiness 26.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 34.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/incognia/](https://apis.io/providers/incognia/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Incognia: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/incognia/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
