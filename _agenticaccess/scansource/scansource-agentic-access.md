---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 11
api_specs:
- filename: scansource-product-openapi.yml
  format: yaml
  label: ScanSource Product API
  slug: scansource-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-product-openapi.yml
- filename: scansource-sales-order-openapi.yml
  format: yaml
  label: ScanSource Sales Order API
  slug: scansource-sales-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-sales-order-openapi.yml
- filename: scansource-invoice-openapi.yml
  format: yaml
  label: ScanSource Invoice API
  slug: scansource-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-invoice-openapi.yml
consequence_counts:
  physical: 5
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scansource Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /salesorder/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /salesorder/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /salesorder/createAsync
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /salesorder/shipquote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /salesorder/vrd
operation_count: 18
overview: 'ScanSource exposes 18 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 2 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ScanSource
provider_slug: scansource
slug: scansource-agentic-access
source_filename: scansource-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/scansource-invoice-openapi.yml, openapi/scansource-product-openapi.yml, openapi/scansource-sales-order-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 11\n    acting: 7\n  by_consequence:\n    read: 11\n    write: 2\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /invoice/summary/{customerNumber}\n  method: get\n  operationId: getInvoiceSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice/list/{customerNumber}\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice/detail/{customerNumber}/{invoiceNumber}\n  method: get\n  operationId: getInvoiceDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice/pdf/{customerNumber}/{invoiceNumber}\n  method: get\n  operationId: getInvoicePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/search\n  method: get\n  operationId: searchProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/detail\n  method: get\n  operationId: getProductDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /product/pricing\n  method: post\n  operationId: getProductPricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/availability\n  method: post\n  operationId: getProductAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesorder/create\n  method: post\n  operationId: createSalesOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesorder/createAsync\n  method: post\n  operationId: createSalesOrderAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesorder/vrd\n  method: post\n  operationId: createVrdOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesorder/summary/{customerNumber}\n\
  \  method: get\n  operationId: getSalesOrderSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesorder/list/{customerNumber}\n  method: get\n  operationId: listSalesOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesorder/detail/{customerNumber}/{salesOrderNumber}\n  method: get\n  operationId: getSalesOrderDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesorder/shipquote\n  method: post\n  operationId: getShippingQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesorder/cancel\n  method: delete\n  operationId: cancelSalesOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesorder/tracking\n  method: get\n  operationId: getOrderTracking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesorder/serials\n  method: get\n  operationId: getSerialNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/agentic-access/scansource-agentic-access.yml
summary_line: 18 operations · 7 acting
tags:
- ScanSource
- Distribution
- Barcode
- Point Of Sale
- AIDC
- Inventory
- Order Management
- E-Commerce
- Fortune 1000
---
