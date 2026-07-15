---
acting_count: 24
action_class_counts:
  acting: 24
api_specs:
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Inventory & Items API
  slug: inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Vendors API
  slug: vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Purchase Orders API
  slug: purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Invoices & Docs API
  slug: invoices-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Deliveries API
  slug: deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Recipes & Menu Profitability API
  slug: recipes-menu-profitability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
consequence_counts:
  physical: 8
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Marketman Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /buyers/docs/GetDocsByDocDate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /buyers/orders/CreateOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /buyers/orders/GetCatalogItems
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /buyers/orders/GetOrdersByDeliveryDate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /buyers/orders/GetOrdersBySentDate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /buyers/webhooks/GetWebhookEventByOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vendors/docs/SetDocs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vendors/docs/ValidateDoc
operation_count: 24
overview: 'MarketMan exposes 24 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 write and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MarketMan
provider_slug: marketman
slug: marketman-agentic-access
source_filename: marketman-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/marketman-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 24\n  by_consequence:\n    write: 16\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /buyers/auth/GetToken\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/auth/GetTokenDetails\n  method: post\n  operationId: getTokenDetails\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/partneraccounts/GetAuthorisedAccounts\n  method: post\n  operationId: getAuthorisedAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/inventory/GetItems\n  method: post\n  operationId: getItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/inventory/GetInventoryItems\n\
  \  method: post\n  operationId: getInventoryItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/inventory/SetInventoryCount\n  method: post\n  operationId: setInventoryCount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/inventory/GetUOMTypes\n  method: post\n  operationId: getUOMTypes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/items/GetVendors\n  method: post\n  operationId: getVendors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/inventory/GetMenuItems\n  method: post\n  operationId: getMenuItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/inventory/GetMenuItemsAvailability\n  method: post\n  operationId: getMenuItemsAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/inventory/GetMenuProfitability\n  method: post\n  operationId: getMenuProfitability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/orders/GetOrdersByDeliveryDate\n  method: post\n  operationId: getOrdersByDeliveryDate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/orders/GetOrdersBySentDate\n\
  \  method: post\n  operationId: getOrdersBySentDate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/orders/GetCatalogItems\n  method: post\n  operationId: getCatalogItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/orders/CreateOrder\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/docs/GetDocsByDocDate\n  method: post\n  operationId: getDocsByDocDate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/docs/SetDocsExported\n  method: post\n  operationId: setDocsExported\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /vendors/docs/GetDeliveryNotesByDate\n  method: post\n  operationId: getDeliveryNotesByDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendors/docs/ValidateDoc\n  method: post\n  operationId: validateDoc\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendors/docs/SetDocs\n  method: post\n  operationId: setDocs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/webhooks/CreateWebhook\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/webhooks/GetWebhooks\n  method: post\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/webhooks/GetWebhookEventByOrder\n  method: post\n  operationId: getWebhookEventByOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyers/webhooks/DeleteWebhook\n  method: post\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/agentic-access/marketman-agentic-access.yml
summary_line: 24 operations · 24 acting
tags:
- Restaurant
- Inventory
- Purchasing
- Supply Chain
- Food Service
---
