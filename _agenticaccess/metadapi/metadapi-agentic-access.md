---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: metadapi-zipc-api-openapi.yml
  format: yaml
  label: Metadapi Zipc API
  slug: metadapi-zipc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metadapi/refs/heads/main/openapi/metadapi-zipc-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Metadapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Metadapi exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Metadapi
provider_slug: metadapi
slug: metadapi-agentic-access
source_filename: metadapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/metadapi-zipcode-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /zipc/v1/zipcodes/{zipcode}\n  method: get\n  operationId: get-zipcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zipc/v1/zipcodes\n  method: get\n  operationId: get-zipcodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zipc/v1/distance\n  method: get\n  operationId:\
  \ get-distance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zipc/v1/radius\n  method: get\n  operationId: get-radius\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zipc/v1/msagroups\n  method: get\n  operationId: get-msagroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zipc/v1/msagroups/{msaCode}\n  method: get\n  operationId: get-msagroups-msacode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zipc/v1\n  method: get\n  operationId: get-zipc-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metadapi/refs/heads/main/agentic-access/metadapi-agentic-access.yml
summary_line: 7 operations
tags:
- Company
- Data
- Reference
- JSON
---
