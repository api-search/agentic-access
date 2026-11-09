---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 14
api_specs:
- filename: cyclesite-co-uk-mcp-api-api-openapi.yml
  format: yaml
  label: Cyclesite MCP API
  slug: cyclesite-co-uk-mcp-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclesite-co-uk/openapi/cyclesite-co-uk-mcp-api-api-openapi.yml
consequence_counts:
  read: 14
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cyclesite Co Uk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Cyclesite exposes 16 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cyclesite
provider_slug: cyclesite-co-uk
slug: cyclesite-co-uk-agentic-access
source_filename: cyclesite-co-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cyclesite-co-uk-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 14\n    acting: 2\n  by_consequence:\n    read: 14\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/mcp/brand/{slug}/models\n  method: get\n  operationId: mcpListBrandModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/brands\n  method: get\n  operationId: mcpListBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/buying-guide\n\
  \  method: get\n  operationId: mcpSearchBuyingGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/by-location\n  method: get\n  operationId: mcpSearchByLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/draft-listing\n  method: post\n  operationId: mcpDraftListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/listing/{slug}\n  method: get\n  operationId: getListingDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/mcp/listing/{slug}/grade\n  method: get\n  operationId: mcpGradeListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/model\n  method: get\n  operationId: getModelInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/recent\n  method: get\n  operationId: mcpListRecent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/recommend\n  method: get\n  operationId: mcpRecommend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/search\n  method: get\n  operationId: searchBikes\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/similar/{slug}\n  method: get\n  operationId: mcpFindSimilar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/size-guide\n  method: get\n  operationId: mcpGetSizeGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/spec-sheet\n  method: get\n  operationId: mcpGetSpecSheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/stolen-check\n  method: post\n  operationId: checkStolen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/valuation\n  method: get\n  operationId: getValuation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cyclesite-co-uk/agentic-access/cyclesite-co-uk-agentic-access.yml
summary_line: 16 operations · 2 acting
tags:
- Bike Marketplace
- Used Bikes
- United Kingdom
- Marketplace
- Community
---
