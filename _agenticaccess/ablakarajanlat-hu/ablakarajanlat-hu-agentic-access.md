---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: ablakarajanlat-hu-agent-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Agent API
  slug: ablakarajanlat-hu-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-agent-api-openapi.yml
- filename: ablakarajanlat-hu-ai-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat AI API
  slug: ablakarajanlat-hu-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-ai-api-openapi.yml
- filename: ablakarajanlat-hu-coverage-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Coverage API
  slug: ablakarajanlat-hu-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-coverage-api-openapi.yml
- filename: ablakarajanlat-hu-estimate-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Estimate API
  slug: ablakarajanlat-hu-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-estimate-api-openapi.yml
- filename: ablakarajanlat-hu-knowledge-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Knowledge API
  slug: ablakarajanlat-hu-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-knowledge-api-openapi.yml
- filename: ablakarajanlat-hu-mcp-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat MCP API
  slug: ablakarajanlat-hu-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-mcp-api-openapi.yml
- filename: ablakarajanlat-hu-quote-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Quote API
  slug: ablakarajanlat-hu-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-quote-api-openapi.yml
- filename: ablakarajanlat-hu-support-api-openapi.yml
  format: yaml
  label: Ablak Árajánlat Support API
  slug: ablakarajanlat-hu-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ablakarajanlat-hu/openapi/ablakarajanlat-hu-support-api-openapi.yml
consequence_counts:
  read: 9
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ablakarajanlat Hu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Ablak Árajánlat exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ablak Árajánlat
provider_slug: ablakarajanlat-hu
slug: ablakarajanlat-hu-agentic-access
source_filename: ablakarajanlat-hu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/ablakarajanlat-hu-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 9\n    acting: 7\n  by_consequence:\n    read: 9\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/quote/custom-calculate\n  method: post\n  operationId: getCustomPriceEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: mcpJsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/coverage\n  method: get\n  operationId: getCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/catalog\n  method: get\n  operationId: getStockCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/estimate\n  method: get\n  operationId: estimateFromQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/estimate\n  method: post\n  operationId: estimateWindowPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/ast\n  method: post\n  operationId: astBridge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/mcp/quote-from-query\n  method: post\n  operationId: mcpQuoteFromQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/mcp/estimate-from-query\n  method: post\n  operationId: mcpEstimateFromQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/search\n  method: get\n  operationId: searchCatalogAndKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/quote\n  method: post\n  operationId: createQuoteDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/quote\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/pdf\n\
  \  method: get\n  operationId: getQuotePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/knowledge\n  method: get\n  operationId: getKnowledgeIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /knowledge/search\n  method: get\n  operationId: searchKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/support/handoff\n  method: post\n  operationId: requestHumanSupportHandoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ablakarajanlat-hu/agentic-access/ablakarajanlat-hu-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- Windows
- Calculator
- Construction
- Hungary
- Pricing
---
