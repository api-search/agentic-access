---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 17
api_specs:
- filename: cuvo-co-a2a-api-openapi.yml
  format: yaml
  label: Cuvo Health A2a API
  slug: cuvo-co-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-a2a-api-openapi.yml
- filename: cuvo-co-acp-api-openapi.yml
  format: yaml
  label: Cuvo Health Acp API
  slug: cuvo-co-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-acp-api-openapi.yml
- filename: cuvo-co-content-api-openapi.yml
  format: yaml
  label: Cuvo Health Content API
  slug: cuvo-co-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-content-api-openapi.yml
- filename: cuvo-co-discovery-api-openapi.yml
  format: yaml
  label: Cuvo Health Discovery API
  slug: cuvo-co-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-discovery-api-openapi.yml
- filename: cuvo-co-mcp-api-openapi.yml
  format: yaml
  label: Cuvo Health MCP API
  slug: cuvo-co-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-mcp-api-openapi.yml
- filename: cuvo-co-status-api-openapi.yml
  format: yaml
  label: Cuvo Health Status API
  slug: cuvo-co-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-status-api-openapi.yml
consequence_counts:
  physical: 5
  read: 17
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cuvo Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/a2a
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/checkout_sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/checkout_sessions/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/checkout_sessions/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acp/checkout_sessions/{id}/complete
operation_count: 25
overview: 'Cuvo Health exposes 25 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 3 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cuvo Health
provider_slug: cuvo-co
slug: cuvo-co-agentic-access
source_filename: cuvo-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cuvo-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 17\n    acting: 8\n  by_consequence:\n    read: 17\n    write: 3\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth.md\n  method: get\n\
  \  operationId: getAuthDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compare/{slug}.md\n  method: get\n  operationId: getComparisonMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: getAgentCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent.json\n  method: get\n  operationId: getAgentCardLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/acp.json\n  method: get\n  operationId: getAcpDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp.json\n  method: get\n  operationId: getMcpManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: callMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /docs/mcp\n  method: post\n  operationId: callDocsMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ask\n  method: get\n\
  \  operationId: ask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: post\n  operationId: askPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/articles\n  method: get\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/comparisons\n  method: get\n  operationId: listComparisons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp-docs.json\n  method: get\n  operationId: getDocsMcpManifest\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp/server-card.json\n  method: get\n  operationId: getMcpServerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-skills/index.json\n  method: get\n  operationId: getAgentSkillsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ai-catalog.json\n  method: get\n  operationId: getAiCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/a2a\n  method: post\n  operationId: sendA2aMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/checkout_sessions\n  method: post\n  operationId: createAcpCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/checkout_sessions/{id}\n  method: get\n  operationId: getAcpCheckoutSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/acp/checkout_sessions/{id}\n  method: post\n  operationId: updateAcpCheckoutSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/checkout_sessions/{id}/complete\n  method: post\n  operationId: completeAcpCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acp/checkout_sessions/{id}/cancel\n  method: post\n  operationId: cancelAcpCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cuvo-co/agentic-access/cuvo-co-agentic-access.yml
summary_line: 25 operations · 8 acting
tags:
- Telehealth
- White‑Label Platform
- Pharmacy Fulfillment
- Brand Licensing
---
