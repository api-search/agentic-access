---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: buyrecord-app-keys-api-openapi.yml
  format: yaml
  label: BuyRecord Keys API
  slug: buyrecord-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-keys-api-openapi.yml
- filename: buyrecord-app-merchants-api-openapi.yml
  format: yaml
  label: BuyRecord Merchants API
  slug: buyrecord-app-merchants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-merchants-api-openapi.yml
- filename: buyrecord-app-outcomes-api-openapi.yml
  format: yaml
  label: BuyRecord Outcomes API
  slug: buyrecord-app-outcomes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-outcomes-api-openapi.yml
- filename: buyrecord-app-products-api-openapi.yml
  format: yaml
  label: BuyRecord Products API
  slug: buyrecord-app-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-products-api-openapi.yml
- filename: buyrecord-app-stays-api-openapi.yml
  format: yaml
  label: BuyRecord Stays API
  slug: buyrecord-app-stays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-stays-api-openapi.yml
consequence_counts:
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Buyrecord App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'BuyRecord exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BuyRecord
provider_slug: buyrecord-app
slug: buyrecord-app-agentic-access
source_filename: buyrecord-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/buyrecord-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/products/search\n  method: get\n  operationId: search_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/compare\n  method: get\n  operationId: compare_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_id}/outcomes\n\
  \  method: get\n  operationId: get_product_outcomes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchants/{shop_domain}\n  method: get\n  operationId: get_merchant_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/outcomes\n  method: post\n  operationId: submit_outcome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/stays/search\n  method: get\n  operationId: search_stays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/stays/{property_id}\n  method: get\n  operationId: get_stay_outcomes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stays/outcomes\n  method: post\n  operationId: submit_stay_outcome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys\n  method: post\n  operationId: create_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/buyrecord-app/agentic-access/buyrecord-app-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Artificial Intelligence
- E-Commerce
- Data
- Shopping
- Analytics
---
