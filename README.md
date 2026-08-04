# Bubble (bubble)

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

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bubble/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bubble/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- No-Code
- Application Platform
- Database
- Workflow Automation
- Plugins

## Timestamps

- **Created:** 2026-05-06
- **Modified:** 2026-05-19

## APIs

### Bubble Data API

REST API exposing the Bubble app database. Supports search with
constraints, cursor-based pagination, single-record CRUD, bulk create
(up to 1,000 records), and metadata discovery. Authentication uses
bearer tokens (admin tokens bypass privacy rules; user tokens enforce
them). Endpoints are available on both live and `version-test`
(development) environments.

- **Human URL:** [https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api.md](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api.md)
- **Base URL:** `https://{appname}.bubbleapps.io/api/1.1`

#### Tags

- Data API
- REST
- CRUD
- Database

#### Properties

- [Documentation](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api.md)
- [API Reference](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api/data-api-endpoints.md)
- [Authentication](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api/authentication.md)
- [Quickstart](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api/data-api-requests.md)
- [OpenAPI](openapi/bubble-data-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bubble-data-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bubble-data-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bubble-data-thing-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bubble-data-search-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/bubble-error-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Bubble Workflow API

REST API for triggering backend workflows defined in the Bubble editor.
Each workflow is exposed at `/api/1.1/wf/{workflow_name}` and can be
configured for POST or GET, with authentication settings ranging from
public to user/admin to admin-only. Workflows can return JSON, plain
text, or a configurable redirect on success/error.

- **Human URL:** [https://manual.bubble.io/core-resources/api/the-bubble-api/the-workflow-api.md](https://manual.bubble.io/core-resources/api/the-bubble-api/the-workflow-api.md)
- **Base URL:** `https://{appname}.bubbleapps.io/api/1.1`

#### Tags

- Workflow API
- REST
- Automation
- Webhooks

#### Properties

- [Documentation](https://manual.bubble.io/core-resources/api/the-bubble-api/the-workflow-api.md)
- [Security](https://manual.bubble.io/help-guides/security/api-security/workflow-api-security.md)
- [OpenAPI](openapi/bubble-workflow-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bubble-workflow-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bubble-workflow-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bubble-workflow-response-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Bubble Plugin API

JavaScript SDK surface for building Bubble plugins. Plugin authors write
server-side actions, client-side actions, and visual elements that
receive `(properties, context)` and read/write data through `BubbleThing`
and `BubbleList` wrappers. Plugin API v4 replaces Fibers with native
Promises and adds first-class type checks (`isBubbleThing`,
`isBubbleList`), id-based lookups (`getThingById`, `getThingsById`), and
async iteration on `BubbleList`.

- **Human URL:** [https://manual.bubble.io/account-and-marketplace/building-plugins.md](https://manual.bubble.io/account-and-marketplace/building-plugins.md)
- **Base URL:** `virtual://plugin-runtime`

#### Tags

- Plugin API
- JavaScript SDK
- Extension
- Marketplace

#### Properties

- [Documentation](https://manual.bubble.io/account-and-marketplace/building-plugins.md)
- [API Reference](https://manual.bubble.io/account-and-marketplace/building-plugins/updating-to-plugin-api-v4.md)
- [Tutorials](https://manual.bubble.io/account-and-marketplace/building-plugins/building-actions.md)
- [Tutorials](https://manual.bubble.io/account-and-marketplace/building-plugins/building-elements.md)
- [OpenAPI](openapi/bubble-plugin-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bubble-plugin-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bubble-plugin-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Documentation](https://manual.bubble.io/)
- [Getting Started](https://manual.bubble.io/getting-started.md)
- [API Reference](https://manual.bubble.io/core-resources/api.md)
- [Authentication](https://manual.bubble.io/help-guides/integrations/api/the-bubble-api/authentication/how-to-authenticate.md)
- [Pricing](https://bubble.io/pricing)
- [Plans](plans/bubble-plans-pricing.yml)
- [Rate Limits](rate-limits/bubble-rate-limits.yml)
- [Plans](https://manual.bubble.io/account-and-marketplace/account-and-billing/pricing-plans.md)
- [Sign Up](https://bubble.io/signup)
- [Login](https://bubble.io/login)
- [Portal](https://bubble.io/)
- [Marketplace](https://bubble.io/plugins)
- [Customers](https://bubble.io/showcase)
- [Showcase](https://bubble.io/showcase)
- [Blog](https://bubble.io/blog)
- [Support](https://bubble.io/contact)
- [Changelog](https://bubble.io/release-notes)
- [Release Notes](https://bubble.io/release-notes)
- [Status Page](https://status.bubble.io/)
- [Terms of Service](https://bubble.io/legal/terms-of-service)
- [Privacy Policy](https://bubble.io/legal/privacy)
- [Compliance](https://manual.bubble.io/help-guides/security.md)
- [Security](https://manual.bubble.io/help-guides/security/api-security.md)
- [Trust Center](https://bubble.io/trust)
- [Glossary](https://manual.bubble.io/glossary.md)
- [Academy](https://bubble.io/academy)
- [YouTube](https://www.youtube.com/@Bubble)
- [X (Twitter)](https://twitter.com/bubble)
- [LinkedIn](https://www.linkedin.com/company/bubble-group)
- [GitHub Organization](https://github.com/bubblegroup)
- [Knowledge Center](https://manual.bubble.io/)
- [JSON-LD](json-ld/bubble-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/bubble-rules.yml)
- [Vocabulary](vocabulary/bubble-vocabulary.yml)
- [Example](examples/bubble-data-search-example.json)
- [Example](examples/bubble-data-create-example.json)
- [Example](examples/bubble-data-modify-example.json)
- [Example](examples/bubble-data-bulk-create-example.json)
- [Example](examples/bubble-workflow-trigger-example.json)
- [Fin Ops](finops/bubble-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kinlane@gmail.com
