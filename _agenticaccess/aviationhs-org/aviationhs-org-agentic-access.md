---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: aviationhs-org-aircraft-api-openapi.yml
  format: yaml
  label: AviationHS Aircraft API
  slug: aviationhs-org-aircraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviationhs-org/openapi/aviationhs-org-aircraft-api-openapi.yml
- filename: aviationhs-org-airports-api-openapi.yml
  format: yaml
  label: AviationHS Airports API
  slug: aviationhs-org-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviationhs-org/openapi/aviationhs-org-airports-api-openapi.yml
- filename: aviationhs-org-runway-api-openapi.yml
  format: yaml
  label: AviationHS Runway API
  slug: aviationhs-org-runway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviationhs-org/openapi/aviationhs-org-runway-api-openapi.yml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aviationhs Org Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'AviationHS exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AviationHS
provider_slug: aviationhs-org
slug: aviationhs-org-agentic-access
source_filename: aviationhs-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/aviationhs-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/airports\n  method: get\n  operationId: search_airports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aircraft\n  method: get\n  operationId: list_aircraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runway\n  method: get\n  operationId: check_runway\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aviationhs-org/agentic-access/aviationhs-org-agentic-access.yml
summary_line: 3 operations
tags:
- Private-Jet
- Charter
- Aviation
- quote-engine
- MCP
---
