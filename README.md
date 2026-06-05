# Dust (dust-tt)

Dust is a Paris-based enterprise AI platform for building, deploying, and operating teams of AI agents that have
shared context across a company's knowledge and tools. Dust positions itself as the platform for "AI Operators" —
the people who design, govern, and continuously improve agentic workflows across Sales, Customer Support,
Marketing, Engineering, Data & Analytics, IT, Legal, Recruiting, and Knowledge teams. Agents in Dust are
model-agnostic (OpenAI, Anthropic, Google, Mistral), grounded on company data through 100+ connectors (Slack,
Notion, GitHub, Google Drive, Salesforce, Zendesk, Jira, Confluence, HubSpot, BigQuery, Snowflake), exposed via a
REST API, MCP servers (client- and server-side), webhooks, and OAuth2, and reachable from a multiplayer
conversation UI, Slack, a Chrome extension, a Raycast extension, and a CLI.

The Dust core platform is open source under the MIT license at github.com/dust-tt/dust. The hosted service is
available on a per-seat Pro plan (29 EUR / user / month) and a custom Enterprise tier (100+ seats) with SSO,
SCIM, dedicated environments, EU residency, and SOC 2 Type II / GDPR / HIPAA-ready compliance.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/apis.yml)

## Scope

- **Access:** 3rd-Party

## Tags

- Agents
- AI
- Artificial Intelligence
- Custom Workflows
- Data Sources
- Dust
- Enterprise AI
- Knowledge Management
- LLM
- MCP
- Multi-Model
- RAG

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Dust Agents API

Create, list, retrieve, update, archive, search, import, and export Dust agent configurations. An agent in Dust is
a named, versioned configuration of an LLM (OpenAI, Anthropic, Google, Mistral) plus instructions, tools, and
data-source bindings that can be invoked from conversations, Slack, the Chrome extension, or programmatically.

- **Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
- **Base URL:** `https://dust.tt/api/v1`

#### Tags

- Agents
- AI
- Artificial Intelligence
- Dust

#### Properties

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-agents-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dust-agents-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/dust-agents-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/dust-agent-configuration-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/dust-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Dust Conversations API

Drive multi-turn conversations with Dust agents. Create conversations, post user messages, stream agent events
over SSE, attach content fragments (file/page/snippet attachments), retrieve and download conversation-scoped
files, submit and delete message feedback, and resolve @mention suggestions for agent routing.

- **Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
- **Base URL:** `https://dust.tt/api/v1`

#### Tags

- AI
- Artificial Intelligence
- Conversations
- Dust
- Messages

#### Properties

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-conversations-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dust-conversations-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/dust-conversations-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/dust-conversation-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Dust Data Sources API

Manage Dust data sources, data source views, spaces, documents, tables, and folders. Upsert documents and table
rows programmatically, search semantically, manage hierarchies and parents, and check the asynchronous upsert
queue. Data sources are the retrieval layer behind every Dust agent.

- **Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
- **Base URL:** `https://dust.tt/api/v1`

#### Tags

- AI
- Artificial Intelligence
- Data Sources
- Dust
- RAG
- Search

#### Properties

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-datasources-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dust-datasources-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/dust-datasources-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/dust-datasource-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/dust-document-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Dust MCP API

Register a client-side Model Context Protocol server with a Dust workspace, stream MCP tool-call requests over
SSE, return tool execution results back to Dust agents, and keep the server's heartbeat alive. Also lists the
MCP server views available in a space.

- **Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
- **Base URL:** `https://dust.tt/api/v1`

#### Tags

- AI
- Artificial Intelligence
- Dust
- MCP
- Tools

#### Properties

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-mcp-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dust-mcp-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/dust-mcp-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Dust Apps API

List Dust Apps in a space and create or retrieve App runs. Dust Apps are chained-block LLM/code pipelines
defined in the Dust Builder and executable as parameterized "functions" from agents, code, or webhooks.

- **Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
- **Base URL:** `https://dust.tt/api/v1`

#### Tags

- AI
- Artificial Intelligence
- Apps
- Dust

#### Properties

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-apps-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dust-apps-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/dust-apps-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Dust Search API

Search nodes (documents, tables, folders, conversations) across an entire Dust workspace. Streaming SSE
variant for incremental result delivery, plus a tool-file upload endpoint backing search-related tool calls.

- **Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
- **Base URL:** `https://dust.tt/api/v1`

#### Tags

- AI
- Artificial Intelligence
- Dust
- Search

#### Properties

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-search-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dust-search-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/dust-search-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Dust Skills API

List the skill bundles installed in a Dust workspace and import new skills from uploaded files. Skills are
reusable instruction + tool packs that agents can attach to.

- **Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
- **Base URL:** `https://dust.tt/api/v1`

#### Tags

- AI
- Artificial Intelligence
- Dust
- Skills

#### Properties

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-skills-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dust-skills-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/dust-skills-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/dust-skill-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Dust Triggers API

Receive an external webhook on a registered Dust webhook source and fan it out to trigger agent workflows
(e.g. run an agent when a GitHub issue opens or a Notion page changes).

- **Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
- **Base URL:** `https://dust.tt/api/v1`

#### Tags

- AI
- Artificial Intelligence
- Dust
- Triggers
- Webhooks

#### Properties

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-triggers-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dust-triggers-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/dust-triggers-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Dust Workspace API

Export workspace analytics and pull aggregated workspace usage data for chargeback, capacity planning, and
FinOps reporting against Dust seat and programmatic-API consumption.

- **Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
- **Base URL:** `https://dust.tt/api/v1`

#### Tags

- Administration
- AI
- Analytics
- Artificial Intelligence
- Dust
- FinOps

#### Properties

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-workspace-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dust-workspace-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/dust-workspace-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://dust.tt)
- [Documentation](https://docs.dust.tt)
- [API Reference](https://docs.dust.tt/reference)
- [Getting Started](https://docs.dust.tt/docs/intro)
- [Getting Started](https://docs.dust.tt/docs/programmatic-usage)
- [Pricing](https://dust.tt/pricing)
- [GitHub Organization](https://github.com/dust-tt)
- [Source Code](https://github.com/dust-tt/dust)
- [License](https://github.com/dust-tt/dust/blob/main/LICENSE)
- [Changelog](https://docs.dust.tt/changelog)
- [Sign Up](https://dust.tt/sign-up)
- [Contact Sales](https://dust.tt/home/contact)
- [Security](https://dust.tt/home/security)
- [Trust Center](https://trust.dust.tt)
- [Terms of Service](https://dust.tt/terms)
- [Privacy Policy](https://dust.tt/website-privacy)
- [Compliance](https://dust.tt/home/security)
- [SDK](https://github.com/dust-tt/dust-sdk-js)
- [SDK](https://docs.dust.tt/reference/javascript-sdk)
- [C L I](https://docs.dust.tt/reference/cli)
- [Tools](https://github.com/dust-tt/dust-labs)
- [Tools](https://github.com/dust-tt/dust-github-action)
- [Tools](https://github.com/dust-tt/dust-n8n-node)
- [Tools](https://github.com/dust-tt/raycast-extension)
- [Tools](https://github.com/dust-tt/browse)
- [Tools](https://github.com/dust-tt/srchd)
- [Browser Extension](https://dust.tt/home/chrome-extension)
- [Postman](https://app.getpostman.com/run-collection/34241185-c7e0fdbe-b2c5-47d5-a923-8244d45cd95e) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [OpenAPI](https://dust.tt/swagger.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Academy Mode](https://dust.tt/academy)
- [Blog](https://blog.dust.tt)
- [Forum](https://dust-community.tightknit.community/join)
- [Status Page](https://status.dust.tt)
- [Integrations](https://dust.tt/integrations)
- [Integrations](https://docs.dust.tt/docs/slack)
- [Integrations](https://docs.dust.tt/docs/notion-mcp)
- [Integrations](https://docs.dust.tt/docs/github-connection)
- [Integrations](https://docs.dust.tt/docs/google-drive-connection)
- [Integrations](https://docs.dust.tt/docs/confluence-connection)
- [Integrations](https://docs.dust.tt/docs/salesforce)
- [Integrations](https://docs.dust.tt/docs/hubspot)
- [Integrations](https://docs.dust.tt/docs/zendesk)
- [Integrations](https://docs.dust.tt/docs/jira)
- [Integrations](https://docs.dust.tt/docs/bigquery)
- [Solutions](https://dust.tt/home/solutions/sales)
- [Solutions](https://dust.tt/home/solutions/customer-support)
- [Solutions](https://dust.tt/home/solutions/marketing)
- [Solutions](https://dust.tt/home/solutions/engineering)
- [Solutions](https://dust.tt/home/solutions/data-analytics)
- [Solutions](https://dust.tt/home/solutions/knowledge)
- [Solutions](https://dust.tt/home/solutions/it)
- [Solutions](https://dust.tt/home/solutions/legal)
- [Solutions](https://dust.tt/home/solutions/recruiting-people)
- [Industry](https://dust.tt/home/industry/b2b-saas)
- [Industry](https://dust.tt/home/industry/financial-services)
- [Industry](https://dust.tt/home/industry/consulting)
- [Industry](https://dust.tt/home/industry/insurance)
- [Industry](https://dust.tt/home/industry/marketplace)
- [Industry](https://dust.tt/home/industry/retail-ecommerce)
- [LinkedIn](https://www.linkedin.com/company/dust-tt)
- [Twitter](https://twitter.com/dust4ai)
- [Plans](plans/dust-plans-pricing.yml)
- [Rate Limits](rate-limits/dust-rate-limits.yml)
- [Fin Ops](finops/dust-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
