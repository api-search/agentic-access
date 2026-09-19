---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 3
api_specs:
- filename: tamara-captures-api-openapi.yml
  format: yaml
  label: Tamara Captures API
  slug: tamara-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-captures-api-openapi.yml
- filename: tamara-channel-partner-webhooks-api-openapi.yml
  format: yaml
  label: Tamara Channel Partner Webhooks API
  slug: tamara-channel-partner-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-channel-partner-webhooks-api-openapi.yml
- filename: tamara-checkout-sessions-api-openapi.yml
  format: yaml
  label: Tamara Checkout Sessions API
  slug: tamara-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-checkout-sessions-api-openapi.yml
- filename: tamara-merchant-api-keys-api-openapi.yml
  format: yaml
  label: Tamara Merchant API Keys API
  slug: tamara-merchant-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-merchant-api-keys-api-openapi.yml
- filename: tamara-merchant-onboarding-api-openapi.yml
  format: yaml
  label: Tamara Merchant Onboarding API
  slug: tamara-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-merchant-onboarding-api-openapi.yml
- filename: tamara-refunds-api-openapi.yml
  format: yaml
  label: Tamara Refunds API
  slug: tamara-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-refunds-api-openapi.yml
consequence_counts:
  physical: 4
  read: 3
  write: 2
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
operation_count: 9
overview: 'Tamara exposes 9 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 2 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tamara
provider_slug: tamara
slug: tamara-agentic-access
source_filename: tamara-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/tamara-captures-api-openapi.yml, openapi/tamara-channel-partner-webhooks-api-openapi.yml,\n  openapi/tamara-checkout-sessions-api-openapi.yml, openapi/tamara-merchant-api-keys-api-openapi.yml,\n  openapi/tamara-merchant-onboarding-api-openapi.yml, openapi/tamara-refunds-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 6\n    connected: 3\n  by_consequence:\n    physical: 4\n    write: 2\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /payments/capture\n  method: post\n  operationId: captureOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel-partners/webhooks/register\n  method: post\n  operationId: registerChannelPartnerWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel-partners/webhooks\n  method: get\n  operationId: listChannelPartnerWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout\n  method: post\n  operationId: createCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel-partners/merchant/{merchantId}/api-key\n  method: get\n  operationId: retrieveMerchantApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channel-partners/merchant-onboarding/create\n  method: post\n  operationId: createMerchantOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel-partners/merchant-onboarding/{onboardingCode}\n  method: get\n  operationId: retrieveMerchantOnboarding\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/simplified-refund/{order_id}\n  method: post\n  operationId: simplifiedRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/refund\n  method: post\n  operationId: refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/agentic-access/tamara-agentic-access.yml
summary_line: 9 operations · 6 acting
tags:
- Buy Now Pay Later
- Fintech
- Payments
- Checkout
- Shariah Compliant
- MENA
- Saudi Arabia
- United Arab Emirates
- Installments
- Pay Later
- Merchant Services
- Order
- Refunds
- Capture
- Webhook
- Disputes
- Channel Partners
- E-Commerce
- Point-of-Sale
---
