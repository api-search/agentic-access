---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 37
api_specs:
- filename: xylem-docview-api-openapi.yml
  format: yaml
  label: Xylem Doc View API
  slug: xylem-docview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-docview-api-openapi.yml
- filename: xylem-infor-api-openapi.yml
  format: yaml
  label: Xylem Infor API
  slug: xylem-infor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-infor-api-openapi.yml
- filename: xylem-mes-api-openapi.yml
  format: yaml
  label: Xylem MES API
  slug: xylem-mes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-mes-api-openapi.yml
- filename: xylem-mes-v2-api-openapi.yml
  format: yaml
  label: Xylem MES V2 API
  slug: xylem-mes-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-mes-v2-api-openapi.yml
- filename: xylem-nameplate-api-openapi.yml
  format: yaml
  label: Xylem Name Plate API
  slug: xylem-nameplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-nameplate-api-openapi.yml
- filename: xylem-serialcard-api-openapi.yml
  format: yaml
  label: Xylem Serial Card API
  slug: xylem-serialcard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-serialcard-api-openapi.yml
consequence_counts:
  physical: 9
  read: 37
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xylem Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/DocView/Get/Docs/OrderNumber
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/DocView/Get/Docs/Range
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/MES/Create/BrazedShippingLabels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/MES/Create/BrazedShippingOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/MES/Create/BrazedShopOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/MES/Get/BrazedNamePlate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/MES_v2/Create/PurchaseOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/MES_v2/Create/ShippingLabels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/MES_v2/Create/ShopOrders
operation_count: 57
overview: 'Xylem exposes 57 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 11 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Xylem
provider_slug: xylem
slug: xylem-agentic-access
source_filename: xylem-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: generated\nsource: openapi/xylem-apis-manager-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 37\n    acting: 20\n  by_consequence:\n    read: 37\n    write: 11\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/DocView/Get/DocTypes\n  method: get\n  operationId: DocView_GetDocTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/DocView/Get/DocFields\n  method: get\n  operationId: DocView_GetDocFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/DocView/Get/DocFields/DocTypeId\n  method: get\n  operationId: DocView_GetDocFieldsByDocTypeId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/DocView/Get/Docs\n  method: post\n  operationId: DocView_GetDocs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/DocView/Get/Docs/OrderNumber\n  method: post\n  operationId: DocView_GetDocsByOrderNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/DocView/Get/Docs/Range\n  method: post\n  operationId: DocView_GetDocsByRange\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/DocView/Get/Rep/UserName\n  method: get\n  operationId: DocView_GetRepByUserName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Infor/Get\n  method: post\n  operationId: Infor_Get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/MES/Get/BrazedOrders\n  method: get\n  operationId: MES_GetBrazedOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES/Get/BrazedOrder\n  method: get\n  operationId: MES_GetBrazedOrderByOrderNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES/Get/BrazedStockParts\n  method: get\n  operationId: MES_GetBrazedStockParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES/Get/BrazedStockPart\n  method: get\n  operationId: MES_GetBrazedStockPartByPartNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/MES/Get/BrazedRouting\n  method: get\n  operationId: MES_GetBrazedRoutingByPartNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES/Get/BrazedBOM\n  method: get\n  operationId: MES_GetBrazedBOMByPartNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES/Get/BrazedShopOrders\n  method: get\n  operationId: MES_GetBrazedShopOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES/Get/BrazedShopOrdersPart\n  method: get\n  operationId: MES_GetBrazedShopOrdersByPart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/MES/Get/BrazedShopOrder\n  method: get\n  operationId: MES_GetBrazedShopOrderByOrderNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES/Get/BrazedOrderNotes\n  method: get\n  operationId: MES_GetBrazedOrderNotesByOrderNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES/Get/BrazedNamePlate\n  method: post\n  operationId: MES_GetBrazedNamePlateByOrderNumberLineNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/MES/Get/BrazedShippingOrders\n\
  \  method: get\n  operationId: MES_GetBrazedShippingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES/Create/BrazedShippingOrders\n  method: post\n  operationId: MES_CreateBrazedShippingOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/MES/Create/BrazedShopOrders\n  method: post\n  operationId: MES_CreateBrazedShopOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/MES/Create/BrazedShippingLabels\n  method: post\n  operationId: MES_CreateBrazedShippingLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/MES/Create/BrazedNamePlateLabels\n  method: post\n  operationId: MES_CreateBrazedNamePlateLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/MES_v2/Get/Orders\n  method: get\n  operationId: MES_v2_GetOrders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/Order\n  method: get\n  operationId: MES_v2_GetOrderByOrderNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/OrdersWithBOM\n  method: get\n  operationId: MES_v2_GetOrdersWithBOM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/ShopOrders\n  method: get\n  operationId: MES_v2_GetShopOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/ShopOrdersPart\n  method: get\n  operationId: MES_v2_GetShopOrdersByPart\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/ShopOrder\n  method: get\n  operationId: MES_v2_GetShopOrderByOrderNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/PurchaseOrders\n  method: get\n  operationId: MES_v2_GetPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/PurchaseOrdersPart\n  method: get\n  operationId: MES_v2_GetPurchaseOrdersByPart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/PurchaseOrder\n  method: get\n  operationId: MES_v2_GetPurchaseOrderByOrderNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/StockParts\n  method: get\n  operationId: MES_v2_GetStockParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/StockPart\n  method: get\n  operationId: MES_v2_GetStockPartByPartNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/PurchasedStockParts\n  method: get\n  operationId: MES_v2_GetPurchasedStockParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/PurchasedStockPart\n  method: get\n  operationId: MES_v2_GetPurchasedStockPartByPartNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/Routing\n  method: get\n  operationId: MES_v2_GetRoutingByPartNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/BOM\n  method: get\n  operationId: MES_v2_GetBOMByPartNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/OrderBOM\n  method: get\n  operationId: MES_v2_GetOrderBOMByOrderNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Get/OrderRecursiveBOMOrderNumberandLine\n  method: get\n  operationId: MES_v2_GetOrderRecursiveBOMByOrderNumberandLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MES_v2/Create/ShopOrders\n  method: post\n  operationId: MES_v2_CreateShopOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/MES_v2/Create/PurchaseOrders\n  method: post\n  operationId: MES_v2_CreatePurchaseOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/MES_v2/Create/ShippingLabels\n  method: post\n  operationId: MES_v2_CreateShippingLabels\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/MES_v2/Create/NamePlateLabels\n  method: post\n  operationId: MES_v2_CreateNamePlateLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NamePlate/Run/Task\n  method: get\n  operationId: NamePlate_RunTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/NamePlate/Engrave/Queue\n  method: post\n  operationId:\
  \ NamePlate_EngraveQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NamePlate/Engrave/Layout\n  method: post\n  operationId: NamePlate_EngraveLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NamePlate/Get/Engraved\n  method: post\n  operationId: NamePlate_GetEngraved\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/NamePlate/Get/Queue\n  method: post\n  operationId: NamePlate_GetQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NamePlate/Create/Queue\n  method: post\n  operationId: NamePlate_CreateQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NamePlate/Delete/Queue\n  method: post\n  operationId: NamePlate_DeleteQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NamePlate/ReEngrave/Queue\n  method: post\n  operationId: NamePlate_ReEngraveQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NamePlate/Get/Authorized/SecurityContent\n  method: get\n  operationId: NamePlate_GetAuthorizedBySecurityContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SerialCard/Get/Details\n  method: get\n  operationId: SerialCard_GetDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/SerialCard/Get/LnOrderInfo\n  method: get\n  operationId: SerialCard_GetLnOrderInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SerialCard/Get/LnItemInfo\n  method: get\n  operationId: SerialCard_GetLnItemInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/agentic-access/xylem-agentic-access.yml
summary_line: 57 operations · 20 acting
tags:
- Fortune 1000
- Water
- Water Technology
- Utilities
- Smart Metering
- Industrial IoT
- Water Quality
- Wastewater
- Manufacturing
---
