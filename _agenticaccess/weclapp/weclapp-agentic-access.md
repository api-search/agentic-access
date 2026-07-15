---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 21
api_specs:
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Customer API
  slug: weclapp-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Article API
  slug: weclapp-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Sales Order API
  slug: weclapp-sales-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Quotation API
  slug: weclapp-quotation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Sales Invoice API
  slug: weclapp-sales-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Shipment API
  slug: weclapp-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
- filename: weclapp-openapi.yml
  format: yaml
  label: weclapp Purchase Order API
  slug: weclapp-purchase-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/openapi/weclapp-openapi.yml
consequence_counts:
  physical: 12
  read: 21
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Weclapp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchaseOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /purchaseOrder/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /purchaseOrder/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /salesInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /salesInvoice/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /salesInvoice/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /salesOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /salesOrder/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /salesOrder/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /shipment/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /shipment/id/{id}
operation_count: 42
overview: 'weclapp exposes 42 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 9 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: weclapp
provider_slug: weclapp
slug: weclapp-agentic-access
source_filename: weclapp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/weclapp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 21\n    acting: 21\n  by_consequence:\n    read: 21\n    write: 9\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /customer\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/count\n  method: get\n  operationId: countCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/id/{id}\n  method: get\n  operationId: getCustomerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/id/{id}\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/id/{id}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /article\n  method: get\n  operationId: getArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /article\n  method: post\n  operationId: createArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /article/count\n  method: get\n  operationId: countArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /article/id/{id}\n  method: get\n  operationId: getArticleById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /article/id/{id}\n  method: put\n  operationId: updateArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /article/id/{id}\n  method: delete\n  operationId: deleteArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesOrder\n  method: get\n  operationId: getSalesOrders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesOrder\n  method: post\n  operationId: createSalesOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesOrder/count\n  method: get\n  operationId: countSalesOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesOrder/id/{id}\n  method: get\n  operationId: getSalesOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesOrder/id/{id}\n\
  \  method: put\n  operationId: updateSalesOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesOrder/id/{id}\n  method: delete\n  operationId: deleteSalesOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotation\n  method: get\n  operationId: getQuotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /quotation\n  method: post\n  operationId: createQuotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotation/count\n  method: get\n  operationId: countQuotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotation/id/{id}\n  method: get\n  operationId: getQuotationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotation/id/{id}\n  method: put\n  operationId: updateQuotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotation/id/{id}\n  method: delete\n  operationId: deleteQuotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesInvoice\n  method: get\n  operationId: getSalesInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesInvoice\n  method: post\n  operationId: createSalesInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesInvoice/count\n  method: get\n  operationId: countSalesInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesInvoice/id/{id}\n  method: get\n  operationId: getSalesInvoiceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesInvoice/id/{id}\n  method: put\n  operationId: updateSalesInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /salesInvoice/id/{id}\n\
  \  method: delete\n  operationId: deleteSalesInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipment\n  method: get\n  operationId: getShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment\n  method: post\n  operationId: createShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /shipment/count\n  method: get\n  operationId: countShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment/id/{id}\n  method: get\n  operationId: getShipmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment/id/{id}\n  method: put\n  operationId: updateShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipment/id/{id}\n  method: delete\n  operationId: deleteShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchaseOrder\n  method: get\n  operationId: getPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchaseOrder\n  method: post\n  operationId: createPurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchaseOrder/count\n  method: get\n  operationId: countPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchaseOrder/id/{id}\n  method: get\n  operationId: getPurchaseOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchaseOrder/id/{id}\n  method: put\n  operationId: updatePurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchaseOrder/id/{id}\n  method: delete\n  operationId: deletePurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weclapp/refs/heads/main/agentic-access/weclapp-agentic-access.yml
summary_line: 42 operations · 21 acting
tags:
- ERP
- CRM
- Cloud ERP
- Accounting
- Inventory
- Commerce
- Germany
- Order Management
- Business Software
- SaaS
---
