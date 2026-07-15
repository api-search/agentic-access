---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: agricultural-marketing-service-mars-api.yaml
  format: yaml
  label: USDA AMS MARS API (MyMarketNews)
  slug: usda-ams-mars-api-mymarketnews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/openapi/agricultural-marketing-service-mars-api.yaml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agricultural Marketing Service Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Agricultural Marketing Service exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
slug: agricultural-marketing-service-agentic-access
source_filename: agricultural-marketing-service-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/agricultural-marketing-service-mars-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{slug_id}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offices\n  method: get\n  operationId: listOffices\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/agentic-access/agricultural-marketing-service-agentic-access.yml
summary_line: 3 operations
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
---
