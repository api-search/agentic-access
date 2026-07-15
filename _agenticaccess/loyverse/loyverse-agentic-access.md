---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 22
api_specs:
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Items API
  slug: loyverse-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Categories API
  slug: loyverse-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Receipts API
  slug: loyverse-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Customers API
  slug: loyverse-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Inventory API
  slug: loyverse-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Stores API
  slug: loyverse-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
- filename: loyverse-openapi.yml
  format: yaml
  label: Loyverse Employees API
  slug: loyverse-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/openapi/loyverse-openapi.yml
consequence_counts:
  read: 22
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Loyverse Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Loyverse exposes 32 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Loyverse
provider_slug: loyverse
slug: loyverse-agentic-access
source_filename: loyverse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/loyverse-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 22\n    acting: 10\n  by_consequence:\n    read: 22\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /items\n  method: get\n  operationId: listItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /items\n  method: post\n  operationId: createOrUpdateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /items/{item_id}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /items/{item_id}\n  method: delete\n  operationId: deleteItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n\
  \    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /categories\n  method: post\n  operationId: createOrUpdateCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /categories/{category_id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /categories/{category_id}\n  method: delete\n  operationId: deleteCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /receipts\n  method: get\n  operationId: listReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n\
  - path: /receipts\n  method: post\n  operationId: createReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /receipts/{receipt_number}\n  method: get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /customers\n  method: post\n  operationId: createOrUpdateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /customers/{customer_id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /customers/{customer_id}\n  method: delete\n  operationId: deleteCustomer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /inventory\n  method: get\n  operationId: getInventoryLevels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /inventory\n  method: post\n  operationId: updateInventoryLevels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /stores\n  method: get\n  operationId: listStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /stores/{store_id}\n  method: get\n  operationId: getStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /employees\n  method: post\n  operationId: createOrUpdateEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /employees/{employee_id}\n  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /employees/{employee_id}\n\
  \  method: delete\n  operationId: deleteEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /payment_types\n  method: get\n  operationId: listPaymentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /payment_types/{payment_type_id}\n  method: get\n  operationId: getPaymentType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /merchants\n  method: get\n  operationId: listMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /taxes\n  method: get\n  operationId: listTaxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /discounts\n  method: get\n  operationId: listDiscounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n\
  \    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /modifiers\n  method: get\n  operationId: listModifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /suppliers\n  method: get\n  operationId: listSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /pos_devices\n  method: get\n  operationId: listPosDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n\
  \    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n- path: /shifts\n  method: get\n  operationId: listShifts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - CUSTOMERS_READ\n    - INVENTORY_READ\n    - ITEMS_READ\n    - RECEIPTS_READ\n    - STORES_READ\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loyverse/refs/heads/main/agentic-access/loyverse-agentic-access.yml
summary_line: 32 operations · 10 acting
tags:
- Point of Sale
- POS
- Retail
- Inventory
- Cafe and Restaurant
- Loyalty
- Payments
- Commerce
---
