---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: dtmframe-com-compare-api-openapi.yml
  format: yaml
  label: DTMFRAME Compare API
  slug: dtmframe-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dtmframe-com/openapi/dtmframe-com-compare-api-openapi.yml
- filename: dtmframe-com-deals-api-openapi.yml
  format: yaml
  label: DTMFRAME Deals API
  slug: dtmframe-com-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dtmframe-com/openapi/dtmframe-com-deals-api-openapi.yml
- filename: dtmframe-com-products-api-openapi.yml
  format: yaml
  label: DTMFRAME Products API
  slug: dtmframe-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dtmframe-com/openapi/dtmframe-com-products-api-openapi.yml
- filename: dtmframe-com-resolve-api-openapi.yml
  format: yaml
  label: DTMFRAME Resolve API
  slug: dtmframe-com-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dtmframe-com/openapi/dtmframe-com-resolve-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dtmframe Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/resolve/
operation_count: 6
overview: 'DTMFRAME exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DTMFRAME
provider_slug: dtmframe-com
slug: dtmframe-com-agentic-access
source_filename: dtmframe-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dtmframe-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    physical: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/products/\n  method: get\n  operationId: search_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products/search/\n  method: post\n  operationId: search_products_by_name\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/products/{id}/offers/\n  method: get\n  operationId: get_current_offers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deals/\n  method: get\n  operationId: list_deals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/resolve/\n  method: post\n  operationId: resolve_purchase_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/compare/\n  method: post\n  operationId: compare_products\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/dtmframe-com/agentic-access/dtmframe-com-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Company
- Music
- Price-Tracking
- Japanese
- Plugins
---
