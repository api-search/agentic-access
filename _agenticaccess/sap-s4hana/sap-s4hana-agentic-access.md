---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 9
api_specs:
- filename: sap-s4hana-partners-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Partners API
  slug: sap-s4hana-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-partners-api-openapi.yml
- filename: sap-s4hana-pricing-elements-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Pricing Elements API
  slug: sap-s4hana-pricing-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-pricing-elements-api-openapi.yml
- filename: sap-s4hana-sales-order-items-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Sales Order Items API
  slug: sap-s4hana-sales-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-sales-order-items-api-openapi.yml
- filename: sap-s4hana-sales-orders-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Sales Orders API
  slug: sap-s4hana-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-sales-orders-api-openapi.yml
- filename: sap-s4hana-schedule-lines-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Schedule Lines API
  slug: sap-s4hana-schedule-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-schedule-lines-api-openapi.yml
- filename: sap-s4hana-text-api-openapi.yml
  format: yaml
  label: SAP S/4HANA Text API
  slug: sap-s4hana-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/openapi/sap-s4hana-text-api-openapi.yml
consequence_counts:
  physical: 6
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sap S4Hana Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /A_SalesOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /A_SalesOrder('{SalesOrder}')
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /A_SalesOrder('{SalesOrder}')
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /A_SalesOrder('{SalesOrder}')/to_Item
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /A_SalesOrderItem(SalesOrder='{SalesOrder}',SalesOrderItem='{SalesOrderItem}')
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /A_SalesOrderItem(SalesOrder='{SalesOrder}',SalesOrderItem='{SalesOrderItem}')
operation_count: 15
overview: 'SAP S/4HANA exposes 15 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
slug: sap-s4hana-agentic-access
source_filename: sap-s4hana-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sap-s4hana-sales-order-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 9\n    acting: 6\n  by_consequence:\n    read: 9\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /A_SalesOrder\n  method: get\n  operationId: listSalesOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /A_SalesOrder\n  method: post\n  operationId: createSalesOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /A_SalesOrder('{SalesOrder}')\n  method: get\n  operationId: getSalesOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /A_SalesOrder('{SalesOrder}')\n  method: patch\n  operationId: updateSalesOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /A_SalesOrder('{SalesOrder}')\n  method: delete\n  operationId: deleteSalesOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /A_SalesOrder('{SalesOrder}')/to_Item\n  method: get\n  operationId: listSalesOrderItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /A_SalesOrder('{SalesOrder}')/to_Item\n  method: post\n  operationId: createSalesOrderItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /A_SalesOrderItem(SalesOrder='{SalesOrder}',SalesOrderItem='{SalesOrderItem}')\n\
  \  method: get\n  operationId: getSalesOrderItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /A_SalesOrderItem(SalesOrder='{SalesOrder}',SalesOrderItem='{SalesOrderItem}')\n  method: patch\n  operationId: updateSalesOrderItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /A_SalesOrderItem(SalesOrder='{SalesOrder}',SalesOrderItem='{SalesOrderItem}')\n  method: delete\n  operationId: deleteSalesOrderItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /A_SalesOrder('{SalesOrder}')/to_Partner\n  method: get\n  operationId: listSalesOrderPartners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /A_SalesOrder('{SalesOrder}')/to_PricingElement\n  method: get\n  operationId: listSalesOrderPricingElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /A_SalesOrderItem(SalesOrder='{SalesOrder}',SalesOrderItem='{SalesOrderItem}')/to_ScheduleLine\n  method: get\n  operationId: listSalesOrderItemScheduleLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /A_SalesOrderItem(SalesOrder='{SalesOrder}',SalesOrderItem='{SalesOrderItem}')/to_PricingElement\n\
  \  method: get\n  operationId: listSalesOrderItemPricingElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /A_SalesOrder('{SalesOrder}')/to_Text\n  method: get\n  operationId: listSalesOrderTexts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/agentic-access/sap-s4hana-agentic-access.yml
summary_line: 15 operations · 6 acting
tags:
- Business Applications
- Cloud
- Enterprise Resource Planning
- ERP
- Finance
- Human Resources
- Inventory
- Logistics
- Manufacturing
- Plant Maintenance
- Procurement
- S/4HANA
- Sales
- SAP
---
