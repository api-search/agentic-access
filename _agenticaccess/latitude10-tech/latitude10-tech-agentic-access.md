---
acting_count: 0
action_class_counts:
  connected: 24
api_specs:
- filename: latitude10-tech-agent-readiness-api-openapi.yml
  format: yaml
  label: latitude10-tech Agent readiness API
  slug: latitude10-tech-agent-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latitude10-tech/openapi/latitude10-tech-agent-readiness-api-openapi.yml
- filename: latitude10-tech-design-packs-api-openapi.yml
  format: yaml
  label: latitude10-tech Design packs API
  slug: latitude10-tech-design-packs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latitude10-tech/openapi/latitude10-tech-design-packs-api-openapi.yml
- filename: latitude10-tech-developer-kits-api-openapi.yml
  format: yaml
  label: latitude10-tech Developer kits API
  slug: latitude10-tech-developer-kits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latitude10-tech/openapi/latitude10-tech-developer-kits-api-openapi.yml
consequence_counts:
  read: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Latitude10 Tech Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'latitude10-tech exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: latitude10-tech
provider_slug: latitude10-tech
slug: latitude10-tech-agentic-access
source_filename: latitude10-tech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/latitude10-tech-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 24\n  by_consequence:\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /api/agent-products/starter-kit\n  method: get\n  operationId: buyStarterKit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agent-payments-kit\n  method: get\n  operationId: buyAgentPaymentsKit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agent-production-kit\n\
  \  method: get\n  operationId: buyAgentProductionKit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/mcp-server-kit\n  method: get\n  operationId: buyMcpServerKit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agent-gateway\n  method: get\n  operationId: buyAgentGateway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agent-spend-guard\n  method: get\n  operationId: buyAgentSpendGuard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agent-trace-kit\n  method: get\n  operationId: buyAgentTraceKit\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agent-eval-kit\n  method: get\n  operationId: buyAgentEvalKit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agentify-api\n  method: get\n  operationId: buyAgentifyApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agentify-api-python\n  method: get\n  operationId: buyAgentifyApiPython\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agentify-api-dotnet\n  method: get\n  operationId: buyAgentifyApiDotnet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agentify-api-java\n  method: get\n  operationId: buyAgentifyApiJava\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agentify-api-ruby\n  method: get\n  operationId: buyAgentifyApiRuby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agentify-api-php\n  method: get\n  operationId: buyAgentifyApiPhp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/agent-production-stack\n  method: get\n  operationId: buyAgentProductionStack\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/design-pack-ledger\n  method: get\n  operationId: buyDesignPackLedger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/design-pack-ledger-project\n  method: get\n  operationId: buyDesignPackLedgerProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/design-pack-terminal\n  method: get\n  operationId: buyDesignPackTerminal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/design-pack-terminal-project\n  method: get\n  operationId: buyDesignPackTerminalProject\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/design-pack-atelier\n  method: get\n  operationId: buyDesignPackAtelier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/design-pack-atelier-project\n  method: get\n  operationId: buyDesignPackAtelierProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/design-pack-meridian\n  method: get\n  operationId: buyDesignPackMeridian\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-products/design-packs-bundle\n  method: get\n  operationId: buyDesignPacksBundle\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/readiness/report\n  method: post\n  operationId: getAgentReadinessReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/latitude10-tech/agentic-access/latitude10-tech-agentic-access.yml
summary_line: 24 operations
tags:
- API Platform
- MCP
- Developer Tools
- AI Agents
- OpenAPI
---
