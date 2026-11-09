---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: assistant247-net-appliances-api-openapi.yml
  format: yaml
  label: AssistAnt 24/7 Appliances API
  slug: assistant247-net-appliances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assistant247-net/openapi/assistant247-net-appliances-api-openapi.yml
- filename: assistant247-net-assistant-pro-directory-api-openapi.yml
  format: yaml
  label: AssistAnt 24/7 AssistAnt Pro Directory API
  slug: assistant247-net-assistant-pro-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assistant247-net/openapi/assistant247-net-assistant-pro-directory-api-openapi.yml
- filename: assistant247-net-pros-api-openapi.yml
  format: yaml
  label: AssistAnt 24/7 Pros API
  slug: assistant247-net-pros-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assistant247-net/openapi/assistant247-net-pros-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Assistant247 Net Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'AssistAnt 24/7 exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AssistAnt 24/7
provider_slug: assistant247-net
slug: assistant247-net-agentic-access
source_filename: assistant247-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/assistant247-net-openapi.json, openapi/assistant247-net-pros-api-openapi.yml,\n  openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/pros\n  method: get\n  operationId: findPros\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pros\n  method: get\n  operationId: findPros\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pros\n\
  \  method: get\n  operationId: findPros\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pros/{slug}\n  method: get\n  operationId: getProProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{state}/{town}\n  method: get\n  operationId: getTownSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appliances/{brand}/{appliance}\n  method: get\n  operationId: getApplianceKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/assistant247-net/agentic-access/assistant247-net-agentic-access.yml
summary_line: 6 operations
tags:
- Marketplace
- Local Services
- Home Repair
- Freelancers
- Small Business
---
