---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 21
api_specs:
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Tokens API
  slug: culqi-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Charges API
  slug: culqi-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Orders API
  slug: culqi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Refunds API
  slug: culqi-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Customers API
  slug: culqi-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Cards API
  slug: culqi-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Plans API
  slug: culqi-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Subscriptions API
  slug: culqi-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Events & Webhooks API
  slug: culqi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi IIN Lookup API
  slug: culqi-iin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
- filename: culqi-openapi.yml
  format: yaml
  label: Culqi Transfers API
  slug: culqi-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-openapi.yml
consequence_counts:
  read: 21
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this payments API to AI agents - review and bind audience per deployment. Money-movement operations (charges, captures, refunds, order and charge confirmation, subscriptions) are marked human-in-the-loop required. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Culqi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 46
overview: 'Culqi exposes 46 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 25 write.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Culqi
provider_slug: culqi
slug: culqi-agentic-access
source_filename: culqi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/culqi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this payments API to AI agents - review and bind audience per\n  deployment. Money-movement operations (charges, captures, refunds, order and charge confirmation, subscriptions)\n  are marked human-in-the-loop required. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    acting: 25\n    connected: 21\n  by_consequence:\n    write: 25\n    read: 21\n  human_in_the_loop_required: 7\noperations:\n- path: /tokens\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /tokens\n  method: get\n  operationId: listTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/yape\n  method: post\n  operationId: createYapeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/{id}\n  method: get\n  operationId: getToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{id}\n  method: patch\n  operationId: updateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /confirm\n  method: post\n  operationId: confirmCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - abnormal\n    audit: required\n- path: /charges\n  method: post\n  operationId: createCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - abnormal\n    audit: required\n- path: /charges\n  method: get\n  operationId: listCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /charges/{id}\n  method: get\n  operationId: getCharge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charges/{id}\n  method: patch\n  operationId: updateCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charges/{id}/capture\n  method: post\n  operationId: captureCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - abnormal\n    audit: required\n- path: /orders\n  method: post\n\
  \  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - abnormal\n    audit: required\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: patch\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/confirm\n  method: post\n  operationId: confirmOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - abnormal\n    audit: required\n- path: /refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - abnormal\n    audit: required\n- path: /refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds/{id}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds/{id}\n  method: patch\n  operationId: updateRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /customers/{id}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards\n  method: get\n  operationId: listCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}\n  method: patch\n  operationId: updateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{id}\n  method: delete\n  operationId: deleteCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{id}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{id}\n  method: patch\n  operationId: updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{id}\n  method: delete\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - abnormal\n    audit: required\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{id}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{id}\n  method: patch\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{id}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n \
  \ operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iins/{iin}\n  method: get\n  operationId: getIin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers\n  method: get\n  operationId: listTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/{id}\n  method: get\n  operationId: getTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/agentic-access/culqi-agentic-access.yml
summary_line: 46 operations · 25 acting · 7 human-in-the-loop
tags:
- Payments
- Payment Gateway
- FinTech
- Peru
- LatAm
- Cards
- Yape
---
