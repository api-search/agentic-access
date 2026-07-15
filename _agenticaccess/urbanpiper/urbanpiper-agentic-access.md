---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 2
api_specs:
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Catalog & Menu API
  slug: catalog-menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Stores & Locations API
  slug: stores-locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Item Availability API
  slug: item-availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
- filename: urbanpiper-openapi.yml
  format: yaml
  label: UrbanPiper Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-openapi.yml
consequence_counts:
  physical: 5
  read: 2
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Urbanpiper Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ext/api/v1/generic/pos/rider-location/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ext/api/v1/generic/pos/rider-status/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /external/api/v1/orders/{id}/status/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /external/api/v1/webhooks/retry/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hub/api/v1/orders/items-oos/
operation_count: 16
overview: 'UrbanPiper exposes 16 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 9 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: UrbanPiper
provider_slug: urbanpiper
slug: urbanpiper-agentic-access
source_filename: urbanpiper-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/urbanpiper-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 14\n    connected: 2\n  by_consequence:\n    write: 9\n    physical: 5\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /external/api/v1/stores/\n  method: post\n  operationId: createUpdateStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/api/v1/location/\n  method: post\n  operationId: createUpdateLocationHub\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v1/inventory/locations/{location_ref_id}/\n  method: post\n  operationId: addUpdateMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/api/v1/items/\n  method: post\n  operationId: addUpdateItemsHub\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /external/api/v1/inventory/categories/timing-groups/\n  method: post\n  operationId: createCategoryTimingGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v1/orders/{id}/status/\n  method: put\n  operationId: updateOrderStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/api/v1/orders/items-oos/\n  method: post\n  operationId: markOrderItemsOutOfStock\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v1/aggregator/zomato/feature-action/\n  method: post\n  operationId: zomatoFeatureAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v1/aggregator/swiggy/feature-action/\n  method: post\n  operationId: swiggyFeatureAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /external/api/v1/webhooks/\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v1/webhooks/\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v1/webhooks/{webhook_id}/\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/api/v1/webhooks/{webhook_id}/\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/api/v1/webhooks/retry/\n  method: post\n  operationId: retryWebhookOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ext/api/v1/generic/pos/rider-status/\n  method: post\n  operationId: riderStatusUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /ext/api/v1/generic/pos/rider-location/\n  method: post\n  operationId: riderLiveTracking\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/agentic-access/urbanpiper-agentic-access.yml
summary_line: 16 operations · 14 acting
tags:
- Restaurants
- Food Delivery
- Ordering
- POS
- Aggregators
- Commerce
---
