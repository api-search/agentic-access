---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: boltena-com-default-api-openapi.yml
  format: yaml
  label: 볼테나 기본 API
  slug: boltena-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boltena-com/openapi/boltena-com-default-api-openapi.yml
- filename: boltena-com-eqp-api-openapi.yml
  format: yaml
  label: 볼테나 EQP 모듈 필요 API
  slug: boltena-com-eqp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boltena-com/openapi/boltena-com-eqp-api-openapi.yml
- filename: boltena-com-hr-api-openapi.yml
  format: yaml
  label: 볼테나 HR 모듈 필요 API
  slug: boltena-com-hr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boltena-com/openapi/boltena-com-hr-api-openapi.yml
consequence_counts:
  read: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Boltena Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: '볼테나 exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 볼테나
provider_slug: boltena-com
slug: boltena-com-agentic-access
source_filename: boltena-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/boltena-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 2\n    acting: 6\n  by_consequence:\n    read: 2\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/ext/ping\n  method: get\n  operationId: get_api_ext_ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ext/masters/{entity}\n  method: get\n  operationId: get_api_ext_masters_entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ext/production/result\n\
  \  method: post\n  operationId: post_api_ext_production_result\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ext/production/result/{extRef}\n  method: delete\n  operationId: delete_api_ext_production_result_extref\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ext/eqp/downtime\n  method: post\n  operationId: post_api_ext_eqp_downtime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ext/eqp/downtime/{extRef}\n  method: delete\n  operationId: delete_api_ext_eqp_downtime_extref\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ext/mcp\n  method: post\n  operationId: post_api_ext_mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ext/attendance\n  method: post\n  operationId: post_api_ext_attendance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/boltena-com/agentic-access/boltena-com-agentic-access.yml
summary_line: 8 operations · 6 acting
tags:
- ERP
- Human Resources
- MES
- Business Intelligence
---
