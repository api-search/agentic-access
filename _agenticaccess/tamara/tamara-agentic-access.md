---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 6
api_specs:
- filename: tamara-checkout-api-openapi.yml
  format: yaml
  label: Tamara Checkout API
  slug: tamara-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-checkout-api-openapi.yml
- filename: tamara-orders-api-openapi.yml
  format: yaml
  label: Tamara Orders API
  slug: tamara-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-orders-api-openapi.yml
- filename: tamara-payments-api-openapi.yml
  format: yaml
  label: Tamara Payments API
  slug: tamara-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-payments-api-openapi.yml
- filename: tamara-in-store-checkout-api-openapi.yml
  format: yaml
  label: Tamara In-Store Checkout API
  slug: tamara-in-store-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-in-store-checkout-api-openapi.yml
- filename: tamara-webhooks-api-openapi.yml
  format: yaml
  label: Tamara Webhooks API
  slug: tamara-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-webhooks-api-openapi.yml
- filename: tamara-disputes-api-openapi.yml
  format: yaml
  label: Tamara Disputes API
  slug: tamara-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-disputes-api-openapi.yml
- filename: tamara-eligibility-api-openapi.yml
  format: yaml
  label: Tamara Pre-Checkout Eligibility API
  slug: tamara-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-eligibility-api-openapi.yml
- filename: tamara-channel-partners-api-openapi.yml
  format: yaml
  label: Tamara Channel Partners API
  slug: tamara-channel-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-channel-partners-api-openapi.yml
consequence_counts:
  physical: 12
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tamara Agentic Access
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
  path: /checkout/in-store
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/in-store-session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{checkout_id}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /external/merchants/orders/disputes/{dispute_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}/authorise
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/{order_id}/reference-id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/simplified-refund/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pre-checkout/v1/eligibility
operation_count: 23
overview: 'Tamara exposes 23 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 5 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tamara
provider_slug: tamara
slug: tamara-agentic-access
source_filename: tamara-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tamara-channel-partners-api-openapi.yml, openapi/tamara-checkout-api-openapi.yml,\n  openapi/tamara-disputes-api-openapi.yml, openapi/tamara-eligibility-api-openapi.yml, openapi/tamara-in-store-checkout-api-openapi.yml,\n  openapi/tamara-orders-api-openapi.yml, openapi/tamara-payments-api-openapi.yml, openapi/tamara-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 17\n    connected: 6\n  by_consequence:\n    write: 5\n    read: 6\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /channel-partners/merchant-onboarding/create\n  method: post\n  operationId: createMerchantOnboarding\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel-partners/merchant-onboarding/{onboardingCode}\n  method: get\n  operationId: retrieveMerchantOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channel-partners/merchant/{merchantId}/api-key\n  method: get\n  operationId: retrieveMerchantApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channel-partners/webhooks/register\n  method: post\n  operationId: registerChannelPartnerWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel-partners/webhooks\n  method: get\n  operationId: listChannelPartnerWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout\n  method: post\n  operationId: createCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/merchants/orders/disputes/\n  method: get\n  operationId: listDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /external/merchants/orders/disputes/{dispute_id}\n  method: post\n  operationId: updateDispute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pre-checkout/v1/eligibility\n  method: post\n  operationId: preCheckoutEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/in-store-session\n  method: post\n  operationId: createInStoreSmsSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/in-store\n  method: post\n  operationId: createInStoreQrSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/{checkout_id}/void\n  method: post\n  operationId: voidCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}\n  method: get\n  operationId: getOrderDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/authorise\n  method: post\n  operationId: authoriseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/reference-id\n  method: put\n  operationId: updateOrderReferenceId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/capture\n  method: post\n  operationId: captureOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /payments/simplified-refund/{order_id}\n  method: post\n  operationId: simplifiedRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/refund\n  method: post\n  operationId: refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: registerWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: get\n  operationId: retrieveWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhookId}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/agentic-access/tamara-agentic-access.yml
summary_line: 23 operations · 17 acting
tags:
- BNPL
- Buy Now Pay Later
- Fintech
- Payments
- Checkout
- Shariah Compliant
- MENA
- Saudi Arabia
- UAE
- Installments
- Pay Later
- Merchant Services
- Orders
- Refunds
- Captures
- Webhooks
- Disputes
- Channel Partners
- E-commerce
- POS
---
