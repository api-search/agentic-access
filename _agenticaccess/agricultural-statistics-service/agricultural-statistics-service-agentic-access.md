---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: agricultural-statistics-service-quickstats-api.yaml
  format: yaml
  label: USDA NASS QuickStats API
  slug: quickstats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/openapi/agricultural-statistics-service-quickstats-api.yaml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agricultural Statistics Service Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Agricultural Statistics Service exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agricultural Statistics Service
provider_slug: agricultural-statistics-service
slug: agricultural-statistics-service-agentic-access
source_filename: agricultural-statistics-service-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/agricultural-statistics-service-quickstats-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api_GET\n  method: get\n  operationId: getStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_param_values\n  method: get\n  operationId: getParamValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_counts\n  method: get\n  operationId:\
  \ getCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/agentic-access/agricultural-statistics-service-agentic-access.yml
summary_line: 3 operations
tags:
- Agriculture
- Federal Government
- Statistics
- Open Data
- Geospatial
---
