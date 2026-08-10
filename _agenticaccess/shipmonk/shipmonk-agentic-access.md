---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 10
api_specs:
- filename: shipmonk-webhooks-asyncapi.yml
  format: yaml
  label: ShipMonk Webhooks
  slug: shipmonk-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/asyncapi/shipmonk-webhooks-asyncapi.yml
- filename: shipmonk-orders-api-openapi.yml
  format: yaml
  label: ShipMonk Orders API
  slug: shipmonk-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-orders-api-openapi.yml
- filename: shipmonk-products-api-openapi.yml
  format: yaml
  label: ShipMonk Products API
  slug: shipmonk-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-products-api-openapi.yml
- filename: shipmonk-receivings-api-openapi.yml
  format: yaml
  label: ShipMonk Receivings API
  slug: shipmonk-receivings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-receivings-api-openapi.yml
- filename: shipmonk-returns-api-openapi.yml
  format: yaml
  label: ShipMonk Returns API
  slug: shipmonk-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-returns-api-openapi.yml
- filename: shipmonk-warehouses-api-openapi.yml
  format: yaml
  label: ShipMonk Warehouses API
  slug: shipmonk-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-warehouses-api-openapi.yml
consequence_counts:
  physical: 3
  read: 10
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shipmonk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/integrations/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/integrations/sandbox/complete-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/integrations/submit-order
operation_count: 19
overview: 'ShipMonk exposes 19 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 6 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ShipMonk
provider_slug: shipmonk
slug: shipmonk-agentic-access
source_filename: shipmonk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/shipmonk-orders-openapi.yml, openapi/shipmonk-products-openapi.yml, openapi/shipmonk-receivings-openapi.yml,\n  openapi/shipmonk-returns-openapi.yml, openapi/shipmonk-warehouses-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 9\n    connected: 10\n  by_consequence:\n    physical: 3\n    read: 10\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/integrations/order\n  method: post\n  operationId: post-v1-integrations-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/orders\n  method: get\n  operationId: get-v1-integrations-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/orders-list\n  method: get\n  operationId: get-v1-integrations-orders-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/sandbox/complete-order\n  method: post\n  operationId: post-v1-integrations-sandbox-complete-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/submit-order\n  method: post\n  operationId: post-v1-integrations-submit-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/product\n  method: post\n  operationId: post-v1-integrations-product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/products/search\n  method: post\n  operationId: post-v1-integrations-products-search\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/products/search/paginate\n  method: get\n  operationId: get-v1-integrations-products-search-paginate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products\n  method: get\n  operationId: get-v1-products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/receiving\n  method: get\n  operationId: get-v1-integrations-receiving\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/receiving\n\
  \  method: post\n  operationId: post-v1-integrations-receiving\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/receipts-list\n  method: get\n  operationId: get-v1-integrations-receipts-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/receivings-list\n  method: get\n  operationId: get-v1-integrations-receivings-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/sandbox/complete-receiving\n  method: post\n  operationId: post-v1-integrations-sandbox-complete-receiving\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/returns\n  method: get\n  operationId: get-v1-integrations-returns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/returns\n  method: post\n  operationId: post-v1-integrations-returns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/returns-list\n  method: get\n  operationId: get-v1-integrations-returns-list\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/sandbox/complete-return\n  method: post\n  operationId: post-v1-integrations-sandbox-complete-return\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/warehouses\n  method: get\n  operationId: get-v1-integrations-warehouses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/agentic-access/shipmonk-agentic-access.yml
summary_line: 19 operations · 9 acting
tags:
- Logistics
- Fulfillment
- 3PL
- Ecommerce
- Warehousing
- Inventory
- Shipping
- Returns
- Supply Chain
- Direct-to-Consumer
- Order Management
---
