---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 39
api_specs:
- filename: byrd-account-api-openapi.yml
  format: yaml
  label: Byrd Account API
  slug: byrd-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/byrd/refs/heads/main/openapi/byrd-account-api-openapi.yml
- filename: byrd-authentication-api-openapi.yml
  format: yaml
  label: Byrd Authentication API
  slug: byrd-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/byrd/refs/heads/main/openapi/byrd-authentication-api-openapi.yml
- filename: byrd-catalog-api-openapi.yml
  format: yaml
  label: Byrd Catalog API
  slug: byrd-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/byrd/refs/heads/main/openapi/byrd-catalog-api-openapi.yml
- filename: byrd-inbound-api-openapi.yml
  format: yaml
  label: Byrd Inbound API
  slug: byrd-inbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/byrd/refs/heads/main/openapi/byrd-inbound-api-openapi.yml
- filename: byrd-shipments-api-openapi.yml
  format: yaml
  label: Byrd Shipments API
  slug: byrd-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/byrd/refs/heads/main/openapi/byrd-shipments-api-openapi.yml
consequence_counts:
  physical: 11
  read: 39
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Byrd Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/returns/announce
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/returns/{return_id}/documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/shipments/recall
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/shipments/release
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v3/shipments/{shipment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v3/shipments/{shipment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/shipments/{shipment_id}/documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/shipments/{shipment_id}/recall
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/shipments/{shipment_id}/schedule-pickup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/shipments/{shipment_id}/validate-address
operation_count: 69
overview: 'Byrd exposes 69 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 39 read, 19 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Byrd
provider_slug: byrd
slug: byrd-agentic-access
source_filename: byrd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/byrd-apis-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    connected: 39\n    acting: 30\n  by_consequence:\n    read: 39\n    write: 19\n    physical: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/auth\n  method: get\n  operationId: authapiv2_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/b2b_config/{b2b_config_id}\n  method: get\n  operationId: b2bconfigapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/b2b_config_templates\n  method: get\n  operationId: b2bconfigtemplateapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/export/user/{user_id}/returns\n  method: get\n  operationId: returnsexportapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/export/user/{user_id}/shipments\n  method: get\n  operationId: shipmentexportapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/login\n  method: post\n  operationId: loginapiv2_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/refresh_token\n  method: post\n  operationId: refreshtokenapi_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/returns\n  method: get\n  operationId: returnshipmentlistapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/returns/{return_id}\n  method: get\n  operationId: returnshipmentdetailapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/users/{user_id}\n  method: patch\n  operationId: userapiv2_patch\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/dangerous-goods-limits\n  method: get\n  operationId: dangerousgoodsunitlimitsapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/deliveries\n  method: get\n  operationId: deliveriesapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/deliveries\n  method: post\n  operationId: deliveriesapi_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/deliveries/{delivery_id}\n  method: get\n  operationId: deliveryapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/deliveries/{delivery_id}\n  method: put\n  operationId: deliveryapi_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/deliveries/{delivery_id}\n  method: patch\n  operationId: deliveryapi_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/deliveries/{delivery_id}\n  method: delete\n  operationId: deliveryapi_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/deliveries/{delivery_id}/lots\n  method: get\n  operationId: deliverylotsapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/delivery-documents\n  method: get\n  operationId: deliverydocumentsapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/delivery-documents\n  method: post\n  operationId:\
  \ deliverydocumentsapi_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/delivery-documents/{document_id}\n  method: patch\n  operationId: deliverydocumentapi_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/delivery-documents/{document_id}\n  method: delete\n  operationId: deliverydocumentapi_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/delivery-items/{item_id}\n  method: get\n  operationId: deliveryitemapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/export/user/{user_id}/inventory\n  method: get\n  operationId: inventoryexportapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/lots\n  method: get\n  operationId: lotlistapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/lots\n  method: post\n  operationId: lotlistapi_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/lots/{lot_id}\n  method: get\n  operationId: lotdetailapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/lots/{lot_id}\n  method: patch\n  operationId: lotdetailapi_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/products\n  method: get\n  operationId: productsapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/products\n\
  \  method: post\n  operationId: productsapi_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/products/{bundle_id}/bundles\n  method: get\n  operationId: bundlelistapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/products/{bundle_id}/bundles\n  method: post\n  operationId: bundlelistapi_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/products/{bundle_id}/bundles\n\
  \  method: put\n  operationId: bundlelistapi_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/products/{bundle_id}/bundles/{ingredient_id}\n  method: get\n  operationId: bundledetailsapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/products/{bundle_id}/bundles/{ingredient_id}\n  method: delete\n  operationId: bundledetailsapi_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v2/warehouse/products/{product_id}\n  method: get\n  operationId: productapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/products/{product_id}\n  method: put\n  operationId: productapi_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/products/{product_id}\n  method: patch\n  operationId: productapi_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/products/{product_id}\n\
  \  method: delete\n  operationId: productapi_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse/products/{product_id}/serial-numbers\n  method: get\n  operationId: productserialnumbersapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/products/{product_id}/stats\n  method: get\n  operationId: productstatsapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/products/{product_id}/stock-by-warehouse\n  method: get\n  operationId: productstockbywarehouseapi_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/user-warehouse-links\n  method: get\n  operationId: userwarehouselinksapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/warehouses\n  method: get\n  operationId: warehousesapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse/warehouses/{warehouse_id}\n  method: get\n  operationId: warehouseapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/deliveries/count\n  method: get\n  operationId: deliverylistcountapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/picks\n  method: get\n  operationId: picklistapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/returns/announce\n  method: post\n  operationId: returnshipmentannouncedapiv3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/returns/{return_id}/documents\n  method: post\n  operationId: returnshipmentdocumentsapiv3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipments\n  method: get\n  operationId: shipmentlistapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/shipments\n  method: post\n  operationId: shipmentlistapiv3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipments/count\n  method: get\n  operationId: shipmentlistcountapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v3/shipments/recall\n  method: post\n  operationId: shipmentbatchrecallapiv3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipments/release\n  method: post\n  operationId: shipmentbatchreleaseapiv3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipments/report\n  method: get\n  operationId: shipmentreportapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/shipments/{shipment_id}\n  method: get\n  operationId: shipmentapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/shipments/{shipment_id}\n  method: patch\n  operationId: shipmentapiv3_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipments/{shipment_id}\n  method: delete\n  operationId: shipmentapiv3_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n \
  \     purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipments/{shipment_id}/documents\n  method: get\n  operationId: shipmentdocumentsbatchapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/shipments/{shipment_id}/documents\n  method: post\n  operationId: shipmentdocumentsbatchapiv3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipments/{shipment_id}/documents/{document_id}/file\n  method: get\n  operationId: shipmentdocumentfileapiv3_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/shipments/{shipment_id}/picks\n  method: get\n  operationId: shipmentpicklistapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/shipments/{shipment_id}/recall\n  method: post\n  operationId: shipmentrecallapiv3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipments/{shipment_id}/reservations\n  method: get\n  operationId: shipmentreservationlistapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/shipments/{shipment_id}/schedule-pickup\n  method: post\n  operationId: schedulepickupapiv3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipments/{shipment_id}/units/{unit_id}\n  method: get\n  operationId: shipmentunitapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/shipments/{shipment_id}/validate-address\n  method: post\n  operationId: shipmentaddressvalidationapiv3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/units\n  method: get\n  operationId: unitlistapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/units/count\n  method: get\n  operationId: unitlistcountapiv3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byrd/refs/heads/main/agentic-access/byrd-agentic-access.yml
summary_line: 69 operations · 30 acting
tags:
- Company
- E-Commerce
- Fulfillment
- Logistics
- 3PL
- Shipping
- Warehousing
- Order Management
- Inventory
- Returns
- Supply Chain
---
