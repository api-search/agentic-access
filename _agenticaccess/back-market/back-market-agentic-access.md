---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 25
api_specs:
- filename: back-market-openapi-original.yml
  format: yaml
  label: Back Market API
  slug: back-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/back-market/refs/heads/main/openapi/back-market-openapi-original.yml
consequence_counts:
  physical: 9
  read: 25
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Back Market Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/buyback/v1/orders/{buybackOrderId}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ws/buyback/v1/orders/{buybackOrderId}/suspend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ws/buyback/v1/orders/{buybackOrderId}/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ws/buyback/v2/orders/{buybackOrderId}/counter-offers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /ws/orderlines/{orderline_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/orders/{order_id}/invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/sav/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/sav/{careFolderId}/item-transfer
operation_count: 39
overview: 'Back Market exposes 39 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 5 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Back Market
provider_slug: back-market
slug: back-market-agentic-access
source_filename: back-market-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/back-market-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 25\n    acting: 14\n  by_consequence:\n    read: 25\n    write: 5\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /ws/category/tree\n  method: get\n  operationId: get-bm-catalog-category\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/category/tree/{categoryId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/listings\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/listings\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/listings/{listingId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/listings/{listingId}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /ws/listings/detail\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/tasks/{taskId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/buyback/v1/orders\n  method: get\n  operationId: get-ws-buyback-v1-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/buyback/v1/orders/pending-reply\n  method: get\n  operationId: get-ws-buyback-v1-orders-pending-reply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/buyback/v1/orders/suspend-reasons\n  method: get\n  operationId: get-ws-buyback-v1-orders-suspend-reasons\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/buyback/v1/orders/{buybackOrderId}\n  method: get\n  operationId: get-ws-buyback-v1-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/buyback/v1/orders/{buybackOrderId}/messages\n  method: get\n  operationId: get-ws-buyback-v1-orders-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/buyback/v1/orders/{buybackOrderId}/messages\n  method: post\n  operationId: post-ws-buyback-v1-orders-messages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/buyback/v1/orders/{buybackOrderId}/suspend\n  method: put\n  operationId: put-ws-buyback-v1-orders-suspend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/buyback/v1/orders/{buybackOrderId}/validate\n  method: put\n  operationId: put-ws-buyback-v1-orders-validate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /ws/buyback/v1/orders/{buybackOrderId}/counter-offers/reasons\n  method: get\n  operationId: get-ws-counter-offer-reason\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/buyback/v2/orders/{buybackOrderId}/counter-offers\n  method: put\n  operationId: put-ws-refurbisher-counter-offer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/buyback/v1/listings\n  method: get\n  operationId: get-ws-buyback-v1-listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/buyback/v1/listings/{buybackListingId}\n\
  \  method: get\n  operationId: get-ws-buyback-v1-listing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/buyback/v1/listings/{buybackListingId}\n  method: put\n  operationId: put-ws-buyback-v1-listing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/buyback/v1/competitors/{listingId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/orders\n  method: get\n  operationId: get-ws-list-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /ws/orders/{order_id}\n  method: get\n  operationId: get-ws-specific-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/orders/{order_id}\n  method: post\n  operationId: update-ws-specific-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/orders/{order_id}/invoice\n  method: post\n  operationId: post-ws-specific-order-invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/orderlines/{orderline_id}\n  method: patch\n  operationId: update-ws-specific-orderline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/shipping/v1/deliveries\n  method: get\n  operationId: GetDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/shipping/v1/returns\n  method: get\n  operationId: GetReturns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/shipping/v1/deliveries/{id}\n\
  \  method: get\n  operationId: GetDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/shipping/v1/returns/{id}\n  method: get\n  operationId: GetReturn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/sav\n  method: get\n  operationId: getCareFolderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/sav/{careFolderId}\n  method: get\n  operationId: getCareFolderDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/sav/{careFolderId}/problem\n  method: post\n  operationId: postProblem\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/sav/refund\n  method: post\n  operationId: postRefundCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/sav/{careFolderId}/msg\n  method: post\n  operationId: postMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/sav/{careFolderId}/item-transfer\n\
  \  method: post\n  operationId: postItemTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/listings_bi\n  method: get\n  operationId: GetBackboxData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/backbox/v1/competitors/{listingId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/back-market/refs/heads/main/agentic-access/back-market-agentic-access.yml
summary_line: 39 operations · 14 acting
tags:
- Company
- E-Commerce
- Marketplace
- Retail
- Refurbished Electronics
- Circular Economy
- Orders
- Listings
- Product Catalog
- Logistics
- Customer Support
---
