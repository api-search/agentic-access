---
acting_count: 131
action_class_counts:
  acting: 131
  connected: 124
api_specs:
- filename: accruent-maintenance-connection-openapi.yml
  format: yaml
  label: Maintenance Connection Web API
  slug: maintenance-connection-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accruent/refs/heads/main/openapi/accruent-maintenance-connection-openapi.yml
consequence_counts:
  physical: 66
  read: 124
  write: 65
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Accruent Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Invoices/{invoicePK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /PurchaseOrderLineItems
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PurchaseOrderLineItems
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /PurchaseOrderLineItems/{lineItemPK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PurchaseOrderNote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PurchaseOrders/{purchaseOrderPK}/Invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /PurchaseOrders/{purchaseOrderPK}/Invoices/{invoicePK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PurchaseOrders/{purchaseOrderPK}/LineItems
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /PurchaseOrders/{purchaseOrderPK}/LineItems/{lineItemPK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PurchaseOrders/{purchaseOrderPK}/Receipts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /PurchaseOrders/{purchaseOrderPK}/Receipts/{receiptPK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /PurchaseOrders/{purchaseOrderPK}/Receipts/{receiptPK}/LineItems
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /PurchaseOrders/{purchaseOrderPK}/Receipts/{receiptPK}/LineItems/{lineItemPK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /WorkOrderAssignments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /WorkOrderAssignments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /WorkOrderAssignments/{assignmentPK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /WorkOrderDocuments/{workOrderPK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /WorkOrderImages/{workOrderPK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /WorkOrderLaborActuals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /WorkOrderLaborActuals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /WorkOrderLaborActuals/{costPK}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /WorkOrderLaborEstimates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /WorkOrderLaborEstimates
operation_count: 255
overview: 'Accruent exposes 255 API operations that an AI agent could call, of which 131 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 124 read, 65 write, and 66 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Accruent
provider_slug: accruent
slug: accruent-agentic-access
source_filename: accruent-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: generated\nsource: openapi/accruent-maintenance-connection-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 255\n  by_action_class:\n    connected: 124\n    acting: 131\n  by_consequence:\n    read: 124\n    write: 65\n    physical: 66\n  human_in_the_loop_required: 0\noperations:\n- path: /Assets/{assetPK}/documents\n  method: get\n  operationId: AssetDocuments_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Assets/{assetPK}/documents\n  method: post\n  operationId: AssetDocuments_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/documents/{PK}\n  method: get\n  operationId: AssetDocuments_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetDocuments\n  method: get\n  operationId: AssetDocuments_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetDocuments/{assetPK}\n  method: get\n  operationId: AssetDocuments_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetDocuments/{assetPK}\n  method: post\n  operationId: AssetDocuments_Post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/images\n  method: get\n  operationId: AssetImages_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Assets/{assetPK}/images\n  method: post\n  operationId: AssetImages_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/images/{imagePK}\n  method: get\n  operationId: AssetImages_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /AssetImages\n  method: get\n  operationId: AssetImages_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetImages/{assetPK}\n  method: get\n  operationId: AssetImages_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetImages/{assetPK}\n  method: post\n  operationId: AssetImages_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/meterhistory\n  method: get\n  operationId: AssetMeterHistory_GetMeterHistoryForAsset\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Assets/{assetPK}/meterhistory\n  method: post\n  operationId: AssetMeterHistory_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/meterhistory/{historyPK}\n  method: get\n  operationId: AssetMeterHistory_GetMeterHistoryRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Assets/{assetPK}/meterhistory/{historyPK}\n  method: put\n  operationId: AssetMeterHistory_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/meternumberhistory\n  method: get\n  operationId: AssetMeterHistory_GetMeterHistoryForAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Assets/{assetPK}/meternumberhistory\n  method: put\n  operationId: AssetMeterHistory_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/meternumberhistory\n  method: post\n  operationId: AssetMeterHistory_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/meternumberhistory/{meterNumber}\n  method: get\n  operationId: AssetMeterHistory_GetMeterNumberHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetMeterHistory\n  method: get\n  operationId: AssetMeterHistory_GetMeterHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetMeterHistory\n  method: put\n  operationId: AssetMeterHistory_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /AssetMeterHistory/{assetPK}\n  method: get\n  operationId: AssetMeterHistory_GetMeterHistoryForAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetMeterHistory/{assetPK}\n  method: put\n  operationId: AssetMeterHistory_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AssetMeterHistory/{assetPK}\n  method: post\n  operationId: AssetMeterHistory_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /Assets\n  method: get\n  operationId: Assets_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Assets\n  method: put\n  operationId: Assets_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets\n  method: post\n  operationId: Assets_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}\n  method: get\n  operationId: Assets_Get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Assets/{assetPK}\n  method: put\n  operationId: Assets_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}\n  method: post\n  operationId: Assets_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/specifications/{PK}\n  method: get\n  operationId: AssetSpecifications_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /Assets/{assetPK}/specifications/{PK}\n  method: put\n  operationId: AssetSpecifications_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Assets/{assetPK}/specifications\n  method: get\n  operationId: AssetSpecifications_GetSpecificationsForAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Assets/{assetPK}/specifications\n  method: post\n  operationId: AssetSpecifications_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /AssetSpecifications\n  method: get\n  operationId: AssetSpecifications_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetSpecifications\n  method: put\n  operationId: AssetSpecifications_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AssetSpecifications/{assetPK}\n  method: get\n  operationId: AssetSpecifications_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssetSpecifications/{assetPK}\n  method: put\n  operationId: AssetSpecifications_Put\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AssetSpecifications/{assetPK}\n  method: post\n  operationId: AssetSpecifications_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classifications\n  method: get\n  operationId: Classifications_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classifications\n  method: put\n  operationId: Classifications_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classifications\n  method: post\n  operationId: Classifications_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classifications/{classificationPK}\n  method: get\n  operationId: Classifications_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classifications/{classificationPK}\n  method: put\n  operationId: Classifications_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Companies\n  method: get\n  operationId: Companies_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Companies\n  method: put\n  operationId: Companies_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Companies\n  method: post\n  operationId: Companies_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /Companies/{companyPK}\n  method: get\n  operationId: Companies_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Companies/{companyPK}\n  method: put\n  operationId: Companies_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ExternalInterface\n  method: get\n  operationId: ExternalInterface_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExternalInterface\n  method: post\n  operationId: ExternalInterface_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ExternalInterface/{externalInterfacePK}\n  method: get\n  operationId: ExternalInterface_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExternalInterface/{externalInterfacePK}\n  method: put\n  operationId: ExternalInterface_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Invoices\n  method: get\n  operationId: Invoices_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /Invoices\n  method: put\n  operationId: Invoices_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Invoices\n  method: post\n  operationId: Invoices_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Invoices/{invoicePK}\n  method: get\n  operationId: Invoices_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /Invoices/{invoicePK}\n  method: put\n  operationId: Invoices_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PurchaseOrders/{purchaseOrderPK}/Invoices/{invoicePK}\n  method: get\n  operationId: Invoices_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PurchaseOrders/{purchaseOrderPK}/Invoices/{invoicePK}\n  method: put\n  operationId: Invoices_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PurchaseOrders/{purchaseOrderPK}/Invoices\n  method: get\n  operationId: Invoices_GetInvoicesForPurchaseOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PurchaseOrders/{purchaseOrderPK}/Invoices\n  method: post\n  operationId: Invoices_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Labors\n  method: get\n  operationId: Labors_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /Labors\n  method: put\n  operationId: Labors_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Labors\n  method: post\n  operationId: Labors_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Labors/{laborPK}\n  method: get\n  operationId: Labors_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Labors/{laborPK}\n  method: put\n  operationId: Labors_Put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Labors/{laborPK}\n  method: post\n  operationId: Labors_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Logs\n  method: get\n  operationId: Log_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Logs\n  method: post\n  operationId: Log_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Logs/{logPK}\n  method: get\n  operationId: Log_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LookupTables\n  method: get\n  operationId: LookupTables_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LookupTables\n  method: put\n  operationId: LookupTables_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /LookupTables\n  method: post\n  operationId: LookupTables_Post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /LookupTables/{lookupTableID}\n  method: get\n  operationId: LookupTables_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LookupTables/{lookupTableID}\n  method: put\n  operationId: LookupTables_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /LookupTables/{lookupTableID}/values\n  method: get\n  operationId: LookupTableValues_Get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LookupTables/{lookupTableID}/values\n  method: post\n  operationId: LookupTableValues_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /LookupTables/{lookupTableID}/values/{codeName}\n  method: get\n  operationId: LookupTableValues_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LookupTables/{lookupTableID}/values/{codeName}\n  method: put\n  operationId: LookupTableValues_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /LookupTableValues\n  method: get\n  operationId: LookupTableValues_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LookupTableValues\n  method: put\n  operationId: LookupTableValues_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /LookupTableValues/{lookupTableID}\n  method: get\n  operationId: LookupTableValues_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LookupTableValues/{lookupTableID}\n  method: put\n\
  \  operationId: LookupTableValues_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /LookupTableValues/{lookupTableID}\n  method: post\n  operationId: LookupTableValues_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Parts/{partPK}/documents\n  method: get\n  operationId: PartDocuments_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Parts/{partPK}/documents\n  method: post\n  operationId: PartDocuments_Post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Parts/{partPK}/documents/{PK}\n  method: get\n  operationId: PartDocuments_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PartDocuments\n  method: get\n  operationId: PartDocuments_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PartDocuments/{partPK}\n  method: get\n  operationId: PartDocuments_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PartDocuments/{partPK}\n  method:\
  \ post\n  operationId: PartDocuments_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Parts/{partPK}/locations\n  method: get\n  operationId: PartLocations_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Parts/{partPK}/locations\n  method: post\n  operationId: PartLocations_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Parts/{partPK}/locations/{partLocationPK}\n  method: get\n  operationId: PartLocations_Get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Parts/{partPK}/locations/{partLocationPK}\n  method: put\n  operationId: PartLocations_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PartLocations\n  method: get\n  operationId: PartLocations_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PartLocations\n  method: put\n  operationId: PartLocations_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PartLocations\n  method: post\n  operationId: PartLocations_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PartLocations/{partLocationPK}\n  method: get\n  operationId: PartLocations_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PartLocations/{partLocationPK}\n  method: put\n  operationId: PartLocations_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /Parts\n  method: get\n  operationId: Parts_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Parts\n  method: put\n  operationId: Parts_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Parts\n  method: post\n  operationId: Parts_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Parts/{partPK}\n  method: get\n  operationId: Parts_Get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Parts/{partPK}\n  method: put\n  operationId: Parts_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Parts/{partPK}\n  method: post\n  operationId: Parts_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Parts/{partPK}/transactions\n  method: get\n  operationId: PartTransactions_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /Parts/{partPK}/transactions\n  method: post\n  operationId: PartTransactions_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Parts/{partPK}/transactions/{partTransactionPK}\n  method: get\n  operationId: PartTransactions_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PartTransactions\n  method: get\n  operationId: PartTransactions_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PartTransactions\n  method: post\n  operationId: PartTransactions_Post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escala\n\n# --- truncated at 32 KB (76 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/accruent/refs/heads/main/agentic-access/accruent-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accruent/refs/heads/main/agentic-access/accruent-agentic-access.yml
summary_line: 255 operations · 131 acting
tags:
- Facilities Management
- Asset Management
- CMMS
- EAM
- Maintenance
- Work Orders
- IWMS
- Space Management
- Engineering Document Management
- Built Environment
- Enterprise Software
- Real Estate
---
