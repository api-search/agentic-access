---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 11
api_specs:
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Inventory Items API
  slug: quartzy-inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Order Requests API
  slug: quartzy-order-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Types API
  slug: quartzy-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Labs API
  slug: quartzy-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Webhooks API
  slug: quartzy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Quartzy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /order-requests/{id}
operation_count: 17
overview: 'Quartzy exposes 17 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 4 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Quartzy
provider_slug: quartzy
slug: quartzy-agentic-access
source_filename: quartzy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/quartzy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 11\n    acting: 6\n  by_consequence:\n    read: 11\n    write: 4\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labs\n  method: get\n  operationId:\
  \ listLabs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labs/{id}\n  method: get\n  operationId: getLab\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory-items\n  method: get\n  operationId: listInventoryItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory-items/{id}\n  method: get\n  operationId: getInventoryItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /inventory-items/{id}\n  method: put\n  operationId: updateInventoryItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory-items/{itemId}/instances/{itemInstanceId}\n  method: put\n  operationId: updateInventoryItemInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order-requests\n  method: get\n  operationId: listOrderRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order-requests\n\
  \  method: post\n  operationId: createOrderRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order-requests/{id}\n  method: get\n  operationId: getOrderRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order-requests/{id}\n  method: put\n  operationId: updateOrderRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/agentic-access/quartzy-agentic-access.yml
summary_line: 17 operations · 6 acting
tags:
- Lab Management
- Inventory Management
- Life Sciences
- Procurement
- Ordering
- Laboratory
- Webhooks
---
