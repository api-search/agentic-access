---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 21
api_specs:
- filename: buyingmesh-com-admin-api-openapi.yml
  format: yaml
  label: BuyingMesh Admin API
  slug: buyingmesh-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-admin-api-openapi.yml
- filename: buyingmesh-com-buyer-confirmations-api-openapi.yml
  format: yaml
  label: BuyingMesh Buyer Confirmations API
  slug: buyingmesh-com-buyer-confirmations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-buyer-confirmations-api-openapi.yml
- filename: buyingmesh-com-inquiries-api-openapi.yml
  format: yaml
  label: BuyingMesh Inquiries API
  slug: buyingmesh-com-inquiries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-inquiries-api-openapi.yml
- filename: buyingmesh-com-landed-cost-api-openapi.yml
  format: yaml
  label: BuyingMesh Landed Cost API
  slug: buyingmesh-com-landed-cost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-landed-cost-api-openapi.yml
- filename: buyingmesh-com-merchant-api-openapi.yml
  format: yaml
  label: BuyingMesh Merchant API
  slug: buyingmesh-com-merchant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-merchant-api-openapi.yml
- filename: buyingmesh-com-orders-api-openapi.yml
  format: yaml
  label: BuyingMesh Orders API
  slug: buyingmesh-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-orders-api-openapi.yml
- filename: buyingmesh-com-products-api-openapi.yml
  format: yaml
  label: BuyingMesh Products API
  slug: buyingmesh-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-products-api-openapi.yml
- filename: buyingmesh-com-quotes-api-openapi.yml
  format: yaml
  label: BuyingMesh Quotes API
  slug: buyingmesh-com-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-quotes-api-openapi.yml
- filename: buyingmesh-com-shipping-api-openapi.yml
  format: yaml
  label: BuyingMesh Shipping API
  slug: buyingmesh-com-shipping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-shipping-api-openapi.yml
- filename: buyingmesh-com-suppliers-api-openapi.yml
  format: yaml
  label: BuyingMesh Suppliers API
  slug: buyingmesh-com-suppliers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-suppliers-api-openapi.yml
- filename: buyingmesh-com-support-api-openapi.yml
  format: yaml
  label: BuyingMesh Support API
  slug: buyingmesh-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-support-api-openapi.yml
- filename: buyingmesh-com-tariffs-api-openapi.yml
  format: yaml
  label: BuyingMesh Tariffs API
  slug: buyingmesh-com-tariffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-tariffs-api-openapi.yml
- filename: buyingmesh-com-webhook-deliveries-api-openapi.yml
  format: yaml
  label: BuyingMesh Webhook Deliveries API
  slug: buyingmesh-com-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-webhook-deliveries-api-openapi.yml
- filename: buyingmesh-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: BuyingMesh Webhook Subscriptions API
  slug: buyingmesh-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyingmesh-com/openapi/buyingmesh-com-webhook-subscriptions-api-openapi.yml
consequence_counts:
  physical: 8
  read: 21
  safety-critical: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Buyingmesh Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/merchant/products/{sku}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/admin/test-catalog/cleanup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{orderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{orderId}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{orderId}/tracking
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{orderId}/tracking/sync
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/support/contact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhook-subscriptions
operation_count: 42
overview: 'BuyingMesh exposes 42 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 12 write, 8 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BuyingMesh
provider_slug: buyingmesh-com
slug: buyingmesh-com-agentic-access
source_filename: buyingmesh-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/buyingmesh-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 21\n    connected: 21\n  by_consequence:\n    physical: 8\n    write: 12\n    read: 21\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/support/contact\n  method: post\n  operationId: contactSupport\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inquiries\n\
  \  method: post\n  operationId: submitInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inquiries/{inquiryId}\n  method: get\n  operationId: getInquiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchant/applications\n  method: post\n  operationId: createMerchantApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchant/products/import\n  method: post\n  operationId: importMerchantProducts\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/applications\n  method: get\n  operationId: listMerchantApplicationsForReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/applications/{applicationId}\n  method: get\n  operationId: getMerchantApplicationForReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/applications/{applicationId}\n  method: post\n  operationId: reviewMerchantApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/suppliers/{supplierId}\n  method: patch\n  operationId: updateSupplierProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/products\n  method: get\n  operationId: listMerchantProductsForReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/traffic\n  method: get\n  operationId: getTrafficSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/admin/products/{productId}\n  method: post\n  operationId: reviewMerchantProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/products\n  method: get\n  operationId: searchProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/suppliers\n  method: get\n  operationId: searchSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/suppliers/{supplierId}\n  method: get\n  operationId: getSupplier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/suppliers/{supplierId}/performance\n  method: get\n  operationId: getSupplierPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/suppliers/{supplierId}/products\n  method: get\n  operationId: listSupplierProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{sku}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchant/products\n  method: get\n  operationId: listMerchantProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchant/products\n  method: post\n\
  \  operationId: createMerchantProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchant/products/{sku}\n  method: patch\n  operationId: updateMerchantProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/quotes\n  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quotes/compare-suppliers\n  method: post\n  operationId: compareSupplierOffers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipping/rates\n  method: post\n  operationId: searchShippingRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tariffs/lookup\n  method: post\n  operationId: lookupTariffs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/landed-cost\n  method: post\n  operationId: estimateLandedCost\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/buyer-confirmations\n  method: post\n  operationId: requestBuyerConfirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quotes/{quoteId}\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{orderId}/status\n  method: post\n  operationId: transitionOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{orderId}/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/orders\n  method: get\n  operationId: adminListOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/catalog-quality\n  method: get\n  operationId: getCatalogQuality\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/test-catalog/cleanup\n  method: post\n  operationId: withdrawInternalTestCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{orderId}/tracking\n  method: post\n  operationId: attachTracking\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{orderId}/tracking/sync\n  method: post\n  operationId: syncTracking\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-subscriptions\n\
  \  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/suppliers/{supplierId}/notification-channel\n  method: get\n  operationId: getSupplierNotificationChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/suppliers/{supplierId}/notification-channel\n  method: patch\n  operationId: updateSupplierNotificationChannel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/suppliers/{supplierId}/notifications\n  method: get\n  operationId: listSupplierNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/buyingmesh-com/agentic-access/buyingmesh-com-agentic-access.yml
summary_line: 42 operations · 21 acting · 1 human-in-the-loop
tags:
- Company
- Procurement
- Artificial Intelligence
- Catalog
- B2B
- Marketplace
---
