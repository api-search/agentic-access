---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 9
api_specs:
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Charges API
  slug: payjp-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Customers API
  slug: payjp-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Cards API
  slug: payjp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Tokens API
  slug: payjp-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Plans API
  slug: payjp-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Subscriptions API
  slug: payjp-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Transfers API
  slug: payjp-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Statements & Balances API
  slug: payjp-statements-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Events & Webhooks API
  slug: payjp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP 3D Secure API
  slug: payjp-three-d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Platform API (Tenants)
  slug: payjp-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
- filename: payjp-openapi.yml
  format: yaml
  label: PAY.JP Account API
  slug: payjp-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/openapi/payjp-openapi.yml
consequence_counts:
  read: 9
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this payments API to AI agents — review and bind audience per deployment. Because these operations move money in JPY, charge, refund, capture, subscription, and tenant writes are flagged human-in-the-loop required by default. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Payjp Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'PAY.JP exposes 24 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 15 write.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PAY.JP
provider_slug: payjp
slug: payjp-agentic-access
source_filename: payjp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/payjp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this payments API to AI agents — review\n  and bind audience per deployment. Because these operations move money in JPY, charge, refund,\n  capture, subscription, and tenant writes are flagged human-in-the-loop required by default.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 15\n    connected: 9\n  by_consequence:\n    write: 15\n    read: 9\n  human_in_the_loop_required: 6\noperations:\n- path: /charges\n  method: post\n  operationId: createCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n    \
  \  - high-value\n    audit: required\n- path: /charges\n  method: get\n  operationId: listCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charges/{id}/refund\n  method: post\n  operationId: refundCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /charges/{id}/capture\n  method: post\n  operationId: captureCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n    audit: required\n- path: /charges/{id}\n  method: get\n  operationId: retrieveCharge\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - pii\n      - card-data\n    audit: required\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - pii\n    audit: required\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ required\n- path: /customers/{id}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - destructive\n    audit: required\n- path: /customers/{id}/cards\n  method: post\n  operationId: createCustomerCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - card-data\n    audit: required\n- path: /customers/{id}/cards/{card_id}\n  method: delete\n  operationId: deleteCustomerCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - destructive\n    audit: required\n- path: /plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /plans/{id}\n  method: delete\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - destructive\n    audit: required\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - recurring-billing\n \
  \     - money-movement\n    audit: required\n- path: /subscriptions/{id}/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - recurring-billing\n    audit: required\n- path: /subscriptions/{id}/pause\n  method: post\n  operationId: pauseSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - recurring-billing\n    audit: required\n- path: /transfers\n  method: get\n  operationId: listTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /statements\n  method: get\n\
  \  operationId: listStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /balances\n  method: get\n  operationId: listBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /three_d_secure_requests\n  method: post\n  operationId: createThreeDSecureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - card-data\n    audit: required\n- path: /tenants\n  method: post\n  operationId: createTenant\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - onboarding\n      - money-movement\n    audit: required\n- path: /tenants/{id}\n  method: delete\n  operationId: deleteTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - destructive\n    audit: required\n- path: /account\n  method: get\n  operationId: retrieveAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payjp/refs/heads/main/agentic-access/payjp-agentic-access.yml
summary_line: 24 operations · 15 acting · 6 human-in-the-loop
tags:
- Payments
- FinTech
- Japan
- Credit Cards
- Subscriptions
- Tokenization
---
