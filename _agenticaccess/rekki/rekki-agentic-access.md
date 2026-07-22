---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 5
api_specs:
- filename: rekki-supplier-api-openapi-original.json
  format: json
  label: REKKI Supplier API
  slug: rekki-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/openapi/rekki-supplier-api-openapi-original.json
consequence_counts:
  physical: 12
  read: 5
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rekki Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v1/orders/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v1/orders/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v1/orders/list_not_integrated
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v1/orders/set_error
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v1/orders/set_integrated
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v3/order-guide
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v3/orders/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v3/orders/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v3/orders/set_error
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v3/orders/set_integrated
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v4/orders/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /integration/v4/orders/set_integrated
operation_count: 32
overview: 'REKKI exposes 32 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 15 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: REKKI
provider_slug: rekki
slug: rekki-agentic-access
source_filename: rekki-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/rekki-supplier-api-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 5\n    acting: 27\n  by_consequence:\n    read: 5\n    write: 15\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /integration/v1/catalog/items\n  method: get\n  operationId: GetCatalogItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/v1/catalog/items\n  method: post\n  operationId: UpdateCatalogItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v1/catalog/items/{id}\n  method: get\n  operationId: GetCatalogItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/v1/catalog/items/{id}\n  method: delete\n  operationId: DeleteCatalogItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v1/catalog/replace\n  method: post\n  operationId: ReplaceCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v1/log\n  method: post\n  operationId: PostLogMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v1/orders/confirm\n  method: post\n  operationId: ConfirmOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v1/orders/list\n  method: post\n  operationId: ListOrdersBySupplier\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v1/orders/list_not_integrated\n  method: post\n  operationId: ListNotIntegratedOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v1/orders/set_error\n  method: post\n  operationId: MarkIntegrationError\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v1/orders/set_integrated\n  method: post\n  operationId: MarkOrdersIntegrated\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v2/catalog/items/availability\n  method: post\n  operationId: UpdateCatalogItemAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /integration/v3/catalog/inventory\n  method: post\n  operationId: UpdateCatalogInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/catalog/items\n  method: get\n  operationId: GetCatalogItemsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/v3/catalog/items\n  method: post\n  operationId: UpdateCatalogItemsV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /integration/v3/catalog/items/availability\n  method: post\n  operationId: UpdateCatalogItemAvailabilityV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/catalog/items/delete\n  method: post\n  operationId: DeleteCatalogItemsV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/catalog/items/photo\n  method: post\n  operationId: UploadCatalogPhoto\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/catalog/items/{id}\n  method: get\n  operationId: GetCatalogItemV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/v3/catalog/pricelist\n  method: post\n  operationId: UpdatePriceList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/catalog/replace\n  method: post\n  operationId: ReplaceCatalogV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/customers-and-product-list/connect\n  method: post\n  operationId: CreateConnectCustomersAndProductListV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/customers/connect\n  method: post\n  operationId: CreateConnectCustomersV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/log\n  method: post\n  operationId: PostLogMessageV3\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/order-guide\n  method: get\n  operationId: GetOrderGuideV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/v3/order-guide\n  method: post\n  operationId: ReplaceOrderGuideV3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/orders/confirm\n  method: post\n  operationId: ConfirmOrdersV3\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/orders/list\n  method: post\n  operationId: ListOrdersBySupplierV3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/orders/set_error\n  method: post\n  operationId: MarkIntegrationErrorV3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v3/orders/set_integrated\n  method: post\n  operationId: MarkOrdersIntegratedV3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/v4/orders/set_integrated\n  method: post\n  operationId: MarkOrdersIntegratedV4\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /integration/v4/orders/list\n  method: post\n  operationId: ListOrdersBySupplierV4\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/agentic-access/rekki-agentic-access.yml
summary_line: 32 operations · 27 acting
tags:
- Company
- Food
- Wholesale
- Ordering
- Restaurants
- Supply Chain
- Catalog
- Orders
- eCommerce
---
