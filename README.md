# Bubble (bubble)

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
