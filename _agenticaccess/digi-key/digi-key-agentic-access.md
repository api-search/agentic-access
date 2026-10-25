---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 46
api_specs:
- filename: digi-key-barcoding-api-openapi.yml
  format: yaml
  label: Digi-Key Barcoding API
  slug: digi-key-barcoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-barcoding-api-openapi.yml
- filename: digi-key-bondedinventory-api-openapi.yml
  format: yaml
  label: Digi-Key Bonded Inventory API
  slug: digi-key-bondedinventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-bondedinventory-api-openapi.yml
- filename: digi-key-customerresource-api-openapi.yml
  format: yaml
  label: Digi-Key Customer Resource API
  slug: digi-key-customerresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-customerresource-api-openapi.yml
- filename: digi-key-lists-api-openapi.yml
  format: yaml
  label: Digi-Key Lists API
  slug: digi-key-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-lists-api-openapi.yml
- filename: digi-key-orderhistory-api-openapi.yml
  format: yaml
  label: Digi-Key Order History API
  slug: digi-key-orderhistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-orderhistory-api-openapi.yml
- filename: digi-key-ordermanagement-api-openapi.yml
  format: yaml
  label: Digi-Key Order Management API
  slug: digi-key-ordermanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-ordermanagement-api-openapi.yml
- filename: digi-key-orders-api-openapi.yml
  format: yaml
  label: Digi-Key Orders API
  slug: digi-key-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-orders-api-openapi.yml
- filename: digi-key-packlist-api-openapi.yml
  format: yaml
  label: Digi-Key Pack List API
  slug: digi-key-packlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-packlist-api-openapi.yml
- filename: digi-key-parts-api-openapi.yml
  format: yaml
  label: Digi-Key Parts API
  slug: digi-key-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-parts-api-openapi.yml
- filename: digi-key-pcn-api-openapi.yml
  format: yaml
  label: Digi-Key Pcn API
  slug: digi-key-pcn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-pcn-api-openapi.yml
- filename: digi-key-quotes-api-openapi.yml
  format: yaml
  label: Digi-Key Quotes API
  slug: digi-key-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-quotes-api-openapi.yml
- filename: digi-key-product-search-api-openapi.yml
  format: yaml
  label: Digi-Key Product Search API
  slug: digi-key-product-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-product-search-api-openapi.yml
consequence_counts:
  physical: 3
  read: 46
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Digi Key Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /SalesOrders/{salesOrderId}/Details/{detailId}/Schedules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /SalesOrders/{salesOrderId}/Details/{detailId}/Schedules/{scheduleIndex}
operation_count: 58
overview: 'Digi-Key exposes 58 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read, 9 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Digi-Key
provider_slug: digi-key
slug: digi-key-agentic-access
source_filename: digi-key-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: generated\nsource: openapi/digi-key-b2bapi-order-management-api-ordermanagement-v1-openapi.yml, openapi/digi-key-barcoding-barcoding-v3-openapi.yml,\n  openapi/digi-key-customerresource-customerresource-v1-openapi.yml, openapi/digi-key-mylists-api-mylists-v1-openapi.yml,\n  openapi/digi-key-ordering-api-v3-ordering-v3-openapi.yml, openapi/digi-key-orderstatus-orderstatus-v4-openapi.yml,\n  openapi/digi-key-packinglist-api-packinglist-openapi.yml, openapi/digi-key-product-change-notifications-api-changenotifications-v3-openapi.yml,\n  openapi/digi-key-productsearch-api-products-v4-openapi.yml, openapi/digi-key-quote-api-quoting-v4-openapi.yml,\n  openapi/digi-key-supply-chain-api-supplychain-v1-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 58\n  by_action_class:\n    connected: 46\n    acting: 12\n  by_consequence:\n    read: 46\n    physical: 3\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /SalesOrders/{salesOrderId}\n  method: get\n  operationId: SalesOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SalesOrders/Search/PoNumber/{poNumber}\n  method: get\n  operationId: SalesOrdersByPoNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SalesOrders/{salesOrderId}/ChangeEligibility\n  method: get\n  operationId: ChangeEligibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SalesOrders/{salesOrderId}/NextAvailableDeliveryDate\n  method: get\n \
  \ operationId: NextAvailableDeliveryDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SalesOrders/{salesOrderId}/Details\n  method: get\n  operationId: SalesOrderDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SalesOrders/{salesOrderId}/Details/{detailId}\n  method: get\n  operationId: SalesOrderDetailById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SalesOrders/{salesOrderId}/Details/{detailId}/Schedules\n  method: get\n  operationId: SalesOrderSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SalesOrders/{salesOrderId}/Details/{detailId}/Schedules\n\
  \  method: put\n  operationId: ReplaceSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SalesOrders/{salesOrderId}/Details/{detailId}/Schedules/{scheduleIndex}\n  method: get\n  operationId: SalesOrderScheduleById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SalesOrders/{salesOrderId}/Details/{detailId}/Schedules/{scheduleIndex}\n  method: patch\n  operationId: PartialScheduleUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ProductBarcodes/{barcode}\n  method: get\n  operationId: ProductBarcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Product2DBarcodes/{barcode}\n  method: get\n  operationId: Product2DBarcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PackListBarcodes/{barcode}\n  method: get\n  operationId: PackListBarcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PackList2DBarcodes/{barcode}\n  method: get\n  operationId: PackList2DBarcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /associatedaccounts\n  method: get\n  operationId: AssociatedAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{listId}/parts/{uniqueId}\n  method: get\n  operationId: GetPartFromListByUniqueId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{listId}/parts/{uniqueId}\n  method: put\n  operationId: UpdatePartFromListByUniqueId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{listId}/parts/{uniqueId}\n  method: delete\n  operationId: DeletePartFromListByUniqueId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{listId}\n  method: get\n  operationId: GetListByListId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{listId}\n  method: delete\n  operationId: DeleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists\n  method: get\n  operationId: Lists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /lists\n  method: post\n  operationId: CreateList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/validate/{listName}\n  method: get\n  operationId: IsValidListName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{listId}/parts\n  method: get\n  operationId: GetPartsByListId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{listId}/parts\n  method: post\n  operationId: AddPartsToListId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{listId}/listName/{listName}\n  method: put\n  operationId: UpdateListName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/validate/name/{listName}\n  method: get\n  operationId: ValidListName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Orders\n  method: post\n  operationId: Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: SearchOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salesorder/{salesOrderId}\n  method: get\n  operationId: RetrieveSalesOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoice/{invoiceId}\n  method: get\n  operationId: GetPackingList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/salesorderid/{salesOrderId}\n  method: get\n  operationId: GetPackingListBySalesOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/purchaseordernumber/{purchaseOrderNumber}\n  method: get\n  operationId: GetPackingListByPoNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Products/{DigiKeyPartNumber}\n  method: get\n  operationId: ProductChangeNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/keyword\n  method: post\n  operationId: KeywordSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/{productNumber}/pricing\n  method: get\n  operationId:\
  \ ProductPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/{productNumber}/productdetails\n  method: get\n  operationId: ProductDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/packagetypebyquantity/{productNumber}\n  method: get\n  operationId: PackageTypeByQuantity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/manufacturers\n  method: get\n  operationId: Manufacturers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/{productNumber}/media\n  method: get\n  operationId: Media\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/categories\n  method: get\n  operationId: Categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/categories/{categoryId}\n  method: get\n  operationId: CategoriesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/{productNumber}/alternatepackaging\n  method: get\n  operationId: AlternatePackaging\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/{productNumber}/digireelpricing\n  method: get\n  operationId: DigiReelPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /search/{productNumber}/recommendedproducts\n  method: get\n  operationId: RecommendedProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/{productNumber}/substitutions\n  method: get\n  operationId: Substitutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/{productNumber}/associations\n  method: get\n  operationId: Associations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/{productNumber}/pricingbyquantity/{requestedQuantity}\n  method: get\n  operationId: PricingOptionsByQuantity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /quotes\n  method: post\n  operationId: CreateQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes\n  method: get\n  operationId: AllQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotes/{quoteId}/details\n  method: post\n  operationId: AddProductsToQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes/{quoteId}/details\n  method: get\n  operationId:\
  \ ProductsFromQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotes/{quoteId}\n  method: get\n  operationId: GetQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BondedQuantity/Locations\n  method: get\n  operationId: GetLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BondedQuantity/Products\n  method: get\n  operationId: GetAllProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BondedQuantity/Locations/{accountId}\n  method: get\n  operationId: GetOneLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BondedQuantity/Locations/{accountId}/Products\n  method: get\n  operationId: GetLocationProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BondedQuantity/Locations/{accountId}/Products/{partNumber}\n  method: get\n  operationId: GetProductByPartNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/agentic-access/digi-key-agentic-access.yml
summary_line: 58 operations · 12 acting
tags:
- Shopping
- Public APIs
- Electronic Components
- Distribution
- Ordering
- Product Search
- Pricing
- Inventory
- Supply Chain
---
