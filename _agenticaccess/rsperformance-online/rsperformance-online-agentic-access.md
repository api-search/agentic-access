---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: rsperformance-online-ai-gateway-openapi.yml
  format: yaml
  label: RS Performance AI Gateway API
  slug: rs-performance-ai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsperformance-online/refs/heads/main/openapi/rsperformance-online-ai-gateway-openapi.yml
consequence_counts:
  read: 3
description: 'Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/. Curated 2026-09-19: all three operations are reads; the surface has no write, so no human-in-the-loop trigger applies. Note the provider''s OTHER agent surfaces do have writes outside this OpenAPI — A2A message/send creates a task and the MCP tools write_intake_note and diagnostic_ingest_brand_knowledge write to the provider''s store (see mcp/ and conventions/).'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Rsperformance Online Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'RS Performance exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RS Performance
provider_slug: rsperformance-online
slug: rsperformance-online-agentic-access
source_filename: rsperformance-online-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/rsperformance-online-ai-gateway-openapi.yml (heuristic classification by derive-agentic-access.py,\n  then curated against the OpenAPI operation descriptions and the live probe on 2026-09-19)\ndescription: 'Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance\n  starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.\n  Curated 2026-09-19: all three operations are reads; the surface has no write, so no human-in-the-loop trigger\n  applies. Note the provider''s OTHER agent surfaces do have writes outside this OpenAPI — A2A message/send creates\n  a task and the MCP tools write_intake_note and diagnostic_ingest_brand_knowledge write to the provider''s store\n  (see mcp/ and conventions/).'\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required:\
  \ 0\noperations:\n- path: /api/search\n  method: post\n  operationId: semanticSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 3600\n    escalation:\n      human-in-the-loop: none\n      triggers: []\n    audit: recommended\n  x-curation-note: Reclassified from acting/write to connected/read. The heuristic keyed on the POST verb, but the\n    provider's OpenAPI describes the operation as retrieval ('Runs answer-first retrieval across services, symptom\n    pages, DTC references, repair reports, and editorial content'), its request body carries only a query and a\n    limit, and the live call created no resource. It is a POST-shaped read.\n- path: /.well-known/freshness.json\n  method: get\n  operationId: gatewayFreshness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/answer-routing.json\n\
  \  method: get\n  operationId: gatewayAnswerRouting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rsperformance-online/refs/heads/main/agentic-access/rsperformance-online-agentic-access.yml
summary_line: 3 operations
tags:
- Automotive
- Auto Repair
- Vehicle Diagnostics
- OBD-II
- Fault Codes
- Knowledge Base
- Semantic Search
- A2A
- MCP
- agent-native
- Local Business
- Poland
---
