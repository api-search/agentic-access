---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 22
api_specs:
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Subscriptions API
  slug: smartrr-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Subscribers API
  slug: smartrr-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Orders and Bills API
  slug: smartrr-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Plans and Purchasables API
  slug: smartrr-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
- filename: smartrr-openapi.yml
  format: yaml
  label: Smartrr Webhooks API
  slug: smartrr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/openapi/smartrr-openapi.yml
consequence_counts:
  physical: 15
  read: 22
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smartrr Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vendor/customer-relationship/import
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer-relationship/{customerRelationshipId}/orgPoints
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer/purchase-state/bulk-cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer/purchase-state/bulk-pause
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/activate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/line-item
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/next-billing-date
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/pause
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/selling-plan
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/skip
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/unskip
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /vendor/order/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vendor/order/{orderId}/open
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vendor/purchase-state
operation_count: 43
overview: 'Smartrr exposes 43 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 6 write, and 15 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Smartrr
provider_slug: smartrr
slug: smartrr-agentic-access
source_filename: smartrr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smartrr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 22\n    acting: 21\n  by_consequence:\n    read: 22\n    physical: 15\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /vendor/purchase-state\n  method: get\n  operationId: getPurchaseStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/purchase-state\n  method: post\n  operationId: createPurchaseState\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/purchase-state/{shopifySubscriptionId}\n  method: get\n  operationId: getPurchaseStateByShopifyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/purchase-state/{shopifySubscriptionId}/orders\n  method: get\n  operationId: getPurchaseStateOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/purchase-state/{shopifySubscriptionId}/bills\n  method: get\n  operationId: getPurchaseStateBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/purchase-state/{shopifySubscriptionId}/events\n\
  \  method: get\n  operationId: getPurchaseStateEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/customer/{customerRelationshipId}/purchase-state/\n  method: get\n  operationId: getPurchaseStatesByCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/skip\n  method: put\n  operationId: skipPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/unskip\n\
  \  method: put\n  operationId: unskipPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/pause\n  method: put\n  operationId: pausePurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/activate\n  method: put\n  operationId: activatePurchase\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/cancel\n  method: put\n  operationId: cancelPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/next-billing-date\n  method: put\n  operationId: setNextBillingDate\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/selling-plan\n  method: put\n  operationId: setSellingPlanOnPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/{customerRelationshipId}/purchase-state/{customerPurchaseStateId}/line-item\n  method: post\n  operationId: addLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/purchase-state/bulk-cancel\n  method: put\n  operationId: bulkCancelPurchases\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/purchase-state/bulk-pause\n  method: put\n  operationId: bulkPausePurchases\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer-relationship\n  method: get\n  operationId: getCustomerRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/customer-relationship/{customerShopifyId}\n  method: get\n  operationId: getCustomerRelationshipByShopifyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/customer-relationship/{customerRelationshipId}/payment-methods\n  method: get\n  operationId: getPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/customer-relationship/{customerShopifyId}/referral-link\n  method:\
  \ get\n  operationId: getReferralLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/customer-relationship/{customerRelationshipId}/orgPoints\n  method: put\n  operationId: addLoyaltyPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer-relationship/import\n  method: post\n  operationId: importCustomerRelationship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/customer/{custRelId}/orders\n  method: get\n  operationId: getOrdersByCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/order\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/order/formatted\n  method: get\n  operationId: getFormattedOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/orders/{shopifyId}\n  method: get\n  operationId: getOrderByShopifyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/order/{orderId}/open\n\
  \  method: post\n  operationId: openOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/order/{orderId}\n  method: delete\n  operationId: closeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/bill\n  method: get\n  operationId: getBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /vendor/bill/{billId}/history\n  method: get\n  operationId: getBillHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/bill/{billId}/retry\n  method: post\n  operationId: retryBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/bill/{billId}/cancel\n  method: post\n  operationId: cancelBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/purchasable\n  method: get\n  operationId: getPurchasables\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/purchasable\n  method: put\n  operationId: updatePurchasable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/purchasable/{id}\n  method: get\n  operationId: getPurchasableById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/purchasable-collection\n  method: get\n  operationId: getPurchasableCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/selling-plan-group\n\
  \  method: get\n  operationId: getSellingPlanGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/selling-plan-configs\n  method: get\n  operationId: getSellingPlanConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/webhook\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/webhook\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /vendor/webhook/{webhookId}\n  method: put\n  operationId: editWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/webhook/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartrr/refs/heads/main/agentic-access/smartrr-agentic-access.yml
summary_line: 43 operations · 21 acting
tags:
- Subscriptions
- Loyalty
- Shopify
- Ecommerce
- DTC
- Recurring Revenue
- Subscription Management
---
