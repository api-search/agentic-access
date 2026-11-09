---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: dibind-com-duty-api-openapi.yml
  format: yaml
  label: Dibblee Industries Duty API
  slug: dibind-com-duty-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dibind-com/openapi/dibind-com-duty-api-openapi.yml
- filename: dibind-com-reference-api-openapi.yml
  format: yaml
  label: Dibblee Industries Reference API
  slug: dibind-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dibind-com/openapi/dibind-com-reference-api-openapi.yml
- filename: dibind-com-status-api-openapi.yml
  format: yaml
  label: Dibblee Industries Status API
  slug: dibind-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dibind-com/openapi/dibind-com-status-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dibind Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Dibblee Industries exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dibblee Industries
provider_slug: dibind-com
slug: dibind-com-agentic-access
source_filename: dibind-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dibind-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /duty\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tariff/{hs_code}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /measures\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /measures/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/data\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dibind-com/agentic-access/dibind-com-agentic-access.yml
summary_line: 7 operations
tags:
- Company
- Defence
- Supply Chain
- Marine Hardware
- NATO
- Logistics
- Artificial Intelligence
- MCP
- Canada
---
