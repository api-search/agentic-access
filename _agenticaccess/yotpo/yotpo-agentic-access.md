---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 6
api_specs:
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Reviews & Ratings API
  slug: yotpo-reviews-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Loyalty & Referrals API
  slug: yotpo-loyalty-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo SMS & Email API
  slug: yotpo-sms-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo UGC & Visual API
  slug: yotpo-ugc-visual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Subscriptions API
  slug: yotpo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Webhooks
  slug: yotpo-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
consequence_counts:
  physical: 2
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yotpo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /core/v3/stores/{store_id}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 14
overview: 'Yotpo exposes 14 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yotpo
provider_slug: yotpo
slug: yotpo-agentic-access
source_filename: yotpo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/yotpo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 8\n    connected: 6\n  by_consequence:\n    write: 6\n    read: 6\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_key}/reviews\n  method: get\n  operationId: retrieveAllReviews\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/widget/reviews\n  method: post\n  operationId: createReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{app_key}/{product_id}/bottomline\n  method: get\n  operationId: getProductBottomLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v3/stores/{store_id}/products\n  method: get\n  operationId: retrieveProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v3/stores/{store_id}/products\n\
  \  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v3/stores/{store_id}/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v3/stores/{store_id}/customers\n  method: post\n  operationId: createOrUpdateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v3/stores/{store_id}/webhook_subscriptions\n  method: get\n  operationId: retrieveWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v3/stores/{store_id}/webhook_subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: getLoyaltyCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n\
  \  method: post\n  operationId: createLoyaltyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /redemptions\n  method: post\n  operationId: createRedemption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /redemption_options\n  method: get\n  operationId: listRedemptionOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/agentic-access/yotpo-agentic-access.yml
summary_line: 14 operations · 8 acting
tags:
- eCommerce
- Reviews
- Loyalty
- Retention Marketing
- UGC
---
