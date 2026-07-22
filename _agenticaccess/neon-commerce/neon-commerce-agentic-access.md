---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 20
api_specs:
- filename: neon-commerce-account-openapi.yml
  format: yaml
  label: Neon Account API
  slug: neon-commerce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-account-openapi.yml
- filename: neon-commerce-assets-openapi.yml
  format: yaml
  label: Neon Assets API
  slug: neon-commerce-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-assets-openapi.yml
- filename: neon-commerce-auth-openapi.yml
  format: yaml
  label: Neon Auth API
  slug: neon-commerce-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-auth-openapi.yml
- filename: neon-commerce-checkout-openapi.yml
  format: yaml
  label: Neon Checkout API
  slug: neon-commerce-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-checkout-openapi.yml
- filename: neon-commerce-payout-openapi.yml
  format: yaml
  label: Neon Payout API
  slug: neon-commerce-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-payout-openapi.yml
- filename: neon-commerce-purchase-openapi.yml
  format: yaml
  label: Neon Purchase API
  slug: neon-commerce-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-purchase-openapi.yml
- filename: neon-commerce-reports-openapi.yml
  format: yaml
  label: Neon Reports API
  slug: neon-commerce-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-reports-openapi.yml
- filename: neon-commerce-status-openapi.yml
  format: yaml
  label: Neon Status API
  slug: neon-commerce-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-status-openapi.yml
- filename: neon-commerce-storefront-openapi.yml
  format: yaml
  label: Neon Storefront API
  slug: neon-commerce-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-storefront-openapi.yml
- filename: neon-commerce-subscriptions-openapi.yml
  format: yaml
  label: Neon Subscriptions API
  slug: neon-commerce-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-subscriptions-openapi.yml
consequence_counts:
  physical: 8
  read: 20
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Neon Commerce Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{checkoutId}/expire
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /client/purchase/{purchaseId}/claim
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchases/webhooks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchases/{purchaseId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /storefront/callbacks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /subscriptions/{subscriptionId}/update-payment-method
operation_count: 48
overview: 'Neon Commerce exposes 48 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 20 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Neon Commerce
provider_slug: neon-commerce
slug: neon-commerce-agentic-access
source_filename: neon-commerce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/neon-commerce-account-openapi.yml, openapi/neon-commerce-assets-openapi.yml,\n  openapi/neon-commerce-auth-openapi.yml, openapi/neon-commerce-checkout-openapi.yml, openapi/neon-commerce-payout-openapi.yml,\n  openapi/neon-commerce-purchase-openapi.yml, openapi/neon-commerce-reports-openapi.yml, openapi/neon-commerce-status-openapi.yml,\n  openapi/neon-commerce-storefront-openapi.yml, openapi/neon-commerce-subscriptions-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    acting: 28\n    connected: 20\n  by_consequence:\n    write: 20\n    read: 20\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /account/merge\n  method: post\n\
  \  operationId: mergeAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/unmerge\n  method: post\n  operationId: unmergeAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/brand-images\n  method: post\n  operationId: createBrandImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /assets/brand-images\n  method: get\n  operationId: getBrandImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/inventory-images\n  method: post\n  operationId: createInventoryImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/inventory-images\n  method: get\n  operationId: getInventoryImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/brand-images/{imageId}\n  method: delete\n  operationId: deleteBrandImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/inventory-images/{imageId}\n  method: delete\n  operationId: deleteInventoryImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/token\n  method: post\n  operationId: createClientToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/checkout\n  method: post\n  operationId: createCheckoutClient\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/{checkoutId}/expire\n  method: post\n  operationId: expireCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pricing-sheet\n  method: get\n  operationId: getActivePricingSheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/{checkoutId}\n  method: get\n  operationId: getCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices\n  method: get\n  operationId: getLocalizedPricingByIpAddressOrCountry\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts\n  method: get\n  operationId: getPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/purchase/{purchaseId}/claim\n  method: patch\n  operationId: clientClaimPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/purchases/unclaimed\n  method: get\n  operationId: clientGetPurchasesUnclaimed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /purchases/search\n  method: get\n  operationId: findPurchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchases/{purchaseId}\n  method: get\n  operationId: getPurchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchases/refunds\n  method: get\n  operationId: getPurchaseRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchases\n  method: get\n  operationId: getPurchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchases/{purchaseId}/refund\n  method: post\n  operationId: refundPurchase\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchases/webhooks\n  method: post\n  operationId: subscribeToWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{reportId}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storefront/items\n  method: post\n  operationId: createStorefrontItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/offer-groups\n  method: post\n  operationId: createStorefrontOfferGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/offers\n  method: post\n  operationId: createStorefrontOffers\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/offers\n  method: get\n  operationId: getStorefrontOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storefront/item/{code}\n  method: delete\n  operationId: deleteStorefrontItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/item/{code}\n  method: get\n  operationId: getStorefrontItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /storefront/item/{code}\n  method: put\n  operationId: updateStorefrontItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/offer/{sku}\n  method: delete\n  operationId: deleteStorefrontOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/offer/{sku}\n  method: get\n  operationId: getStorefrontOffer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /storefront/offer/{sku}\n  method: put\n  operationId: updateStorefrontOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/offer-group/{code}\n  method: delete\n  operationId: deleteStorefrontOfferGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/offer-group/{code}\n  method: get\n  operationId: getStorefrontOfferGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storefront/offer-group/{code}\n\
  \  method: put\n  operationId: updateStorefrontOfferGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/prices\n  method: get\n  operationId: getRegionalPricingByIpAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storefront/theme\n  method: get\n  operationId: getTheme\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storefront/theme\n  method: put\n  operationId: updateTheme\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storefront/callbacks\n  method: post\n  operationId: subscribeToCallbacks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}/update-payment-method\n  method: post\n\
  \  operationId: generateUpdatePaymentMethodUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: postSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/agentic-access/neon-commerce-agentic-access.yml
summary_line: 48 operations · 28 acting
tags:
- Commerce
- Payments
- Gaming
- Checkout
- Storefront
- Direct-to-Consumer
- Subscriptions
- Merchant of Record
- Game Monetization
- Company
---
