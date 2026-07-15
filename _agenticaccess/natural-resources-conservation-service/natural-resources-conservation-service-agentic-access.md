---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 2
api_specs:
- filename: natural-resources-conservation-service-openapi.yml
  format: yaml
  label: NRCS Soil Data Access
  slug: soil-data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-resources-conservation-service/refs/heads/main/openapi/natural-resources-conservation-service-openapi.yml
consequence_counts:
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Natural Resources Conservation Service Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Natural Resources Conservation Service exposes 4 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Natural Resources Conservation Service
provider_slug: natural-resources-conservation-service
slug: natural-resources-conservation-service-agentic-access
source_filename: natural-resources-conservation-service-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/natural-resources-conservation-service-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 2\n    connected: 2\n  by_consequence:\n    write: 2\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /Tabular/post.rest\n  method: post\n  operationId: runQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Tabular/SDMTabularService.asmx\n  method: post\n  operationId: runQuerySoap\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Spatial/SDMWGS84Geographic.wfs\n  method: get\n  operationId: wfsWgs84\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Spatial/SDM.wms\n  method: get\n  operationId: wmsSoils\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natural-resources-conservation-service/refs/heads/main/agentic-access/natural-resources-conservation-service-agentic-access.yml
summary_line: 4 operations · 2 acting
tags:
- Federal Government
- Agriculture
- Conservation
- Soil
- Natural Resources
---
