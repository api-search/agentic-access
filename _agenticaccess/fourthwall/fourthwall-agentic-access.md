---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 25
api_specs:
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Storefront Products API
  slug: fourthwall-storefront-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Storefront Collections API
  slug: fourthwall-storefront-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Storefront Cart & Checkout API
  slug: fourthwall-storefront-cart-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Orders API
  slug: fourthwall-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Products API
  slug: fourthwall-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Gifting & Giveaways API
  slug: fourthwall-gifting-giveaways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Promotions API
  slug: fourthwall-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Memberships API
  slug: fourthwall-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Webhooks API
  slug: fourthwall-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
consequence_counts:
  physical: 2
  read: 25
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fourthwall Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /open-api/v1.0/gifting/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /open-api/v1.0/order/{orderId}/downloaded
operation_count: 43
overview: 'Fourthwall exposes 43 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 16 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fourthwall
provider_slug: fourthwall
slug: fourthwall-agentic-access
source_filename: fourthwall-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fourthwall-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 25\n    acting: 18\n  by_consequence:\n    read: 25\n    write: 16\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/products/{slug}\n  method: get\n  operationId: getStorefrontProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections\n  method: get\n  operationId: getStorefrontCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/collections/{slug}\n  method: get\n  operationId: getStorefrontCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections/{slug}/products\n  method: get\n  operationId: getStorefrontCollectionProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shop\n  method: get\n  operationId: getStorefrontShop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/carts\n  method: post\n  operationId: createCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /v1/carts/{cartId}\n  method: get\n  operationId: getCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/carts/{cartId}/add\n  method: post\n  operationId: addToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/carts/{cartId}/change\n  method: post\n  operationId: changeCartItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/carts/{cartId}/remove\n  method:\
  \ post\n  operationId: removeFromCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/order\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - order_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/order/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - order_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/order/by-friendly-id/{friendlyId}\n  method: get\n  operationId: getOrderByFriendlyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - order_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/order/{orderId}/downloaded\n  method: put\n  operationId: markOrderDownloaded\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - order_write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/products\n  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - offer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - offer_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/products/{productId}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - offer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/products/{productId}\n  method: delete\n  operationId: archiveProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - offer_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/products/{productId}/inventory\n  method: get\n  operationId: getProductInventory\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - offer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/collections\n  method: get\n  operationId: getCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - offer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/collections\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - offer_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/collections/{collectionIdOrSlug}\n  method: get\n  operationId: getCollectionByIdOrSlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   scope:\n    - offer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/collections/{collectionId}/products\n  method: get\n  operationId: getCollectionProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - offer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/collections/{collectionId}/products\n  method: put\n  operationId: setCollectionProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - offer_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/promotions\n  method: get\n  operationId: getPromotions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - promotions_read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/promotions\n  method: post\n  operationId: createPromotion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - promotions_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/promotions/{promotionId}\n  method: get\n  operationId: getPromotion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - promotions_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/promotions/{promotionId}\n  method: put\n  operationId: updatePromotion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - promotions_write\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/gifting/config\n  method: get\n  operationId: getGiftingConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - offer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/gifting/config\n  method: put\n  operationId: updateGiftingConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - offer_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/gifting/checkout\n  method: post\n  operationId: createGiftingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n  \
  \  - offer_write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/gifting/draw/{id}\n  method: get\n  operationId: getGiftDraw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - offer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/gifting/draw/{id}/finish\n  method: put\n  operationId: finishGiftDraw\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - offer_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/giveaways/giveaways\n  method: post\n  operationId: createGiveaway\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - giveaway_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/memberships/tiers\n  method: get\n  operationId: listMembershipTiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memberships_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/memberships/members\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memberships_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/memberships/members/{id}\n  method: get\n  operationId: getMember\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    scope:\n    - memberships_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhook_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhook_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/webhooks/{webhookConfigurationId}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhook_read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api/v1.0/webhooks/{webhookConfigurationId}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhook_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/webhooks/{webhookConfigurationId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhook_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api/v1.0/webhook-events\n  method: get\n  operationId: getWebhookEvents\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhook_read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/agentic-access/fourthwall-agentic-access.yml
summary_line: 43 operations · 18 acting
tags:
- Creator Commerce
- Ecommerce
- Merch
- Storefront
- Memberships
- Donations
- Print on Demand
---
