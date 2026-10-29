# Bubble

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

Bubble is a no-code application development platform that lets builders ship
full-stack web and mobile apps without writing code. Bubble exposes three
developer APIs — the Data API for CRUD against the app database, the
Workflow API for triggering backend automations, and a JavaScript Plugin
API for extending the platform with custom actions and elements. Server-side
consumption is metered in Workload Units (WU) bundled into a tiered
subscription (Free, Starter, Growth, Team, Enterprise) with overage pricing
for additional WU and storage.

**Areas:** No-Code · Application Platform · Database · Workflow Automation · Plugins

## Bubble on APIs.io

Everything profiled for Bubble is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/bubble/](https://apis.io/providers/bubble/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Bubble Action API](https://apis.io/apis/bubble/bubble-action-api/) — Server-side and client-side action functions invoked by Bubble workflows.
- [Bubble Context API](https://apis.io/apis/bubble/bubble-context-api/) — Helpers exposed on the runtime context object.
- [Bubble Element API](https://apis.io/apis/bubble/bubble-element-api/) — Visual element lifecycle hooks invoked by the Bubble page renderer.
- [Bubble Thing API](https://apis.io/apis/bubble/bubble-thing-api/) — Database object accessors exposed to plugin code.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (10)

Multi-step workflows that chain operations into a business task.

- [Bubble Bulk Create Then Search](https://apis.io/arazzos/bubble/bubble-bulk-create-then-search-workflow/)
- [Bubble Create and Verify a Thing](https://apis.io/arazzos/bubble/bubble-create-and-get-thing-workflow/)
- [Bubble Create a Thing Then Trigger a Backend Workflow](https://apis.io/arazzos/bubble/bubble-create-thing-then-trigger-workflow-workflow/)
- [Bubble Discover Data Types Then Search](https://apis.io/arazzos/bubble/bubble-discover-types-then-search-workflow/)
- [Bubble Get Then Replace a Thing](https://apis.io/arazzos/bubble/bubble-get-then-replace-thing-workflow/)
- [Bubble Initialize Then Trigger a Backend Workflow](https://apis.io/arazzos/bubble/bubble-initialize-then-trigger-workflow-workflow/)
- [Bubble Search Then Delete a Thing](https://apis.io/arazzos/bubble/bubble-search-then-delete-thing-workflow/)
- [Bubble Search Then Update a Thing](https://apis.io/arazzos/bubble/bubble-search-then-update-thing-workflow/)
- [Bubble Trigger a Workflow Then Log a Thing](https://apis.io/arazzos/bubble/bubble-trigger-workflow-then-log-thing-workflow/)
- [Bubble Upsert a Thing](https://apis.io/arazzos/bubble/bubble-upsert-thing-workflow/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Bubble Agentic Access](https://apis.io/agentic-access/bubble/bubble-agentic-access/)

#### JSON Schema (4)

The data models the API reads and writes.

- [Bubble Data Search Response](https://apis.io/schemas/bubble/bubble-data-search-response/)
- [Bubble Data Thing](https://apis.io/schemas/bubble/bubble-data-thing/)
- [Bubble API Error](https://apis.io/schemas/bubble/bubble-error/)
- [Bubble Workflow Response](https://apis.io/schemas/bubble/bubble-workflow-response/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Bubble Context](https://apis.io/jsonld/bubble/bubble-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Bubble Vocabulary](https://apis.io/vocabularies/bubble/bubble-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Bubble Data Bulk Create Example](https://apis.io/examples/bubble/bubble-data-bulk-create-example/)
- [Bubble Data Create Example](https://apis.io/examples/bubble/bubble-data-create-example/)
- [Bubble Data Modify Example](https://apis.io/examples/bubble/bubble-data-modify-example/)
- [Bubble Data Search Example](https://apis.io/examples/bubble/bubble-data-search-example/)
- [Bubble Workflow Trigger Example](https://apis.io/examples/bubble/bubble-workflow-trigger-example/)

#### Collections (10)

Postman and Open Collection request collections.

- [Bubble Data Action API](https://apis.io/collections/bubble/open-bubble-action-api/)
- [Bubble Data Action Context API](https://apis.io/collections/bubble/open-bubble-context-api/)
- [Bubble Action Data API](https://apis.io/collections/bubble/open-bubble-data-api/)
- [Bubble Data Action Element API](https://apis.io/collections/bubble/open-bubble-element-api/)
- [Bubble Plugin API](https://apis.io/collections/bubble/open-bubble-plugin-api/)
- [Bubble Data Action Thing API](https://apis.io/collections/bubble/open-bubble-thing-api/)
- [Bubble Data Action Workflow API](https://apis.io/collections/bubble/open-bubble-workflow-api/)
- [Bubble Data API](https://apis.io/collections/bubble/postman-bubble-data-api/)
- [Bubble Plugin API](https://apis.io/collections/bubble/postman-bubble-plugin-api/)
- [Bubble Workflow API](https://apis.io/collections/bubble/postman-bubble-workflow-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Bubble — jsonschema rules](https://apis.io/rules/bubble/bubble-jsonschema-spectral-rules/)
- [Bubble API Rules](https://apis.io/rules/bubble/bubble-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Bubble Authentication](https://apis.io/security/bubble/bubble-authentication/)
- [Bubble Domain Security](https://apis.io/security/bubble/bubble-domain-security/)
- [Bubble Trust Center](https://apis.io/security/bubble/bubble-trust-center/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Bubble Plans Pricing](https://apis.io/plans/bubble/bubble-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Bubble Rate Limits](https://apis.io/rate-limits/bubble/bubble-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Bubble Finops](https://apis.io/finops/bubble/bubble-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://bubble.io)
- [Documentation](https://manual.bubble.io/)
- [Getting started](https://manual.bubble.io/getting-started.md)
- [API reference](https://manual.bubble.io/core-resources/api.md)
- [Pricing](https://bubble.io/pricing)
- [Support](https://bubble.io/contact)
- [Changelog](https://bubble.io/release-notes)
- [Blog](https://bubble.io/blog)
- [Security](https://manual.bubble.io/help-guides/security/api-security.md)
- [Compliance](https://manual.bubble.io/help-guides/security.md)
- [Trust centre](https://bubble.io/trust)
- [Terms of service](https://bubble.io/legal/terms-of-service)
- [Privacy policy](https://bubble.io/legal/privacy)
- [GitHub](https://github.com/bubblegroup)
- [Status](https://status.bubble.io/)

## API Evangelist rating

**Kin Score 47.8** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 50.2 |
| Contract governance | 27.3 |
| Operational transparency | 52.6 |
| Developer ergonomics | 58.3 |
| Access clarity | 32.9 |

**Agent readiness 20.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 21.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/bubble/](https://apis.io/providers/bubble/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Bubble: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/bubble/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
