---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: 1211holding-com-art-api-openapi.yml
  format: yaml
  label: 1211 Art API
  slug: 1211holding-com-art-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/1211holding-com/openapi/1211holding-com-art-api-openapi.yml
- filename: 1211holding-com-catalog-api-openapi.yml
  format: yaml
  label: 1211 Catalog API
  slug: 1211holding-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/1211holding-com/openapi/1211holding-com-catalog-api-openapi.yml
- filename: 1211holding-com-designs-api-openapi.yml
  format: yaml
  label: 1211 Designs API
  slug: 1211holding-com-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/1211holding-com/openapi/1211holding-com-designs-api-openapi.yml
consequence_counts:
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 1211Holding Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: '1211 exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: '1211'
provider_slug: 1211holding-com
slug: 1211holding-com-agentic-access
source_filename: 1211holding-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/1211holding-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 1\n    acting: 2\n  by_consequence:\n    read: 1\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/catalog\n  method: get\n  operationId: list_items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/art\n  method: post\n  operationId: check_art\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/designs\n  method: post\n  operationId: create_design\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/1211holding-com/agentic-access/1211holding-com-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- Print on Demand
- E-Commerce
- Merchandise
- Custom Products
---
