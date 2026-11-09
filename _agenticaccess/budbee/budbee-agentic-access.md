---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 15
api_specs:
- filename: budbee-box-api-openapi.yml
  format: yaml
  label: Budbee Box API
  slug: budbee-box-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budbee/openapi/budbee-box-api-openapi.yml
- filename: budbee-boxes-api-openapi.yml
  format: yaml
  label: Budbee Boxes API
  slug: budbee-boxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budbee/openapi/budbee-boxes-api-openapi.yml
- filename: budbee-budbee-api-api-openapi.yml
  format: yaml
  label: Budbee Budbee API
  slug: budbee-budbee-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budbee/openapi/budbee-budbee-api-api-openapi.yml
- filename: budbee-intervals-api-openapi.yml
  format: yaml
  label: Budbee Intervals API
  slug: budbee-intervals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budbee/openapi/budbee-intervals-api-openapi.yml
- filename: budbee-multiple-api-openapi.yml
  format: yaml
  label: Budbee Multiple API
  slug: budbee-multiple-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budbee/openapi/budbee-multiple-api-openapi.yml
- filename: budbee-postalcodes-api-openapi.yml
  format: yaml
  label: Budbee Postalcodes API
  slug: budbee-postalcodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budbee/openapi/budbee-postalcodes-api-openapi.yml
- filename: budbee-returns-api-openapi.yml
  format: yaml
  label: Budbee Returns API
  slug: budbee-returns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budbee/openapi/budbee-returns-api-openapi.yml
- filename: budbee-users-api-openapi.yml
  format: yaml
  label: Budbee Users API
  slug: budbee-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budbee/openapi/budbee-users-api-openapi.yml
- filename: budbee-webhooks-api-openapi.yml
  format: yaml
  label: Budbee Webhooks API
  slug: budbee-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budbee/openapi/budbee-webhooks-api-openapi.yml
consequence_counts:
  physical: 5
  read: 15
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Budbee Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /multiple/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /multiple/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /multiple/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /multiple/orders/{id}/parcels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /multiple/orders/{id}/parcels/{parcelid}
operation_count: 23
overview: 'Budbee exposes 23 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 3 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Budbee
provider_slug: budbee
slug: budbee-agentic-access
source_filename: budbee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/budbee-box-api-openapi.yml, openapi/budbee-boxes-api-openapi.yml, openapi/budbee-budbee-api-api-openapi.yml,\n  openapi/budbee-intervals-api-openapi.yml, openapi/budbee-multiple-api-openapi.yml, openapi/budbee-postalcodes-api-openapi.yml,\n  openapi/budbee-returns-api-openapi.yml, openapi/budbee-users-api-openapi.yml, openapi/budbee-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 15\n    acting: 8\n  by_consequence:\n    read: 15\n    write: 3\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /box/return\n  method: get\n  operationId: get_box_return\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /box/return\n  method: post\n  operationId: post_box_return\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boxes/BOX0001\n  method: get\n  operationId: get_boxes_BOX0001\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boxes/all/SE\n  method: get\n  operationId: get_boxes_all_SE\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boxes/postalcodes/validate/SE/{seid}\n  method: get\n  operationId: get_boxes_postalcodes_validate_SE_seid\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intervals/{countrycode}/{postalcode}/{fromdate}/{todate}\n  method: get\n  operationId: get_intervals_countrycode_postalcode_fromdate_todate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /multiple/orders\n  method: get\n  operationId: get_multiple_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /multiple/orders\n  method: post\n  operationId: post_multiple_orders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multiple/orders/e140396d-5679-4211-96f8-c6c877b43186/parcels\n  method: get\n  operationId: get_multiple_orders_e140396d_5679_4211_96f8_c6c877b43186_parcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /multiple/orders/e140396d-5679-4211-96f8-c6c877b43186/parcels/{parcelId}\n  method: get\n  operationId: get_multiple_orders_e140396d_5679_4211_96f8_c6c877b43186_parcels_parcelId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /multiple/orders/{id}\n  method: delete\n  operationId: delete_multiple_orders_id\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multiple/orders/{id}\n  method: get\n  operationId: get_multiple_orders_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /multiple/orders/{id}\n  method: put\n  operationId: put_multiple_orders_id\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multiple/orders/{id}/parcels\n\
  \  method: post\n  operationId: post_multiple_orders_id_parcels\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multiple/orders/{id}/parcels/{parcelid}\n  method: delete\n  operationId: delete_multiple_orders_id_parcels_parcelid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multiple/orders/{id}/tracking-url\n  method: get\n  operationId: get_multiple_orders_id_tracking_url\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postalcodes/validate/{countrycode}/{postalcode}\n  method: get\n  operationId: get_postalcodes_validate_countrycode_postalcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postalcodes/{countrycode}\n  method: get\n  operationId: get_postalcodes_countrycode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /returns\n  method: get\n  operationId: get_returns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /returns\n  method: post\n  operationId: post_returns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/collection-points\n  method: get\n  operationId: get_users_collection_points\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhookid}\n  method: post\n  operationId: post_webhooks_webhookid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/budbee/agentic-access/budbee-agentic-access.yml
summary_line: 23 operations · 8 acting
tags:
- Company
- Delivery
- Logistics
- E-Commerce
- Sustainability
---
