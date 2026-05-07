# Bubble (bubble)

Bubble is a no-code application development platform that lets builders ship full-stack web and mobile apps without writing code. Bubble exposes three developer APIs — the Data API for CRUD against the app database, the Workflow API for triggering backend automations, and a JavaScript Plugin API for extending the platform with custom actions and elements. Server-side consumption is metered in Workload Units (WU) bundled into a tiered subscription (Free, Starter, Growth, Team, Enterprise) with overage pricing for additional WU and storage.

**URL:** [Visit APIs.json URL](https://bubble.io/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - No-Code, Application Platform, Database, Workflow Automation, Plugins

## Timestamps

- **Created:** 2026-05-06
- **Modified:** 2026-05-06

## APIs

### Bubble Data API

REST API exposing the Bubble app database. Supports search with constraints, cursor-based pagination, single-record CRUD, bulk create (up to 1,000 records), and metadata discovery. Authentication uses bearer tokens (admin tokens bypass privacy rules; user tokens enforce them). Endpoints are available on both live and `version-test` (development) environments.

**Human URL:** [https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api.md](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api.md)

#### Tags:

 - Data API, REST, CRUD, Database

#### Properties

- [Documentation](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api.md)
- [APIReference](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api/data-api-endpoints.md)
- [Authentication](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api/authentication.md)
- [Quickstart](https://manual.bubble.io/core-resources/api/the-bubble-api/the-data-api/data-api-requests.md)
- [OpenAPI](openapi/bubble-data-api-openapi.yml)
- [JSONSchema](json-schema/bubble-data-thing-schema.json)
- [JSONSchema](json-schema/bubble-data-search-response-schema.json)
- [JSONSchema](json-schema/bubble-error-schema.json)

### Bubble Workflow API

REST API for triggering backend workflows defined in the Bubble editor. Each workflow is exposed at `/api/1.1/wf/{workflow_name}` and can be configured for POST or GET, with authentication settings ranging from public to user/admin to admin-only. Workflows can return JSON, plain text, or a configurable redirect on success/error.

**Human URL:** [https://manual.bubble.io/core-resources/api/the-bubble-api/the-workflow-api.md](https://manual.bubble.io/core-resources/api/the-bubble-api/the-workflow-api.md)

#### Tags:

 - Workflow API, REST, Automation, Webhooks

#### Properties

- [Documentation](https://manual.bubble.io/core-resources/api/the-bubble-api/the-workflow-api.md)
- [Security](https://manual.bubble.io/help-guides/security/api-security/workflow-api-security.md)
- [OpenAPI](openapi/bubble-workflow-api-openapi.yml)
- [JSONSchema](json-schema/bubble-workflow-response-schema.json)

### Bubble Plugin API

JavaScript SDK surface for building Bubble plugins. Plugin authors write server-side actions, client-side actions, and visual elements that receive `(properties, context)` and read/write data through `BubbleThing` and `BubbleList` wrappers. Plugin API v4 replaces Fibers with native Promises and adds first-class type checks (`isBubbleThing`, `isBubbleList`), id-based lookups (`getThingById`, `getThingsById`), and async iteration on `BubbleList`.

**Human URL:** [https://manual.bubble.io/account-and-marketplace/building-plugins.md](https://manual.bubble.io/account-and-marketplace/building-plugins.md)

#### Tags:

 - Plugin API, JavaScript SDK, Extension, Marketplace

#### Properties

- [Documentation](https://manual.bubble.io/account-and-marketplace/building-plugins.md)
- [APIReference](https://manual.bubble.io/account-and-marketplace/building-plugins/updating-to-plugin-api-v4.md)
- [Tutorials](https://manual.bubble.io/account-and-marketplace/building-plugins/building-actions.md)
- [Tutorials](https://manual.bubble.io/account-and-marketplace/building-plugins/building-elements.md)
- [OpenAPI](openapi/bubble-plugin-api-openapi.yml)

## Common Properties

- [Documentation](https://manual.bubble.io/)
- [GettingStarted](https://manual.bubble.io/getting-started.md)
- [APIReference](https://manual.bubble.io/core-resources/api.md)
- [Authentication](https://manual.bubble.io/help-guides/integrations/api/the-bubble-api/authentication/how-to-authenticate.md)
- [Pricing](https://bubble.io/pricing)
- [Plans](plans/bubble-plans-pricing.yml)
- [RateLimits](rate-limits/bubble-rate-limits.yml)
- [Plans](https://manual.bubble.io/account-and-marketplace/account-and-billing/pricing-plans.md)
- [SignUp](https://bubble.io/signup)
- [Login](https://bubble.io/login)
- [Portal](https://bubble.io/)
- [Marketplace](https://bubble.io/plugins)
- [Customers](https://bubble.io/showcase)
- [Showcase](https://bubble.io/showcase)
- [Blog](https://bubble.io/blog)
- [Support](https://bubble.io/contact)
- [ChangeLog](https://bubble.io/release-notes)
- [ReleaseNotes](https://bubble.io/release-notes)
- [StatusPage](https://status.bubble.io/)
- [TermsOfService](https://bubble.io/legal/terms-of-service)
- [PrivacyPolicy](https://bubble.io/legal/privacy)
- [Compliance](https://manual.bubble.io/help-guides/security.md)
- [Security](https://manual.bubble.io/help-guides/security/api-security.md)
- [TrustCenter](https://bubble.io/trust)
- [Glossary](https://manual.bubble.io/glossary.md)
- [Academy](https://bubble.io/academy)
- [YouTube](https://www.youtube.com/@Bubble)
- [X](https://twitter.com/bubble)
- [LinkedIn](https://www.linkedin.com/company/bubble-group)
- [GitHubOrganization](https://github.com/bubblegroup)
- [KnowledgeCenter](https://manual.bubble.io/)
- [JSONLD](json-ld/bubble-context.jsonld)
- [SpectralRules](rules/bubble-rules.yml)
- [Vocabulary](vocabulary/bubble-vocabulary.yml)
- [NaftikoCapability](capabilities/shared/bubble-data-api.yaml)
- [NaftikoCapability](capabilities/shared/bubble-workflow-api.yaml)
- [NaftikoCapability](capabilities/headless-backend.yaml)
- [Example](examples/bubble-data-search-example.json)
- [Example](examples/bubble-data-create-example.json)
- [Example](examples/bubble-data-modify-example.json)
- [Example](examples/bubble-data-bulk-create-example.json)
- [Example](examples/bubble-workflow-trigger-example.json)
- [FinOps](finops/bubble-finops.yml)

## Features

| Name | Description |
|------|-------------|
| Visual Editor | Drag-and-drop application designer with responsive layouts and reusable element groups. |
| Built-In Database | Type-safe app database with privacy rules, search constraints, and Data API exposure. |
| Backend Workflows | Server-side automation engine with scheduling, recurring events, and webhook triggers. |
| Plugin Marketplace | Public catalog of plugins exposing custom actions, elements, and integrations to Bubble apps. |
| API Connector | Built-in HTTP client for calling external REST APIs from Bubble workflows and elements. |
| Custom Domains | Connect a custom domain on paid plans, with automatic SSL. |
| Version Control | Editor-level version control with branches and rollback (Growth, Team, Enterprise). |
| Workload Dashboard | Real-time visibility into Workload Unit consumption per activity, page, and workflow. |
| Mobile Builds | Native iOS and Android builds via the Mobile add-on bundles. |
| Multi-App Editing | Multiple editors and multi-app dashboards for agencies and teams. |

## Use Cases

| Name | Description |
|------|-------------|
| Internal Tools | Build admin dashboards, CRM panels, and operations consoles without engineering headcount. |
| Marketplaces | Two-sided marketplace MVPs with user roles, listings, search, and payments. |
| SaaS MVPs | Subscription-billed SaaS products with multi-tenant data, auth, and Stripe integration. |
| Headless Backend | Use a Bubble app as a managed backend for separately built mobile or web clients. |
| Internal API Integrations | Webhook ingestion and back-office automation triggered from third-party tools. |
| Customer Portals | Authenticated portals with privacy-rule-controlled data access and document upload. |

## Integrations

| Name | Description |
|------|-------------|
| Stripe | Built-in Stripe plugin for payments, subscriptions, and Connect. |
| SendGrid | Transactional and marketing email via the SendGrid plugin. |
| Twilio | SMS and programmable voice via the Twilio plugin. |
| Google APIs | Maps, OAuth, Calendar, Sheets, and Drive integrations via plugins. |
| AWS | S3 file storage, Lambda, and SES integrations. |
| Algolia | Hosted search backed by Algolia for high-volume Bubble data. |
| Zapier | Bubble Workflow API endpoints triggered by Zapier zaps. |
| Make (Integromat) | Bubble Workflow API endpoints triggered by Make scenarios. |
| OpenAI | AI-powered features via OpenAI plugin actions. |
| Slack | Outbound notifications and inbound webhooks for team collaboration. |

## Solutions

| Name | Description |
|------|-------------|
| For Founders | Ship a SaaS or marketplace MVP without hiring engineers; iterate with users in real time. |
| For Agencies | White-label client apps with multi-app editor, version control, and sub-app architecture. |
| For Enterprise | Dedicated infrastructure, SSO, custom rate limits, advanced security, and SLA-backed support. |
| For Developers | Build and publish plugins to the marketplace; extend Bubble apps with custom JavaScript actions and elements. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Bubble Data API](openapi/bubble-data-api-openapi.yml)
- [Bubble Workflow API](openapi/bubble-workflow-api-openapi.yml)
- [Bubble Plugin API](openapi/bubble-plugin-api-openapi.yml)

### JSON Schema

- [Bubble Data Thing](json-schema/bubble-data-thing-schema.json)
- [Bubble Data Search Response](json-schema/bubble-data-search-response-schema.json)
- [Bubble Workflow Response](json-schema/bubble-workflow-response-schema.json)
- [Bubble API Error](json-schema/bubble-error-schema.json)

### JSON-LD

- [Bubble Context](json-ld/bubble-context.jsonld)

### Examples

- [Data API — Search](examples/bubble-data-search-example.json)
- [Data API — Create](examples/bubble-data-create-example.json)
- [Data API — Modify](examples/bubble-data-modify-example.json)
- [Data API — Bulk Create](examples/bubble-data-bulk-create-example.json)
- [Workflow API — Trigger](examples/bubble-workflow-trigger-example.json)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Bubble Data API](capabilities/shared/bubble-data-api.yaml) — 8 operations for database CRUD, search, bulk, and metadata
- [Bubble Workflow API](capabilities/shared/bubble-workflow-api.yaml) — 3 operations for triggering and initializing backend workflows

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Headless Backend](capabilities/headless-backend.yaml) | Data API + Workflow API | 6 | Backend Integrator |

## Vocabulary

- [Bubble Vocabulary](vocabulary/bubble-vocabulary.yml) — Unified taxonomy mapping 12 resources, 11 actions, 7 workflows, and 6 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Bubble Rules](rules/bubble-rules.yml) — 12 rules across info/server/security/operation/path categories enforcing Bubble API conventions

## Plans, Rate Limits & FinOps

- [Plans & Pricing](plans/bubble-plans-pricing.yml) — Free, Starter, Growth, Team, Enterprise tiers plus Mobile bundles and add-ons
- [Rate Limits](rate-limits/bubble-rate-limits.yml) — Per-plan request-per-minute ceilings, hard limits, and Workload Unit policies
- [FinOps](finops/bubble-finops.yml) — FOCUS-aligned billing model with WU as the primary meter

## Maintainers

**FN:** Kin Lane

**Email:** kinlane@gmail.com
