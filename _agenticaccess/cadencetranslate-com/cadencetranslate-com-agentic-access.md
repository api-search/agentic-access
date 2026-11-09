---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: cadencetranslate-com-cadence-info-api-openapi.yml
  format: yaml
  label: Cadence Cadence Info API
  slug: cadencetranslate-com-cadence-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cadencetranslate-com/openapi/cadencetranslate-com-cadence-info-api-openapi.yml
- filename: cadencetranslate-com-orders-api-openapi.yml
  format: yaml
  label: Cadence Orders API
  slug: cadencetranslate-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cadencetranslate-com/openapi/cadencetranslate-com-orders-api-openapi.yml
- filename: cadencetranslate-com-public-api-openapi.yml
  format: yaml
  label: Cadence Public API
  slug: cadencetranslate-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cadencetranslate-com/openapi/cadencetranslate-com-public-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cadencetranslate Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 7
overview: 'Cadence exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cadence
provider_slug: cadencetranslate-com
slug: cadencetranslate-com-agentic-access
source_filename: cadencetranslate-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: generated\nsource: openapi/cadencetranslate-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 1\n    connected: 6\n  by_consequence:\n    physical: 1\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: post\n  operationId: create_order_orders_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: list_orders_orders_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}\n  method: get\n  operationId: get_order_orders__order_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cadence-info\n  method: get\n  operationId: cadence_info_cadence_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/jwks.json\n  method: get\n  operationId: jwks__well_known_jwks_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/editor-jwks.json\n  method: get\n  operationId: editor_jwks__well_known_editor_jwks_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cadencetranslate-com/agentic-access/cadencetranslate-com-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Company
- Language Services
- Financial Technology
- Translation
- Global Markets
---
