---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: channelape-openapi-generated.yml
  format: yaml
  label: ChannelApe API
  slug: channelape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/_ae-authored/channelape-openapi-generated.yml
- filename: channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api-openapi.yml
  format: yaml
  label: ChannelApe 0B2D6F2B 4676 40B4 9588 2A4C93F6B250 API
  slug: channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api-openapi.yml
- filename: channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api-openapi.yml
  format: yaml
  label: ChannelApe 6F7402B4 E75C 4573 B3B4 3139Dc1B733D API
  slug: channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api-openapi.yml
- filename: channelape-channelape-api-api-openapi.yml
  format: yaml
  label: ChannelApe ChannelApe API
  slug: channelape-channelape-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-channelape-api-api-openapi.yml
- filename: channelape-inventory-item-quantity-adjustments-api-openapi.yml
  format: yaml
  label: ChannelApe Inventory Item Quantity Adjustments API
  slug: channelape-inventory-item-quantity-adjustments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-inventory-item-quantity-adjustments-api-openapi.yml
- filename: channelape-rest-api-openapi.yml
  format: yaml
  label: ChannelApe Rest API
  slug: channelape-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-rest-api-openapi.yml
- filename: channelape-suppliers-api-openapi.yml
  format: yaml
  label: ChannelApe Suppliers API
  slug: channelape-suppliers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/channelape/openapi/channelape-suppliers-api-openapi.yml
consequence_counts:
  physical: 3
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Channelape Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0b2d6f2b-4676-40b4-9588-2a4c93f6b250
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /6f7402b4-e75c-4573-b3b4-3139dc1b733d
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/suppliers/{supplierid}/callbacks
operation_count: 8
overview: 'ChannelApe exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 3 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ChannelApe
provider_slug: channelape
slug: channelape-agentic-access
source_filename: channelape-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/channelape-0b2d6f2b-4676-40b4-9588-2a4c93f6b250-api-openapi.yml, openapi/channelape-6f7402b4-e75c-4573-b3b4-3139dc1b733d-api-openapi.yml,\n  openapi/channelape-channelape-api-api-openapi.yml, openapi/channelape-inventory-item-quantity-adjustments-api-openapi.yml,\n  openapi/channelape-rest-api-openapi.yml, openapi/channelape-suppliers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 6\n    connected: 2\n  by_consequence:\n    physical: 3\n    read: 2\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /0b2d6f2b-4676-40b4-9588-2a4c93f6b250\n  method: post\n  operationId: post_0b2d6f2b_4676_40b4_9588_2a4c93f6b250\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /6f7402b4-e75c-4573-b3b4-3139dc1b733d\n  method: post\n  operationId: post_6f7402b4_e75c_4573_b3b4_3139dc1b733d\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{v1id}\n  method: get\n  operationId: get_v1_v1id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inventory_item_quantity_adjustments\n\
  \  method: post\n  operationId: post_v1_inventory_item_quantity_adjustments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/rpc/{rpcid}\n  method: post\n  operationId: post_rest_v1_rpc_rpcid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/{v1id}\n  method: get\n  operationId: get_rest_v1_v1id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/{v1id}\n  method: post\n  operationId: post_rest_v1_v1id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/suppliers/{supplierid}/callbacks\n  method: post\n  operationId: post_v1_suppliers_supplierid_callbacks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/channelape/agentic-access/channelape-agentic-access.yml
summary_line: 8 operations · 6 acting
tags:
- Inventory
- Wholesale
- Retail
---
