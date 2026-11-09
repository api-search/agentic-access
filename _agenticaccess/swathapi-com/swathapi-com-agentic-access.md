---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 11
api_specs:
- filename: swathapi-com-billing-api-openapi.yml
  format: yaml
  label: swathapi-com Billing API
  slug: swathapi-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swathapi-com/openapi/swathapi-com-billing-api-openapi.yml
- filename: swathapi-com-monitors-api-openapi.yml
  format: yaml
  label: swathapi-com Monitors API
  slug: swathapi-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swathapi-com/openapi/swathapi-com-monitors-api-openapi.yml
- filename: swathapi-com-property-api-openapi.yml
  format: yaml
  label: swathapi-com Property API
  slug: swathapi-com-property-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swathapi-com/openapi/swathapi-com-property-api-openapi.yml
- filename: swathapi-com-signup-api-openapi.yml
  format: yaml
  label: swathapi-com Signup API
  slug: swathapi-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swathapi-com/openapi/swathapi-com-signup-api-openapi.yml
- filename: swathapi-com-storms-api-openapi.yml
  format: yaml
  label: swathapi-com Storms API
  slug: swathapi-com-storms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swathapi-com/openapi/swathapi-com-storms-api-openapi.yml
- filename: swathapi-com-swaths-api-openapi.yml
  format: yaml
  label: swathapi-com Swaths API
  slug: swathapi-com-swaths-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swathapi-com/openapi/swathapi-com-swaths-api-openapi.yml
- filename: swathapi-com-usage-api-openapi.yml
  format: yaml
  label: swathapi-com Usage API
  slug: swathapi-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swathapi-com/openapi/swathapi-com-usage-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Swathapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 16
overview: 'swathapi-com exposes 16 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: swathapi-com
provider_slug: swathapi-com
slug: swathapi-com-agentic-access
source_filename: swathapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/swathapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 11\n    acting: 5\n  by_consequence:\n    read: 11\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/swaths/geometry\n  method: get\n  operationId: swath_geometry_in_bbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storms/proof\n  method: get\n  operationId: storm_proof_document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/storms/at\n  method: get\n  operationId: storms_at_point\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storms/at\n  method: post\n  operationId: storms_at_points\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storms\n  method: get\n  operationId: find_storms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swaths/{id}\n  method: get\n  operationId: get_swath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swaths/{id}/geometry\n\
  \  method: get\n  operationId: get_swath_geometry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swaths/{id}/properties\n  method: get\n  operationId: get_swath_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swaths/{id}/properties/quote\n  method: get\n  operationId: get_report_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swaths/{id}/email-report\n  method: post\n  operationId: email_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/property\n  method: get\n  operationId: lookup_property\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors\n  method: get\n  operationId: list_monitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors\n  method: post\n  operationId: create_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: get_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/billing/checkout\n  method: post\n  operationId: create_checkout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signup\n  method: post\n  operationId: create_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/swathapi-com/agentic-access/swathapi-com-agentic-access.yml
summary_line: 16 operations · 5 acting
tags:
- Company
- Weather
- Storm
- Artificial Intelligence
- NOAA
---
