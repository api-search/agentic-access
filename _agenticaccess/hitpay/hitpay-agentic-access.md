---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 4
api_specs:
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Payment Requests API
  slug: hitpay-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Recurring Billing API
  slug: hitpay-recurring-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Subscription Plans API
  slug: hitpay-subscription-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Refunds API
  slug: hitpay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
- filename: hitpay-openapi.yml
  format: yaml
  label: HitPay Platform API
  slug: hitpay-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/openapi/hitpay-openapi.yml
consequence_counts:
  read: 4
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Payment mutations are money-movement operations; treat writes as high-value and require human-in-the-loop by default. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Hitpay Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'HitPay exposes 12 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 8 write.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HitPay
provider_slug: hitpay
slug: hitpay-agentic-access
source_filename: hitpay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/hitpay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind\n  audience per deployment. Payment mutations are money-movement operations; treat writes as\n  high-value and require human-in-the-loop by default. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 8\n    connected: 4\n  by_consequence:\n    write: 8\n    read: 4\n  human_in_the_loop_required: 8\noperations:\n- path: /payment-requests\n  method: post\n  operationId: createPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - abnormal\n\
  \    audit: required\n- path: /payment-requests\n  method: get\n  operationId: listPaymentRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-requests/{id}\n  method: get\n  operationId: getPaymentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-requests/{id}\n  method: delete\n  operationId: deletePaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - abnormal\n    audit: required\n- path: /refund\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - irreversible\n    audit: required\n- path: /recurring-billing\n  method: post\n  operationId: createRecurringBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - recurring-commitment\n      - high-value\n    audit: required\n- path: /recurring-billing/{id}\n  method: get\n  operationId: getRecurringBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring-billing/{id}\n  method: delete\n  operationId: cancelRecurringBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - abnormal\n    audit: required\n- path: /charge/{recurring_billing_id}\n  method: post\n  operationId: chargeRecurringBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /subscription-plan\n  method: get\n  operationId: listSubscriptionPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription-plan\n  method: post\n  operationId: createSubscriptionPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription-plan/{id}\n  method: delete\n  operationId: deleteSubscriptionPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hitpay/refs/heads/main/agentic-access/hitpay-agentic-access.yml
summary_line: 12 operations · 8 acting · 8 human-in-the-loop
tags:
- Payments
- Fintech
- PayNow
- Southeast Asia
- SMB
---
