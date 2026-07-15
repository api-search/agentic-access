---
acting_count: 164
action_class_counts:
  acting: 164
  connected: 79
api_specs:
- filename: ordoro-ordoro-api-openapi.yml
  format: yaml
  label: Ordoro API
  slug: ordoro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordoro/refs/heads/main/openapi/ordoro-ordoro-api-openapi.yml
consequence_counts:
  physical: 106
  read: 79
  safety-critical: 4
  write: 54
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Ordoro Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/order/{order_number}/return_preset/{preset_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v3/order/{order_number}/return_preset/{preset_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/order/{order_number}/shipment_preset/{preset_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v3/order/{order_number}/shipment_preset/{preset_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /product/{sku}/buy/{supplier_id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /product/{sku}/default_dropshipper/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /product/{sku}/default_dropshipper/{supplier_id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /product/{sku}/fulfillment/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase_order/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase_order/tag/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /purchase_order/tag/{name}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /purchase_order/tag/{name}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /purchase_order/{po_id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /purchase_order/{po_id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase_order/{po_id}/comment/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase_order/{po_id}/create_goods_receipt/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase_order/{po_id}/line/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /purchase_order/{po_id}/line/{po_item_id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /purchase_order/{po_id}/line/{po_item_id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase_order/{po_id}/send/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase_order/{po_id}/tag/{tag_name}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /purchase_order/{po_id}/tag/{tag_name}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /rule/reorder/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipper/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /shipper/{shipper_id}/
operation_count: 243
overview: 'Ordoro exposes 243 API operations that an AI agent could call, of which 164 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 79 read, 54 write, 106 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ordoro
provider_slug: ordoro
slug: ordoro-agentic-access
source_filename: ordoro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ordoro-ordoro-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 243\n  by_action_class:\n    connected: 79\n    acting: 164\n  by_consequence:\n    read: 79\n    write: 54\n    physical: 106\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /address/\n  method: get\n  operationId: Address_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /address/\n  method: post\n  operationId: Address_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /address/{address_id}/\n  method: get\n  operationId: AddressByAddressId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /address/{address_id}/\n  method: put\n  operationId: AddressByAddressId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_key/\n  method: get\n  operationId: ApiKey_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_key/\n  method: post\n  operationId: ApiKey_POST\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_key/{api_key_id}/\n  method: delete\n  operationId: ApiKeyByApiKeyId_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_key/{api_key_id}/\n  method: get\n  operationId: ApiKeyByApiKeyId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_key/{api_key_id}/\n  method: put\n  operationId: ApiKeyByApiKeyId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authenticated/\n  method: get\n  operationId: Authenticated_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/\n  method: get\n  operationId: Cart_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/\n  method: post\n  operationId: Cart_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/{cart_id}/\n \
  \ method: get\n  operationId: CartByCartId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/{cart_id}/\n  method: put\n  operationId: CartByCartId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/{cart_id}/warehouse/\n  method: get\n  operationId: CartWarehouseByCartId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/{cart_id}/autosync/\n  method: get\n  operationId: CartAutosyncByCartId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /cart/{cart_id}/autosync/\n  method: delete\n  operationId: CartAutosyncByCartId_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/\n  method: get\n  operationId: Company_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/\n  method: put\n  operationId: Company_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/logo/\n  method: get\n  operationId: CompanyLogo_GET\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/logo/{name}/\n  method: get\n  operationId: CompanyLogoByName_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/logo/{name}/\n  method: put\n  operationId: CompanyLogoByName_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/{company_id}/logo/{name}/\n  method: get\n  operationId: CompanyLogoByCompanyIdAndName_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /company/{company_id}/logo/{name}/raw/\n  method: get\n  operationId: CompanyLogoRawByCompanyIdAndName_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goods_receipt/\n  method: get\n  operationId: GoodsReceipt_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goods_receipt/\n  method: post\n  operationId: GoodsReceipt_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goods_receipt/{goods_receipt_id}/\n  method: delete\n  operationId: GoodsReceiptByGoodsReceiptId_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goods_receipt/{goods_receipt_id}/\n  method: get\n  operationId: GoodsReceiptByGoodsReceiptId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goods_receipt/{goods_receipt_id}/\n  method: put\n  operationId: GoodsReceiptByGoodsReceiptId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goods_receipt/{goods_receipt_id}/comment/\n  method: post\n  operationId: GoodsReceiptCommentByGoodsReceiptId_POST\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goods_receipt/{goods_receipt_id}/comment/\n  method: get\n  operationId: GoodsReceiptCommentByGoodsReceiptId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goods_receipt/{goods_receipt_id}/line/{goods_receipt_item_id}/\n  method: put\n  operationId: GoodsReceiptLineByGoodsReceiptId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/\n  method: get\n  operationId: Integration_GET\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/\n  method: post\n  operationId: Integration_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration/{integration_id}/\n  method: get\n  operationId: IntegrationByIntegrationId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/{integration_id}/\n  method: put\n  operationId: IntegrationByIntegrationId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /label/{label_id}/raw/\n  method: get\n  operationId: LabelRawByLabelId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packing_list/\n  method: get\n  operationId: PackingList_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packing_list/\n  method: post\n  operationId: PackingList_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /packing_list/{packing_list_id}/\n  method: delete\n  operationId: PackingListByPackingListId_DELETE\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /packing_list/{packing_list_id}/\n  method: get\n  operationId: PackingListByPackingListId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packing_list/{packing_list_id}/\n  method: put\n  operationId: PackingListByPackingListId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /packing_list/{packing_list_id}/make_default/\n  method: post\n  operationId: PackingListMakeDefaultByPackingListId_POST\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/\n  method: get\n  operationId: Product_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/\n  method: post\n  operationId: Product_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/\n  method: get\n  operationId: ProductBySku_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /product/{sku}/\n  method: put\n  operationId: ProductBySku_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/archive/\n  method: post\n  operationId: ProductArchiveBySku_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/unarchive/\n  method: post\n  operationId: ProductUnarchiveBySku_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/fulfillment/\n  method: put\n  operationId: ProductFulfillmentBySku_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/image/\n  method: get\n  operationId: ProductImageBySku_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/{sku}/image/\n  method: post\n  operationId: ProductImageBySku_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/kit_component/\n  method: post\n  operationId: ProductKitComponentBySku_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/kit_component/\n  method: put\n  operationId: ProductKitComponentBySku_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/kit_component/\n  method: delete\n  operationId: ProductKitComponentBySku_DELETE\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/kit_graph/\n  method: get\n  operationId: ProductKitGraphBySku_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/{sku}/supplier/{supplier_id}/\n  method: put\n  operationId: ProductSupplierBySkuAndSupplierId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/supplier/{supplier_id}/\n  method: delete\n  operationId: ProductSupplierBySkuAndSupplierId_DELETE\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/default_supplier/\n  method: delete\n  operationId: ProductDefaultSupplierBySku_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/default_supplier/{supplier_id}/\n  method: post\n  operationId: ProductDefaultSupplierBySkuAndSupplierId_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/cart/{cart_id}/\n  method: get\n  operationId: ProductCartBySkuAndCartId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/{sku}/cart/{cart_id}/\n  method: put\n  operationId: ProductCartBySkuAndCartId_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/cart/{cart_id}/extra_info/\n  method: get\n  operationId: ProductCartExtraInfoBySkuAndCartId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/{sku}/cart/{cart_id}/extra_info/\n\
  \  method: post\n  operationId: ProductCartExtraInfoBySkuAndCartId_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/cart/{cart_id}/extra_info/{extra_info_id}\n  method: put\n  operationId: ProductCartExtraInfoBySkuAndCartIdandExtraInfoId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/tag/{name}/\n  method: post\n  operationId: ProductTagBySkuAndName_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/tag/{name}/\n  method: delete\n  operationId: ProductTagBySkuAndName_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/warehouse/{warehouse_id}/\n  method: put\n  operationId: ProductWarehouseBySkuAndWarehouseId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/default_dropshipper/\n  method: delete\n  operationId:\
  \ ProductDefaultDropshipperBySku_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/default_dropshipper/{supplier_id}/\n  method: post\n  operationId: ProductDefaultDropshipperBySku_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/{sku}/buy/{supplier_id}/\n  method: post\n  operationId: ProductBuyBySkuAndSupplierId_POST\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/tag/\n  method: get\n  operationId: ProductTag_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/tag/\n  method: post\n  operationId: ProductTag_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/tag/{tagNamePath}/\n  method: get\n  operationId: ProductTagWithName_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/tag/{tagNamePath}/\n  method: put\n  operationId: ProductTag_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/tag/{tagNamePath}/\n  method: delete\n  operationId: ProductTag_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order\n  method: get\n  operationId: ManufacturingOrder_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v3/manufacturing_order\n  method: post\n  operationId: ManufacturingOrder_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/{reference_id}\n  method: get\n  operationId: ManufacturingOrderByRefId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/manufacturing_order/{reference_id}\n  method: put\n  operationId: ManufacturingOrderByRefId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/counts\n  method: get\n  operationId: ManufacturingOrderCounts_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/manufacturing_order/tag\n  method: post\n  operationId: ManufacturingOrderTags_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/tag\n  method: get\n  operationId: ManufacturingOrderTags_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/manufacturing_order/tag/{name}\n  method: get\n  operationId: ManufacturingOrderTag_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/manufacturing_order/tag/{name}\n  method: put\n  operationId: ManufacturingOrderTags_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/tag/{name}\n  method: delete\n  operationId: ManufacturingOrderTags_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/{reference_id}/tag/{tag_name}\n  method: post\n  operationId: ManufacturingOrderTagPO_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/{reference_id}/tag/{tag_name}\n  method: delete\n  operationId: ManufacturingOrderTagPO_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/{reference_id}/comment\n  method: post\n  operationId: ManufacturingOrderCommentByMoId_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/{reference_id}/comment\n  method: get\n  operationId: ManufacturingOrderCommentByMoId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/manufacturing_order/{reference_id}/line\n  method: post\n  operationId: ManufacturingOrderLine_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/{reference_id}/line/{manufacturing_order_line_id}\n  method: put\n  operationId: ManufacturingOrderLine_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/{reference_id}/line/{manufacturing_order_line_id}\n  method: delete\n  operationId: ManufacturingOrderLine_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/manufacturing_order/{reference_id}/line/{manufacturing_order_line_id}/finish\n  method: post\n  operationId: ManufacturingOrderLineFinished_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase_order/\n  method: get\n  operationId: PurchaseOrder_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchase_order/\n  method: post\n  operationId: PurchaseOrder_POST\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase_order/counts/\n  method: get\n  operationId: PurchaseOrderCounts_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchase_order/{po_id}/\n  method: delete\n  operationId: PurchaseOrderByPoId_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase_order/{po_id}/\n\
  \  method: get\n  operationId: PurchaseOrderByPoId_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchase_order/{po_id}/\n  method: put\n  operationId: PurchaseOrderByPoId_PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase_order/{po_id}/comment/\n  method: post\n  operationId: PurchaseOrderCommentByPoId_POST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \n# --- truncated at 32 KB (81 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/ordoro/refs/heads/main/agentic-access/ordoro-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordoro/refs/heads/main/agentic-access/ordoro-agentic-access.yml
summary_line: 243 operations · 164 acting · 4 human-in-the-loop
tags:
- Order Management
- Inventory Management
- Shipping
- Dropshipping
- Ecommerce
- Multi-Channel
- Fulfillment
- Logistics
---
