---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 20
api_specs:
- filename: rye-checkout-intents-openapi-original.yml
  format: yaml
  label: Universal Checkout API
  slug: universal-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-checkout-intents-openapi-original.yml
consequence_counts:
  physical: 10
  read: 20
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rye Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/betas/checkout-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/billing/drawdown/topup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/billing/drawdown/topup/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/checkout-intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/checkout-intents/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/checkout-intents/{id}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/orders/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payment-gateways/{gateway}/session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/test-helpers/checkout-intents/{checkoutIntentId}/shipments/advance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/test-helpers/returns/{returnId}/refund
operation_count: 39
overview: 'Rye exposes 39 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 9 write, and 10 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rye
provider_slug: rye
slug: rye-agentic-access
source_filename: rye-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/rye-checkout-intents-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 20\n    acting: 19\n  by_consequence:\n    read: 20\n    write: 9\n    physical: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/billing/balance\n  method: get\n  operationId: GetBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing\n  method: get\n  operationId: GetSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n \
  \   - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/drawdown\n  method: post\n  operationId: SetupDrawdown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/drawdown/topup\n  method: post\n  operationId: CreateTopUpInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/drawdown/topup/{invoiceId}\n  method: delete\n  operationId:\
  \ CancelTopUpInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/transactions\n  method: get\n  operationId: ListTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/brands/domain/{domain}\n  method: get\n  operationId: GetBrandByDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/checkout-intents\n  method: get\n  operationId: ListCheckoutIntents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/checkout-intents\n  method: post\n  operationId: CreateCheckoutIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout_intents:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/checkout-intents/{id}\n  method: get\n  operationId: GetCheckoutIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/checkout-intents/{id}/order\n  method: get\n  operationId: GetCheckoutIntentOrder\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/checkout-intents/{id}/confirm\n  method: post\n  operationId: ConfirmCheckoutIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout_intents:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/checkout-intents/{id}/shipments\n  method: get\n  operationId: GetShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/checkout-intents/purchase\n  method: post\n\
  \  operationId: Purchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout_intents:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/betas/checkout-sessions\n  method: post\n  operationId: Create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout_intents:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/commissions/{id}\n  method: get\n  operationId: GetCommission\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commissions\n  method: get\n  operationId: ListCommissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events\n  method: get\n  operationId: List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - events:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events/{id}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - events:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events/trigger\n  method: post\n  operationId: Trigger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - events:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/merchant-connectors/{connector}/installation-link\n  method: get\n  operationId: CreateInstallationLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orders\n  method: get\n  operationId: ListOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orders/{id}\n  method: get\n  operationId: GetOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/orders/{id}/cancel\n  method: post\n  operationId: CancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout_intents:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payment-gateways/{gateway}/session\n  method: post\n  operationId: CreateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - checkout_intents:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/products/lookup\n \
  \ method: get\n  operationId: Lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products/subscriptions\n  method: get\n  operationId: ListSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products/subscribe\n  method: post\n  operationId: Subscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/products/unsubscribe\n  method: post\n  operationId: Unsubscribe\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - products:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/returns\n  method: post\n  operationId: RequestReturn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - checkout_intents:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/returns/{returnId}\n  method: get\n  operationId: GetReturn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/shipments\n  method: get\n  operationId: ListShipments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/shipments/{id}\n  method: get\n  operationId: GetShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - checkout_intents:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/test-helpers/checkout-intents/{checkoutIntentId}/shipments/advance\n  method: post\n  operationId: AdvanceShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - test_helpers:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/test-helpers/returns\n  method: post\n  operationId:\
  \ CreateSimulatedReturn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - test_helpers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/test-helpers/returns/{returnId}/approve\n  method: post\n  operationId: ApproveReturn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - test_helpers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/test-helpers/returns/{returnId}/deny\n  method: post\n  operationId: DenyReturn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - test_helpers:write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/test-helpers/returns/{returnId}/refund\n  method: post\n  operationId: RefundReturn\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - test_helpers:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/test-helpers/returns/{returnId}/fail\n  method: post\n  operationId: FailReturn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - test_helpers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/agentic-access/rye-agentic-access.yml
summary_line: 39 operations · 19 acting
tags:
- Company
- Commerce
- E-Commerce
- Checkout
- Payments
- Agentic Commerce
- AI Agents
- Universal Checkout
- Shopping
---
