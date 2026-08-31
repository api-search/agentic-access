---
acting_count: 39
action_class_counts:
  acting: 39
  connected: 23
api_specs:
- filename: getir-auth-api-openapi.yml
  format: yaml
  label: Getir Auth API
  slug: getir-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-auth-api-openapi.yml
- filename: getir-chain-menus-api-openapi.yml
  format: yaml
  label: Getir Chain Menus API
  slug: getir-chain-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-chain-menus-api-openapi.yml
- filename: getir-changelog-api-openapi.yml
  format: yaml
  label: Getir Changelog API
  slug: getir-changelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-changelog-api-openapi.yml
- filename: getir-food-orders-api-openapi.yml
  format: yaml
  label: Getir Food Orders API
  slug: getir-food-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-food-orders-api-openapi.yml
- filename: getir-health-api-openapi.yml
  format: yaml
  label: Getir Health API
  slug: getir-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-health-api-openapi.yml
- filename: getir-payment-methods-api-openapi.yml
  format: yaml
  label: Getir Payment Methods API
  slug: getir-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-payment-methods-api-openapi.yml
- filename: getir-products-api-openapi.yml
  format: yaml
  label: Getir Products API
  slug: getir-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-products-api-openapi.yml
- filename: getir-restaurants-api-openapi.yml
  format: yaml
  label: Getir Restaurants API
  slug: getir-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-restaurants-api-openapi.yml
consequence_counts:
  physical: 18
  read: 23
  safety-critical: 1
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Getir Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restaurants/courier/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/active
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/periodic/cancelled
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/periodic/unapproved
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/{foodOrderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/{foodOrderId}/deliver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/{foodOrderId}/handover
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/{foodOrderId}/invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /food-orders/{foodOrderId}/invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/{foodOrderId}/invoice-url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/{foodOrderId}/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /food-orders/{foodOrderId}/restaurant-panel-operation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/{foodOrderId}/transfer-to-another-restaurant
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/{foodOrderId}/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /food-orders/{foodOrderId}/verify-scheduled
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /restaurants/payment-methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /restaurants/payment-methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /restaurants/payment-methods/active
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /restaurants/payment-methods/inactive
operation_count: 62
overview: 'Getir exposes 62 API operations that an AI agent could call, of which 39 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 20 write, 18 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Getir
provider_slug: getir
slug: getir-agentic-access
source_filename: getir-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: generated\nsource: openapi/getir-food-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 62\n  by_action_class:\n    connected: 23\n    acting: 39\n  by_consequence:\n    read: 23\n    physical: 18\n    write: 20\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /chain-menus\n  method: get\n  operationId: getChainmenus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog\n  method: get\n  operationId: getChangelog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-methods\n  method: get\n  operationId: getPaymentmethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restaurants\n  method: get\n  operationId: getRestaurants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain-menus/chain-option-categories\n  method: get\n  operationId: getChainmenusChainoptioncategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain-menus/{chainMenuOID}\n  method: get\n  operationId: getChainmenusChainmenuoid\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-orders/report\n  method: get\n  operationId: getFoodordersReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-orders/{foodOrderId}\n  method: get\n  operationId: getFoodordersFoodorderid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restaurants/menu\n  method: get\n  operationId: getRestaurantsMenu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restaurants/option-products\n  method: get\n  operationId: getRestaurantsOptionproducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /restaurants/payment-methods\n  method: get\n  operationId: getRestaurantsPaymentmethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restaurants/payment-methods\n  method: post\n  operationId: postRestaurantsPaymentmethods\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/payment-methods\n  method: delete\n  operationId: deleteRestaurantsPaymentmethods\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/reviews\n  method: get\n  operationId: getRestaurantsReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restaurants/working-hours\n  method: get\n  operationId: getRestaurantsWorkinghours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restaurants/working-hours\n  method: put\n  operationId: putRestaurantsWorkinghours\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /restaurants/zones\n  method: get\n  operationId: getRestaurantsZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-orders/report/details\n  method: get\n  operationId: getFoodordersReportDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-orders/{foodOrderId}/cancel-options\n  method: get\n  operationId: getFoodordersFoodorderidCanceloptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-orders/{foodOrderId}/invoice\n  method: get\n  operationId: getFoodordersFoodorderidInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food-orders/{foodOrderId}/invoice\n\
  \  method: post\n  operationId: postFoodordersFoodorderidInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/invoice\n  method: delete\n  operationId: deleteFoodordersFoodorderidInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/available-restaurants-for-transfer\n  method: get\n  operationId: getFoodordersFoodorderidAvailablerestaurantsfortransfer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productId}/status\n  method: get\n  operationId: getProductsProductidStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productId}/status\n  method: put\n  operationId: putProductsProductidStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/zones/eta\n  method: get\n  operationId: getRestaurantsZonesEta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /restaurants/zones/{zoneId}\n  method: get\n  operationId: getRestaurantsZonesZoneid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/chain-id/{chainProductId}/status\n  method: get\n  operationId: getProductsChainidChainproductidStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/chain-id/{chainProductId}/status\n  method: put\n  operationId: putProductsChainidChainproductidStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login\n  method: post\n  operationId: postAuthLogin\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/active\n  method: post\n  operationId: postFoodordersActive\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/pos-status\n  method: post\n  operationId: postRestaurantsPosstatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /restaurants/pos-status\n  method: put\n  operationId: putRestaurantsPosstatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain-menus/{chainMenuOID}/update-prices\n  method: post\n  operationId: postChainmenusChainmenuoidUpdateprices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/periodic/cancelled\n  method: post\n  operationId: postFoodordersPeriodicCancelled\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/periodic/unapproved\n  method: post\n  operationId: postFoodordersPeriodicUnapproved\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/cancel\n  method: post\n  operationId: postFoodordersFoodorderidCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/deliver\n  method: post\n  operationId: postFoodordersFoodorderidDeliver\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/prepare\n  method: post\n  operationId: postFoodordersFoodorderidPrepare\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/verify\n\
  \  method: post\n  operationId: postFoodordersFoodorderidVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/verify-scheduled\n  method: post\n  operationId: postFoodordersFoodorderidVerifyscheduled\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/invoice-url\n  method: post\n  operationId: postFoodordersFoodorderidInvoiceurl\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/handover\n  method: post\n  operationId: postFoodordersFoodorderidHandover\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/transfer-to-another-restaurant\n  method: post\n  operationId: postFoodordersFoodorderidTransfertoanotherrestaurant\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{productId}/inactivate-as-option\n  method: post\n  operationId: postProductsProductidInactivateasoption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{productId}/activate-as-option\n  method: post\n  operationId: postProductsProductidActivateasoption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /restaurants/courier/disable\n  method: post\n  operationId: postRestaurantsCourierDisable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /restaurants/courier/enable\n  method: post\n  operationId: postRestaurantsCourierEnable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/payment-methods/active\n  method: post\n  operationId: postRestaurantsPaymentmethodsActive\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/payment-methods/inactive\n  method: post\n  operationId: postRestaurantsPaymentmethodsInactive\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/chain-id/{chainProductId}/inactivate-as-option\n  method: post\n  operationId: postProductsChainidChainproductidInactivateasoption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/chain-id/{chainProductId}/activate-as-option\n  method: post\n  operationId: postProductsChainidChainproductidActivateasoption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/average-preparation-time\n  method: put\n  operationId: putRestaurantsAveragepreparationtime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /food-orders/{foodOrderId}/restaurant-panel-operation\n\
  \  method: put\n  operationId: putFoodordersFoodorderidRestaurantpaneloperation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/delivery-duration/busyness\n  method: put\n  operationId: putRestaurantsDeliverydurationBusyness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/status/close\n  method: put\n  operationId: putRestaurantsStatusClose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/status/open\n  method: put\n  operationId: putRestaurantsStatusOpen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/zones/{zoneId}/active\n  method: put\n  operationId: putRestaurantsZonesZoneidActive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/zones/{zoneId}/inactive\n  method: put\n  operationId: putRestaurantsZonesZoneidInactive\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/{restaurantId}/zones/{zoneId}\n  method: put\n  operationId: putRestaurantsRestaurantidZonesZoneid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/option-products/chain-id/{chainOptionProductId}/option-categories/{chainOptionCategoryId}/options/{chainOptionId}/status\n  method: put\n  operationId: putRestaurantsOptionproductsChainidChainoptionproductidOptioncategoriesChainoptioncategoryidOptionsChainoptionidStatus\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/agentic-access/getir-agentic-access.yml
summary_line: 62 operations · 39 acting · 1 human-in-the-loop
tags:
- Company
- Food Delivery
- Grocery Delivery
- On-Demand Delivery
- Logistics
- Restaurant
- Point-of-Sale
- Marketplace
- Turkey
- Partner Integration
---
