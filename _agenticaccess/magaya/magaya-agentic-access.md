---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Shipments API
  slug: magaya-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Warehouse Receipts API
  slug: magaya-warehouse-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Invoices API
  slug: magaya-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Items API
  slug: magaya-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Transactions API
  slug: magaya-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
consequence_counts:
  physical: 2
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Magaya Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments
operation_count: 14
overview: 'Magaya exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Magaya
provider_slug: magaya
slug: magaya-agentic-access
source_filename: magaya-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/magaya-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 10\n    acting: 4\n  by_consequence:\n    read: 10\n    physical: 2\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /shipments\n  method: get\n  operationId: listShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments\n  method: post\n  operationId: createShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments/{guid}\n  method: get\n  operationId: getShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /warehouse-receipts\n  method: get\n  operationId: listWarehouseReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /warehouse-receipts\n  method: post\n  operationId: createWarehouseReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /warehouse-receipts/{guid}\n  method: get\n  operationId:\
  \ getWarehouseReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{guid}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /items\n\
  \  method: get\n  operationId: listItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /items\n  method: post\n  operationId: createItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/{guid}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{guid}\n  method: get\n  operationId:\
  \ getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/agentic-access/magaya-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Logistics
- Supply Chain
- Freight Forwarding
- Warehouse Management
- Shipping
- Customs
- Transportation
---
