---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: realworldapis-com-ai-recommend-api-openapi.yml
  format: yaml
  label: realworldapis-com Ai Recommend API
  slug: realworldapis-com-ai-recommend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realworldapis-com/openapi/realworldapis-com-ai-recommend-api-openapi.yml
- filename: realworldapis-com-apis-api-openapi.yml
  format: yaml
  label: realworldapis-com APIs API
  slug: realworldapis-com-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realworldapis-com/openapi/realworldapis-com-apis-api-openapi.yml
- filename: realworldapis-com-capabilities-json-api-openapi.yml
  format: yaml
  label: realworldapis-com Capabilities.json API
  slug: realworldapis-com-capabilities-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realworldapis-com/openapi/realworldapis-com-capabilities-json-api-openapi.yml
- filename: realworldapis-com-catalog-json-api-openapi.yml
  format: yaml
  label: realworldapis-com Catalog.json API
  slug: realworldapis-com-catalog-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realworldapis-com/openapi/realworldapis-com-catalog-json-api-openapi.yml
- filename: realworldapis-com-categories-json-api-openapi.yml
  format: yaml
  label: realworldapis-com Categories.json API
  slug: realworldapis-com-categories-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realworldapis-com/openapi/realworldapis-com-categories-json-api-openapi.yml
- filename: realworldapis-com-recommend-api-openapi.yml
  format: yaml
  label: realworldapis-com Recommend API
  slug: realworldapis-com-recommend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realworldapis-com/openapi/realworldapis-com-recommend-api-openapi.yml
- filename: realworldapis-com-research-api-openapi.yml
  format: yaml
  label: realworldapis-com Research API
  slug: realworldapis-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realworldapis-com/openapi/realworldapis-com-research-api-openapi.yml
- filename: realworldapis-com-verify-requirement-api-openapi.yml
  format: yaml
  label: realworldapis-com Verify Requirement API
  slug: realworldapis-com-verify-requirement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/realworldapis-com/openapi/realworldapis-com-verify-requirement-api-openapi.yml
consequence_counts:
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Realworldapis Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'realworldapis-com exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: realworldapis-com
provider_slug: realworldapis-com
slug: realworldapis-com-agentic-access
source_filename: realworldapis-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/realworldapis-com-mcp-openapi.json, openapi/realworldapis-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 2\n    connected: 11\n  by_consequence:\n    write: 2\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog.json\n  method: get\n  operationId: catalog\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities.json\n  method: get\n  operationId: capabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/capabilities.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify-requirement\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify-requirement\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apis/{slug}.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recommend\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai-recommend\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories.json\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /research/state-of-agent-ready-apis-2026.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/realworldapis-com/agentic-access/realworldapis-com-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Discovery
- Artificial Intelligence
- PhysicalWorld
- RealWorldAPIs
---
