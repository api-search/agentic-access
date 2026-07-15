---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: openfema-fire-data-openapi.yml
  format: yaml
  label: OpenFEMA Fire Data API
  slug: openfema-fire-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-fire-administration/refs/heads/main/openapi/openfema-fire-data-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: United States Fire Administration Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'United States Fire Administration exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: United States Fire Administration
provider_slug: united-states-fire-administration
slug: united-states-fire-administration-agentic-access
source_filename: united-states-fire-administration-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openfema-fire-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/OpenFemaDataSets\n  method: get\n  operationId: listDataSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/OpenFemaDataSetFields\n  method: get\n  operationId: listDataSetFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/FemaWebDisasterDeclarations\n \
  \ method: get\n  operationId: getDisasterDeclarations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/DisasterDeclarationsSummaries\n  method: get\n  operationId: getDisasterDeclarationsSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-fire-administration/refs/heads/main/agentic-access/united-states-fire-administration-agentic-access.yml
summary_line: 4 operations
tags:
- Federal Government
- Fire Safety
- Emergency Management
- Public Safety
- FEMA
---
