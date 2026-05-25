# Dust (dust-tt)
Dust is a Paris-based enterprise AI platform for building, deploying, and operating teams of AI agents with shared context across a company's knowledge and tools. Agents are model-agnostic (OpenAI, Anthropic, Google, Mistral), grounded on company data via 100+ connectors (Slack, Notion, GitHub, Google Drive, Salesforce, Zendesk, Jira, Confluence, HubSpot, BigQuery, Snowflake), and reachable through a REST API, MCP servers, webhooks, OAuth2, a multiplayer conversation UI, Slack, a Chrome extension, a Raycast extension, and a CLI. The core platform is open-source (MIT) at [github.com/dust-tt/dust](https://github.com/dust-tt/dust).

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Agents, AI, Artificial Intelligence, Custom Workflows, Data Sources, Dust, Enterprise AI, Knowledge Management, LLM, MCP, Multi-Model, RAG

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Dust Agents API
Create, list, retrieve, update, archive, search, import, and export Dust agent configurations. Agents are versioned LLM configurations (OpenAI, Anthropic, Google, Mistral) plus instructions, tools, and data-source bindings.

**Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
**Base URL:** `https://dust.tt/api/v1`

- [Documentation](https://docs.dust.tt/reference)
- [OpenAPI](openapi/dust-agents-api-openapi.yml)
- [JSON Schema — Agent Configuration](json-schema/dust-agent-configuration-schema.json)
- [JSON-LD](json-ld/dust-context.jsonld)
- [Naftiko Capability — Agents](capabilities/agents-agents.yaml)

### Dust Conversations API
Drive multi-turn conversations with Dust agents. Create conversations, post messages, stream agent events over SSE, attach content fragments, retrieve files, submit feedback, and resolve @mentions.

**Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
**Base URL:** `https://dust.tt/api/v1`

- [OpenAPI](openapi/dust-conversations-api-openapi.yml)
- [JSON Schema — Conversation](json-schema/dust-conversation-schema.json)
- [Naftiko Capability — Conversations](capabilities/conversations-conversations.yaml)

### Dust Data Sources API
Manage Dust data sources, data source views, spaces, documents, tables, and folders. Upsert documents and rows programmatically, search semantically, and check the asynchronous upsert queue. This is the retrieval layer behind every Dust agent.

**Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
**Base URL:** `https://dust.tt/api/v1`

- [OpenAPI](openapi/dust-datasources-api-openapi.yml)
- [JSON Schema — Data Source](json-schema/dust-datasource-schema.json)
- [JSON Schema — Document](json-schema/dust-document-schema.json)
- [Naftiko Capability — Data Sources](capabilities/datasources-datasources.yaml)

### Dust MCP API
Register client-side Model Context Protocol servers, stream tool-call requests over SSE, return results, and keep the server's heartbeat alive. Also lists MCP server views in a space.

**Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
**Base URL:** `https://dust.tt/api/v1`

- [OpenAPI](openapi/dust-mcp-api-openapi.yml)
- [Naftiko Capability — MCP](capabilities/mcp-mcp.yaml)

### Dust Apps API
List Dust Apps and create or retrieve App runs. Dust Apps are chained-block LLM/code pipelines built in the Dust Builder and executable as parameterized functions from agents, code, or webhooks.

**Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
**Base URL:** `https://dust.tt/api/v1`

- [OpenAPI](openapi/dust-apps-api-openapi.yml)
- [Naftiko Capability — Apps](capabilities/apps-apps.yaml)

### Dust Search API
Search nodes (documents, tables, folders, conversations) across a workspace. Streaming SSE variant available; tool-file upload endpoint backs search-related tool calls.

**Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
**Base URL:** `https://dust.tt/api/v1`

- [OpenAPI](openapi/dust-search-api-openapi.yml)
- [Naftiko Capability — Search](capabilities/search-search.yaml)

### Dust Skills API
List the skill bundles installed in a workspace and import new skills from uploaded files. Skills are reusable instruction + tool packs.

**Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
**Base URL:** `https://dust.tt/api/v1`

- [OpenAPI](openapi/dust-skills-api-openapi.yml)
- [JSON Schema — Skill](json-schema/dust-skill-schema.json)
- [Naftiko Capability — Skills](capabilities/skills-skills.yaml)

### Dust Triggers API
Receive external webhook events on a registered Dust webhook source and fan them out to trigger agent workflows (e.g. run an agent when a GitHub issue opens or a Notion page changes).

**Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
**Base URL:** `https://dust.tt/api/v1`

- [OpenAPI](openapi/dust-triggers-api-openapi.yml)
- [Naftiko Capability — Triggers](capabilities/triggers-triggers.yaml)

### Dust Workspace API
Export workspace analytics and pull aggregated usage data for chargeback, capacity planning, and FinOps reporting against Dust seat and programmatic-API consumption.

**Human URL:** [https://docs.dust.tt/reference](https://docs.dust.tt/reference)
**Base URL:** `https://dust.tt/api/v1`

- [OpenAPI](openapi/dust-workspace-api-openapi.yml)
- [Naftiko Capability — Workspace](capabilities/workspace-workspace.yaml)

## Common Properties

- [Portal — dust.tt](https://dust.tt)
- [Documentation — docs.dust.tt](https://docs.dust.tt)
- [APIReference — Dust API Reference](https://docs.dust.tt/reference)
- [GettingStarted — Intro](https://docs.dust.tt/docs/intro)
- [GettingStarted — Programmatic Usage Guide](https://docs.dust.tt/docs/programmatic-usage)
- [Pricing](https://dust.tt/pricing)
- [GitHubOrganization](https://github.com/dust-tt)
- [SourceCode — dust (core, MIT)](https://github.com/dust-tt/dust)
- [License — MIT](https://github.com/dust-tt/dust/blob/main/LICENSE)
- [ChangeLog](https://docs.dust.tt/changelog)
- [SignUp](https://dust.tt/sign-up)
- [ContactSales](https://dust.tt/home/contact)
- [Security](https://dust.tt/home/security)
- [TrustCenter](https://trust.dust.tt)
- [TermsOfService](https://dust.tt/terms)
- [PrivacyPolicy](https://dust.tt/website-privacy)
- [Compliance — SOC 2 Type II, GDPR, HIPAA-ready](https://dust.tt/home/security)
- [SDK — Dust JavaScript / TypeScript SDK](https://github.com/dust-tt/dust-sdk-js)
- [SDK — JavaScript SDK reference](https://docs.dust.tt/reference/javascript-sdk)
- [CLI — Dust CLI](https://docs.dust.tt/reference/cli)
- [Tools — dust-labs](https://github.com/dust-tt/dust-labs)
- [Tools — dust-github-action](https://github.com/dust-tt/dust-github-action)
- [Tools — Dust n8n node](https://github.com/dust-tt/dust-n8n-node)
- [Tools — Dust Raycast extension](https://github.com/dust-tt/raycast-extension)
- [Tools — browse (agentic browser-use CLI)](https://github.com/dust-tt/browse)
- [Tools — srchd (research agents harness)](https://github.com/dust-tt/srchd)
- [BrowserExtension — Dust Chrome Extension](https://dust.tt/home/chrome-extension)
- [Postman — Dust Postman collection](https://app.getpostman.com/run-collection/34241185-c7e0fdbe-b2c5-47d5-a923-8244d45cd95e)
- [OpenAPI — Dust master OpenAPI 3.0](https://dust.tt/swagger.json)
- [AcademyMode — Dust Academy](https://dust.tt/academy)
- [Blog — blog.dust.tt](https://blog.dust.tt)
- [Forum — Dust Community (Slack)](https://dust-community.tightknit.community/join)
- [StatusPage](https://status.dust.tt)
- [LinkedIn](https://www.linkedin.com/company/dust-tt)
- [Twitter](https://twitter.com/dust4ai)

## Integrations

Slack · Notion (MCP) · GitHub · Google Drive · Confluence · Salesforce · HubSpot · Zendesk · Jira · BigQuery — full list at [dust.tt/integrations](https://dust.tt/integrations).

## Solutions

Sales · Customer Support · Marketing · Engineering · Data & Analytics · Knowledge · IT · Legal · Recruiting & People

## Industries

B2B SaaS · Financial Services · Consulting · Insurance · Marketplace · Retail & E-commerce

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Dust Agents API](openapi/dust-agents-api-openapi.yml)
- [Dust Conversations API](openapi/dust-conversations-api-openapi.yml)
- [Dust Data Sources API](openapi/dust-datasources-api-openapi.yml)
- [Dust MCP API](openapi/dust-mcp-api-openapi.yml)
- [Dust Apps API](openapi/dust-apps-api-openapi.yml)
- [Dust Search API](openapi/dust-search-api-openapi.yml)
- [Dust Skills API](openapi/dust-skills-api-openapi.yml)
- [Dust Triggers API](openapi/dust-triggers-api-openapi.yml)
- [Dust Workspace API](openapi/dust-workspace-api-openapi.yml)

### JSON Schema

- [Agent Configuration](json-schema/dust-agent-configuration-schema.json)
- [Conversation](json-schema/dust-conversation-schema.json)
- [Data Source](json-schema/dust-datasource-schema.json)
- [Document](json-schema/dust-document-schema.json)
- [Skill](json-schema/dust-skill-schema.json)

### JSON-LD

- [Dust Context](json-ld/dust-context.jsonld)

### Capabilities (Naftiko)

- [Agents](capabilities/agents-agents.yaml)
- [Conversations](capabilities/conversations-conversations.yaml)
- [Data Sources](capabilities/datasources-datasources.yaml)
- [MCP](capabilities/mcp-mcp.yaml)
- [Apps](capabilities/apps-apps.yaml)
- [Search](capabilities/search-search.yaml)
- [Skills](capabilities/skills-skills.yaml)
- [Triggers](capabilities/triggers-triggers.yaml)
- [Workspace](capabilities/workspace-workspace.yaml)

### Commercial artifacts

- [Plans / Pricing](plans/dust-plans-pricing.yml)
- [Rate Limits](rate-limits/dust-rate-limits.yml)
- [FinOps Definition](finops/dust-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
