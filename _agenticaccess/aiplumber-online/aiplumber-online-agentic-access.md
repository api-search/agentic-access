---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: aiplumber-online-gta-api-openapi.yml
  format: yaml
  label: GTA AI Plumber Gta API
  slug: aiplumber-online-gta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiplumber-online/openapi/aiplumber-online-gta-api-openapi.yml
- filename: aiplumber-online-health-api-openapi.yml
  format: yaml
  label: GTA AI Plumber Health API
  slug: aiplumber-online-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiplumber-online/openapi/aiplumber-online-health-api-openapi.yml
consequence_counts:
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aiplumber Online Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'GTA AI Plumber exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GTA AI Plumber
provider_slug: aiplumber-online
slug: aiplumber-online-agentic-access
source_filename: aiplumber-online-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aiplumber-online-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 1\n    connected: 1\n  by_consequence:\n    write: 1\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/gta/requests\n  method: post\n  operationId: findGtaPlumbersAndRequestQuotes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aiplumber-online/agentic-access/aiplumber-online-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Plumbing
- Artificial Intelligence
- Marketplace
- GTA
- Services
---
