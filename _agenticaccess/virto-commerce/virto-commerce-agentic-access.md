---
acting_count: 283
action_class_counts:
  acting: 283
  connected: 143
api_specs:
- filename: VirtoCommerce.Catalog
  format: yaml
  label: Virto Commerce Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Catalog
- filename: VirtoCommerce.Pricing
  format: yaml
  label: Virto Commerce Pricing API
  slug: pricing
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Pricing
- filename: VirtoCommerce.Inventory
  format: yaml
  label: Virto Commerce Inventory API
  slug: inventory
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Inventory
- filename: VirtoCommerce.Orders
  format: yaml
  label: Virto Commerce Order Management API
  slug: orders
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Orders
- filename: VirtoCommerce.Cart
  format: yaml
  label: Virto Commerce Shopping Cart API
  slug: cart
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Cart
- filename: VirtoCommerce.Customer
  format: yaml
  label: Virto Commerce Customer API
  slug: customer
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Customer
- filename: VirtoCommerce.Marketing
  format: yaml
  label: Virto Commerce Marketing API
  slug: marketing
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Marketing
- filename: VirtoCommerce.Quote
  format: yaml
  label: Virto Commerce Quotes API
  slug: quotes
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Quote
- filename: VirtoCommerce.Store
  format: yaml
  label: Virto Commerce Store API
  slug: store
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Store
- filename: VirtoCommerce.Platform
  format: yaml
  label: Virto Commerce Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Platform
consequence_counts:
  physical: 37
  read: 143
  safety-critical: 9
  write: 237
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 9
kind: agentic-access
layout: agentic-access
method: generated
name: Virto Commerce Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/changes/changed-entities/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/platform-cache/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/platform/security/users/{loginOrEmail}/requestpasswordreset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/platform/security/users/{userId}/resetpasswordconfirm
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/platform/security/users/{userId}/sessions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/platform/security/users/{userId}/sessions/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/platform/security/users/{userId}/validatepasswordresettoken
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/platform/security/users/{userName}/resetpassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /revoke/token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/carts/availshippingrates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/carts/patch/{cartId}/payments/{paymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/carts/patch/{cartId}/shipments/{shipmentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/carts/{cartId}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/carts/{cartId}/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/inventory/fulfillmentcenters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/inventory/fulfillmentcenters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/inventory/fulfillmentcenters/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/inventory/fulfillmentcenters/plenty
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/inventory/fulfillmentcenters/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/inventory/fulfillmentcenters/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/order/customerOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/order/customerOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/order/customerOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/order/customerOrders/indexed/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/order/customerOrders/recalculate
operation_count: 426
overview: 'Virto Commerce exposes 426 API operations that an AI agent could call, of which 283 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 143 read, 237 write, 37 physical, and 9 safety-critical.


  9 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Virto Commerce
provider_slug: virto-commerce
slug: virto-commerce-agentic-access
source_filename: virto-commerce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/virto-commerce-cart-openapi.json, openapi/virto-commerce-catalog-openapi.json,\n  openapi/virto-commerce-customer-openapi.json, openapi/virto-commerce-inventory-openapi.json,\n  openapi/virto-commerce-marketing-openapi.json, openapi/virto-commerce-orders-openapi.json,\n  openapi/virto-commerce-platform-openapi.json, openapi/virto-commerce-pricing-openapi.json,\n  openapi/virto-commerce-quote-openapi.json, openapi/virto-commerce-store-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 426\n  by_action_class:\n    connected: 143\n    acting: 283\n  by_consequence:\n    read: 143\n    write: 237\n    physical: 37\n    safety-critical: 9\n  human_in_the_loop_required: 9\noperations:\n\
  - path: /api/carts/{storeId}/{customerId}/{cartName}/{currency}/{cultureName}/current\n  method: get\n  operationId: CartModule_GetCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/carts/{cartId}/itemscount\n  method: get\n  operationId: CartModule_GetCartItemsCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/carts/{cartId}/items\n  method: post\n  operationId: CartModule_AddItemToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/{cartId}/items\n  method: put\n  operationId: CartModule_ChangeCartItem\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/{cartId}/items\n  method: delete\n  operationId: CartModule_ClearCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/{cartId}/items/{lineItemId}\n  method: delete\n  operationId: CartModule_RemoveCartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/carts/{cartId}\n  method: patch\n  operationId: CartModule_MergeWithCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/{cartId}\n  method: get\n  operationId: CartModule_GetCartById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/carts/{cartId}/availshippingrates\n  method: get\n  operationId: CartModule_GetAvailableShippingRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/carts/availshippingrates\n  method: post\n  operationId: CartModule_GetAvailableShippingRatesByContext\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/{cartId}/availpaymentmethods\n  method: get\n  operationId: CartModule_GetAvailablePaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/carts/{cartId}/coupons/{couponCode}\n  method: post\n  operationId: CartModule_AddCartCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/{cartId}/coupons/{couponCode}\n  method:\
  \ delete\n  operationId: CartModule_RemoveCartCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/{cartId}/shipments\n  method: post\n  operationId: CartModule_AddOrUpdateCartShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/{cartId}/payments\n  method: post\n  operationId: CartModule_AddOrUpdateCartPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/search\n  method: post\n  operationId: CartModule_SearchShoppingCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cart:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts\n  method: post\n  operationId: CartModule_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cart:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts\n  method:\
  \ put\n  operationId: CartModule_UpdateShoppingCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cart:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts\n  method: delete\n  operationId: CartModule_DeleteCarts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cart:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/recalculate\n  method: post\n  operationId: CartModule_RecalculateTotals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/patch/{id}\n  method: patch\n  operationId: CartModule_PatchCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cart:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/patch/{cartId}/items/{lineItemId}\n  method: patch\n  operationId: CartModule_PatchCartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cart:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/patch/{cartId}/shipments/{shipmentId}\n  method: patch\n\
  \  operationId: CartModule_PatchCartShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - cart:update\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/carts/patch/{cartId}/payments/{paymentId}\n  method: patch\n  operationId: CartModule_PatchCartPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - cart:update\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/automatic-link-queries/search\n  method: post\n  operationId: AutomaticLinkQuery_Search\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/automatic-link-queries\n  method: post\n  operationId: AutomaticLinkQuery_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/automatic-link-queries\n  method: put\n  operationId: AutomaticLinkQuery_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:update\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/automatic-link-queries\n  method: delete\n  operationId: AutomaticLinkQuery_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/automatic-link-queries/{id}\n  method: get\n  operationId: AutomaticLinkQuery_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/products/associations/{productId}\n  method: get\n  operationId: CatalogModuleAssociations_GetProductAssociations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/products/associations/get/multiple\n  method: post\n  operationId: CatalogModuleAssociations_GetProductsAssociations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products/associations\n  method: post\n  operationId: CatalogModuleAssociations_UpdateAssociations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/catalog/products/associations\n  method: delete\n  operationId: CatalogModuleAssociations_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products/associations/search\n  method: post\n  operationId: CatalogModuleAssociations_Search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products/associations/{id}\n  method: patch\n  operationId: CatalogModuleAssociations_PatchAssociation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brand-settings/store/{storeId}\n  method: get\n  operationId: CatalogModuleBrandSetting_GetByStoreId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/brand-settings\n  method: put\n  operationId: CatalogModuleBrandSetting_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/catalogs/search\n\
  \  method: post\n  operationId: CatalogModuleCatalogs_SearchCatalogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/catalogs/{id}\n  method: get\n  operationId: CatalogModuleCatalogs_GetCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/catalogs/{id}\n  method: delete\n  operationId: CatalogModuleCatalogs_DeleteCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/catalog/catalogs/{id}\n  method: patch\n  operationId: CatalogModuleCatalogs_PatchCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/catalogs/outer/{outerId}\n  method: get\n  operationId: CatalogModuleCatalogs_GetCatalogByOuterId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/catalogs/getnew\n  method: get\n  operationId: CatalogModuleCatalogs_GetNewCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:create\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/catalogs/getnewvirtual\n  method: get\n\
  \  operationId: CatalogModuleCatalogs_GetNewVirtualCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:create\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/catalogs\n  method: post\n  operationId: CatalogModuleCatalogs_CreateCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/catalogs\n  method: put\n  operationId: CatalogModuleCatalogs_UpdateCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/categories/{id}\n  method: get\n  operationId: CatalogModuleCategories_GetCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/categories/{id}\n  method: patch\n  operationId: CatalogModuleCategories_PatchCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/categories/outer/{outerId}\n  method: get\n  operationId: CatalogModuleCategories_GetCategoryByOuterId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/categories\n\
  \  method: get\n  operationId: CatalogModuleCategories_GetCategoriesByIdsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/categories\n  method: post\n  operationId: CatalogModuleCategories_CreateOrUpdateCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/categories\n  method: delete\n  operationId: CatalogModuleCategories_DeleteCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /api/catalog/categories/plenty\n  method: post\n  operationId: CatalogModuleCategories_GetCategoriesByPlentyIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/{catalogId}/categories-by-codes\n  method: post\n  operationId: CatalogModuleCategories_GetCategoriesByCodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/{catalogId}/categories/newcategory\n  method: get\n  operationId: CatalogModuleCategories_GetNewCategory\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/categories/batch\n  method: post\n  operationId: CatalogModuleCategories_SaveCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/categories/{id}/automatic-links\n  method: post\n  operationId: CatalogModuleCategories_UpdateAutomaticLinks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/categories/{id}/automatic-links\n  method: delete\n  operationId: CatalogModuleCategories_DeleteAutomaticLinks\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products/configurations/{id}\n  method: get\n  operationId: CatalogModuleConfigurations_GetConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - catalog:configurations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/products/configurations/{id}\n  method: patch\n  operationId: CatalogModuleConfigurations_PatchConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:configurations:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products/configurations/search\n  method: post\n  operationId: CatalogModuleConfigurations_SearchConfigurations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:configurations:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products/configurations\n  method: post\n  operationId: CatalogModuleConfigurations_CreateOrUpdateConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - catalog:configurations:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/search/products\n\
  \  method: post\n  operationId: CatalogModuleIndexedSearch_SearchProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/search/products/suggestions\n  method: post\n  operationId: CatalogModuleIndexedSearch_GetProductSuggestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/search/categories\n  method: post\n  operationId: CatalogModuleIndexedSearch_SearchCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/listentries\n  method: post\n  operationId: CatalogModuleListEntry_ListItemsSearchAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/listentrylinks\n  method: post\n  operationId: CatalogModuleListEntry_CreateLinks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/listentrylinks/bulkcreate\n  method: post\n  operationId: CatalogModuleListEntry_BulkCreateLinks\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/listentrylinks/search\n  method: post\n  operationId: CatalogModuleListEntry_SearchLinks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/listentrylinks/delete\n  method: post\n  operationId: CatalogModuleListEntry_DeleteLinks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/listentries/move\n  method: post\n  operationId: CatalogModuleListEntry_Move\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/listentries/delete\n  method: post\n  operationId: CatalogModuleListEntry_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/measures/{id}\n  method: get\n  operationId: CatalogModuleMeasures_GetMeasureById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - measures:access\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/measures/{id}\n  method: patch\n  operationId: CatalogModuleMeasures_PatchMeasure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - measures:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/measures/search\n  method: post\n  operationId: CatalogModuleMeasures_SearchMeasures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - measures:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/measures\n  method: post\n  operationId: CatalogModuleMeasures_CreateMeasure\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - measures:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/measures\n  method: put\n  operationId: CatalogModuleMeasures_UpdateMeasure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - measures:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/measures\n  method: delete\n  operationId: CatalogModuleMeasures_DeleteMeasures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - measures:delete\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/measures/default\n  method: get\n  operationId: CatalogModuleMeasures_GetDefaultMeasures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - measures:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/products/{id}\n  method: get\n  operationId: CatalogModuleProducts_GetProductById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/products/{id}\n  method: patch\n  operationId: CatalogModuleProducts_PatchProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products/outer/{outerId}\n  method: get\n  operationId: CatalogModuleProducts_GetProductByOuterId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/{catalogId}/products-by-codes\n  method: post\n  operationId: CatalogModuleProducts_GetByCodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products\n  method: get\n  operationId: CatalogModuleProducts_GetProductByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/products\n  method:\
  \ post\n  operationId: CatalogModuleProducts_SaveProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products\n  method: delete\n  operationId: CatalogModuleProducts_DeleteProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products\n  method: patch\n  operationId: CatalogModuleProducts_BulkPatchProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/products/plenty\n  method: post\n  operationId: CatalogModuleProducts_GetProductByPlentyIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/catalog/{catalogId}/products/getnew\n  method: get\n  operationId: CatalogModuleProducts_GetNewProductByCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/{catalogId}/categories/{categoryId}/products/getnew\n  method: get\n  operationId: CatalogModuleProducts_GetNewProductByCatalogAndCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ \n\n# --- truncated at 32 KB (148 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/agentic-access/virto-commerce-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/agentic-access/virto-commerce-agentic-access.yml
summary_line: 426 operations · 283 acting · 9 human-in-the-loop
tags:
- B2B E-Commerce
- Catalog Management
- Order Management
- Pricing
- Inventory
- Shopping Cart
- Customer Management
- Marketing
- Payments
- Shipping
- Subscriptions
- Headless Commerce
- Open Source
- .NET
---
