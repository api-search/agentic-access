---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 19
consequence_counts:
  physical: 1
  read: 19
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sap Bydesign Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sap/byd/odata/cust/v1/khcustomerinvoice/Release
operation_count: 26
overview: 'SAP Business ByDesign exposes 26 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SAP Business ByDesign
provider_slug: sap-bydesign
slug: sap-bydesign-agentic-access
source_filename: sap-bydesign-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sap-bydesign-odata-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 19\n    acting: 7\n  by_consequence:\n    read: 19\n    write: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /sap/byd/odata/cust/v1/{service}/\n  method: get\n  operationId: getEntitySets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/{service}/$metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/vmumaterial/MaterialCollection\n  method: get\n  operationId: queryMaterials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/vmumaterial/MaterialCollection\n  method: post\n  operationId: createMaterial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sap/byd/odata/cust/v1/khsalesorder/SalesOrderCollection\n  method: get\n  operationId: querySalesOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khsalesorder/SalesOrderCollection('{ObjectID}')\n\
  \  method: get\n  operationId: getSalesOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khcustomerquote/CustomerQuoteCollection\n  method: get\n  operationId: queryCustomerQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khcustomerquote/CustomerQuoteCollection\n  method: post\n  operationId: createCustomerQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sap/byd/odata/cust/v1/khcustomerinvoice/CustomerInvoiceQueryByElements2\n  method: get\n  operationId: queryCustomerInvoices\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khcustomerinvoice/Release\n  method: post\n  operationId: releaseCustomerInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sap/byd/odata/cust/v1/khpurchaseorder/PurchaseOrderCollection\n  method: get\n  operationId: queryPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khsupplierinvoice/SupplierInvoiceCollection\n  method: get\n  operationId: querySupplierInvoices\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khoutbounddelivery/OutboundDeliveryCollection\n  method: get\n  operationId: queryOutboundDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khoutbounddelivery/Release\n  method: post\n  operationId: releaseOutboundDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sap/byd/odata/cust/v1/khoutbounddeliveryrequest/ItemPostGoodsIssue\n  method: post\n  operationId: postGoodsIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sap/byd/odata/cust/v1/khinbounddelivery/InboundDeliveryCollection\n  method: get\n  operationId: queryInboundDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khinbounddelivery/InboundDeliveryCollection\n  method: post\n  operationId: createInboundDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sap/byd/odata/cust/v1/khinbounddelivery/PostGoodsReceipt\n  method: post\n  operationId: postGoodsReceipt\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sap/byd/odata/cust/v1/khproject/ProjectCollection\n  method: get\n  operationId: queryProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khlead/LeadCollection\n  method: get\n  operationId: queryLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khopportunity/OpportunityCollection\n  method: get\n  operationId: queryOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /sap/byd/odata/cust/v1/khpayment/PaymentCollection\n  method: get\n  operationId: queryPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/cust/v1/khhousebankaccount/HouseBankAccountQueryByElements\n  method: get\n  operationId: queryHouseBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/ana_businessanalytics_analytics.svc/$metadata\n  method: get\n  operationId: getAnalyticsMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/ana_businessanalytics_analytics.svc/{ReportEntitySet}\n  method: get\n  operationId: queryAnalyticsReport\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sap/byd/odata/\n  method: get\n  operationId: listODataServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/agentic-access/sap-bydesign-agentic-access.yml
summary_line: 26 operations · 7 acting
tags:
- ERP
- Cloud
- Midmarket
- Financials
- CRM
- Procurement
- Supply Chain
- Project Management
- OData
- SOAP
- SAP
---
