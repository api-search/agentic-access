---
acting_count: 4
action_class_counts:
  acting: 4
api_specs:
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Menu / Catalog API
  slug: menu-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Stores API
  slug: stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Stock / Availability API
  slug: stock-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Callbacks API
  slug: callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
consequence_counts:
  physical: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Petpooja Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /save_order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /update_store_status
operation_count: 4
overview: 'Petpooja exposes 4 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 write and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Petpooja
provider_slug: petpooja
slug: petpooja-agentic-access
source_filename: petpooja-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/petpooja-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 4\n  by_consequence:\n    write: 2\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /mapped_restaurant_menus\n  method: post\n  operationId: fetchMappedRestaurantMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /save_order\n  method: post\n  operationId: saveOrder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_store_status\n  method: post\n  operationId: updateStoreStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_item_stock\n  method: post\n  operationId: updateItemStock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/agentic-access/petpooja-agentic-access.yml
summary_line: 4 operations · 4 acting
tags:
- Restaurant
- POS
- Online Ordering
- Menu
- Food Delivery
---
