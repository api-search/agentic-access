---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 9
api_specs:
- filename: google-play-developer-api.yml
  format: yaml
  label: Google Play Developer APIs
  slug: google-play-developer-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/openapi/google-play-developer-api.yml
consequence_counts:
  physical: 6
  read: 9
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Android Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /applications/{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{packageName}/orders/{orderId}:refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{packageName}/purchases/products/{productId}/tokens/{token}:acknowledge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{packageName}/purchases/products/{productId}/tokens/{token}:consume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:acknowledge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:defer
operation_count: 21
overview: 'Android exposes 21 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 5 write, 6 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Android
provider_slug: android
slug: android-agentic-access
source_filename: android-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-play-developer-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 9\n    acting: 12\n  by_consequence:\n    read: 9\n    physical: 6\n    safety-critical: 1\n    write: 5\n  human_in_the_loop_required: 1\noperations:\n- path: /applications/{packageName}/purchases/products/{productId}/tokens/{token}\n  method: get\n  operationId: getPurchaseProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/purchases/products/{productId}/tokens/{token}:acknowledge\n  method: post\n\
  \  operationId: acknowledgePurchaseProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/purchases/products/{productId}/tokens/{token}:consume\n  method: post\n  operationId: consumePurchaseProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}\n\
  \  method: get\n  operationId: getPurchaseSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:acknowledge\n  method: post\n  operationId: acknowledgePurchaseSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:cancel\n  method: post\n  operationId: cancelPurchaseSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:defer\n  method: post\n  operationId: deferPurchaseSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:revoke\n  method: post\n  operationId: revokePurchaseSubscription\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/purchases/subscriptionsv2/tokens/{token}\n  method: get\n  operationId: getSubscriptionPurchaseV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/purchases/voidedpurchases\n  method: get\n  operationId: listVoidedPurchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/monetization/subscriptions\n\
  \  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/monetization/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/monetization/subscriptions/{productId}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/monetization/subscriptions/{productId}\n\
  \  method: patch\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/monetization/subscriptions/{productId}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/monetization/subscriptions/{productId}/basePlans/{basePlanId}/offers\n  method: get\n  operationId: listSubscriptionOffers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/monetization/subscriptions/{productId}/basePlans/{basePlanId}/offers\n  method: post\n  operationId: createSubscriptionOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/reviews\n  method: get\n  operationId: listReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/reviews/{reviewId}\n  method: get\n  operationId: getReview\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/reviews/{reviewId}:reply\n  method: post\n  operationId: replyToReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidpublisher\n- path: /applications/{packageName}/orders/{orderId}:refund\n  method: post\n  operationId: refundOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - androidpublisher\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/agentic-access/android-agentic-access.yml
summary_line: 21 operations · 12 acting · 1 human-in-the-loop
tags:
- AI
- Android
- Automotive
- Google
- Machine Learning
- Mobile Development
- SDK
- TV
- Wearables
---
