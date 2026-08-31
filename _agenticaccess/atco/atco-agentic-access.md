---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: atco-query-api-openapi.yml
  format: yaml
  label: ATCO Query API
  slug: atco-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atco/refs/heads/main/openapi/atco-query-api-openapi.yml
- filename: atco-service-api-openapi.yml
  format: yaml
  label: ATCO Service API
  slug: atco-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atco/refs/heads/main/openapi/atco-service-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atco Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'ATCO exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ATCO
provider_slug: atco
slug: atco-agentic-access
source_filename: atco-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/atco-electric-hosting-capacity-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\n  note: >-\n    All five operations are reads. The service advertises ArcGIS capabilities \"Query\" only —\n    there is no write surface. The POST form of /0/query was hand-corrected from the derive\n    script's HTTP-method heuristic, which had classified it acting/write.\noperations:\n- path: /\n  method: get\n  operationId: getFeatureServiceInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /0\n  method: get\n  operationId: getHostingCapacityLayerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/query\n  method: get\n  operationId: queryHostingCapacity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/query\n  method: post\n  operationId: queryHostingCapacityByPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n  note: >-\n    Hand-corrected from the derive script's method heuristic. This is a POST-shaped READ:\n    the service advertises capabilities \"Query\" only, so this operation is the form-encoded\n    variant of the GET query and mutates nothing.\n- path: /0/queryTopFeatures\n  method: get\n  operationId: queryTopHostingCapacityFeatures\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atco/refs/heads/main/agentic-access/atco-agentic-access.yml
summary_line: 5 operations
tags:
- Energy
- Canada
- Utilities
- Electricity
- Gas
- Grid
- Distribution
- Transmission
- DER
- Solar
- Renewables
- Open Data
- Geospatial
- Alberta
---
