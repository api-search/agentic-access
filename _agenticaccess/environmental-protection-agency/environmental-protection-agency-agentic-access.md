---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: environmental-protection-agency-openapi.yml
  format: yaml
  label: EPA Envirofacts Data Service API
  slug: envirofacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/environmental-protection-agency/refs/heads/main/openapi/environmental-protection-agency-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Environmental Protection Agency Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Environmental Protection Agency exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Environmental Protection Agency
provider_slug: environmental-protection-agency
slug: environmental-protection-agency-agentic-access
source_filename: environmental-protection-agency-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/environmental-protection-agency-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /efservice/{table}/{format}\n  method: get\n  operationId: queryEnvirofactsTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /efservice/{table}/{column}/{operator}/{value}/{format}\n  method: get\n  operationId: queryEnvirofactsFiltered\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /dmapservice/getEnvirofactsUVHOURLY/ZIP/{zip}/{format}\n  method: get\n  operationId: getUvHourlyByZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dmapservice/getEnvirofactsUVHOURLY/CITY/{city}/STATE/{state}/{format}\n  method: get\n  operationId: getUvHourlyByCityState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dmapservice/getEnvirofactsUVDAILY/ZIP/{zip}/{format}\n  method: get\n  operationId: getUvDailyByZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dmapservice/getEnvirofactsUVDAILY/CITY/{city}/STATE/{state}/{format}\n  method: get\n  operationId: getUvDailyByCityState\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/environmental-protection-agency/refs/heads/main/agentic-access/environmental-protection-agency-agentic-access.yml
summary_line: 6 operations
tags:
- Environment
- Federal Government
- Air Quality
- Open Data
---
