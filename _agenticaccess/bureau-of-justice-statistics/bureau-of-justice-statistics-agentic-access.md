---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: bureau-of-justice-statistics-openapi.yml
  format: yaml
  label: NIBRS National Estimates API
  slug: nibrs-national-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-justice-statistics/refs/heads/main/openapi/bureau-of-justice-statistics-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bureau Of Justice Statistics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Bureau of Justice Statistics exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bureau of Justice Statistics
provider_slug: bureau-of-justice-statistics
slug: bureau-of-justice-statistics-agentic-access
source_filename: bureau-of-justice-statistics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bureau-of-justice-statistics-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /resource/r32q-bdaw.json\n  method: get\n  operationId: getViolentIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/iv7i-eah6.json\n  method: get\n  operationId: getPropertyIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/x3sz-eb6y.json\n\
  \  method: get\n  operationId: getViolentOffenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/kj7p-vx4s.json\n  method: get\n  operationId: getPropertyOffenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/ms42-n765.json\n  method: get\n  operationId: getVictimizationCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/uy37-xgmh.json\n  method: get\n  operationId: getVictimizationRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-justice-statistics/refs/heads/main/agentic-access/bureau-of-justice-statistics-agentic-access.yml
summary_line: 6 operations
tags:
- Crime
- Federal Government
- Justice
- Statistics
- Victimization
- Recidivism
---
