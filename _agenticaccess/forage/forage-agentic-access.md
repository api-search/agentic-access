---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 16
api_specs:
- filename: forage-payments-api-openapi.yml
  format: yaml
  label: Forage EBT SNAP Payments API
  slug: forage-ebt-snap-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-payments-api-openapi.yml
- filename: forage-bearer-tokens-api-openapi.yml
  format: yaml
  label: Forage Bearer Tokens API
  slug: forage-bearer-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-bearer-tokens-api-openapi.yml
- filename: forage-card-details-api-openapi.yml
  format: yaml
  label: Forage Card Details API
  slug: forage-card-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-card-details-api-openapi.yml
- filename: forage-custom-sessions-api-openapi.yml
  format: yaml
  label: Forage Custom Sessions API
  slug: forage-custom-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-custom-sessions-api-openapi.yml
- filename: forage-deferred-capture-api-openapi.yml
  format: yaml
  label: Forage Deferred Capture API
  slug: forage-deferred-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-deferred-capture-api-openapi.yml
- filename: forage-fully-hosted-sessions-api-openapi.yml
  format: yaml
  label: Forage Fully Hosted Sessions API
  slug: forage-fully-hosted-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-fully-hosted-sessions-api-openapi.yml
- filename: forage-order-payments-api-openapi.yml
  format: yaml
  label: Forage Order Payments API
  slug: forage-order-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-order-payments-api-openapi.yml
- filename: forage-order-refunds-api-openapi.yml
  format: yaml
  label: Forage Order Refunds API
  slug: forage-order-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-order-refunds-api-openapi.yml
- filename: forage-orders-api-openapi.yml
  format: yaml
  label: Forage Orders API
  slug: forage-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-orders-api-openapi.yml
- filename: forage-payment-methods-api-openapi.yml
  format: yaml
  label: Forage Payment Methods API
  slug: forage-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-payment-methods-api-openapi.yml
- filename: forage-payment-refunds-api-openapi.yml
  format: yaml
  label: Forage Payment Refunds API
  slug: forage-payment-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-payment-refunds-api-openapi.yml
- filename: forage-reports-api-openapi.yml
  format: yaml
  label: Forage Reports API
  slug: forage-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-reports-api-openapi.yml
- filename: forage-sandbox-testing-api-openapi.yml
  format: yaml
  label: Forage Sandbox Testing API
  slug: forage-sandbox-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-sandbox-testing-api-openapi.yml
consequence_counts:
  physical: 21
  read: 16
  safety-critical: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Forage Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /o/bulk_revoke/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /o/revoke_token/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/capture_sessions/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/orders/{order_ref}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_ref}/cancel/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/orders/{order_ref}/payments/{payment_ref}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_ref}/payments/{payment_ref}/cancel/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_ref}/refund_all/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_ref}/refund_by_product/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_ref}/refunds/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment_methods/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/payment_methods/{payment_method_ref}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/payment_methods/{payment_method_ref}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/payments/{payment_ref}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{payment_ref}/authorize/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{payment_ref}/cancel/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{payment_ref}/capture-sync/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{payment_ref}/capture_payment/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{payment_ref}/collect_pin_backend/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{payment_ref}/refunds/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{payment_ref}/refunds/{refund_ref}/void/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{payment_ref}/void/
operation_count: 43
overview: 'Forage exposes 43 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 4 write, 21 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Forage
provider_slug: forage
slug: forage-agentic-access
source_filename: forage-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/forage-payments-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    acting: 27\n    connected: 16\n  by_consequence:\n    write: 4\n    read: 16\n    physical: 21\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /api/balance_sessions/\n  method: post\n  operationId: Create balance session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/balance_sessions/{session_ref}/\n\
  \  method: get\n  operationId: View balance session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - internal\n    - pinpad_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/capture_sessions/\n  method: post\n  operationId: Create capture session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_ref}/\n  method: get\n  operationId: Get order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_ref}/\n\
  \  method: patch\n  operationId: Update order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_ref}/cancel/\n  method: post\n  operationId: Cancel order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_ref}/payments/\n  method: get\n  operationId: Get all payments\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_ref}/payments/{payment_ref}/\n  method: get\n  operationId: Get a payment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_ref}/payments/{payment_ref}/\n  method: patch\n  operationId: PATCH Update an order payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/orders/{order_ref}/payments/{payment_ref}/cancel/\n  method: post\n  operationId: Cancel a payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_ref}/refund_all/\n  method: post\n  operationId: Refund order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_ref}/refund_by_product/\n\
  \  method: post\n  operationId: Create refunds by product\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_ref}/refunds/\n  method: post\n  operationId: Create a refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_ref}/refunds/\n  method:\
  \ get\n  operationId: Get all order refunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_ref}/refunds/{refund_ref}/\n  method: get\n  operationId: Get an order refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payment_methods/\n  method: post\n  operationId: Create payment method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/payment_methods/{payment_method_ref}/\n  method: get\n  operationId: Get payment method\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payment_methods/{payment_method_ref}/\n  method: patch\n  operationId: Update a payment method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payment_methods/{payment_method_ref}/\n  method: delete\n  operationId: Delete payment method\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/\n  method: post\n  operationId: Create a payment (custom checkout)\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/\n  method: get\n  operationId: Get payment details by merchant id.\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - pinpad_only\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments/{payment_ref}/\n  method: get\n  operationId: Get payment details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - internal\n    - pinpad_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments/{payment_ref}/\n  method: patch\n  operationId: Update a payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{payment_ref}/authorize/\n  method: post\n  operationId: Authorize a payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{payment_ref}/cancel/\n  method: post\n  operationId: Cancel a payment (custom checkout)\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{payment_ref}/capture-sync/\n  method: post\n  operationId: Capture a Payment during sandbox testing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n\
  \    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{payment_ref}/capture_payment/\n  method: post\n  operationId: Capture a payment - deferred capture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{payment_ref}/collect_pin_backend/\n  method: post\n  operationId: Submit PIN during sandbox testing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n\
  \    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{payment_ref}/refunds/\n  method: post\n  operationId: Create a refund (custom checkout)\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{payment_ref}/refunds/\n  method: get\n  operationId: Get all payment refunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - internal\n    - pinpad_only\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments/{payment_ref}/refunds/{refund_ref}/\n  method: get\n  operationId: Get a payment refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - internal\n    - pinpad_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments/{payment_ref}/refunds/{refund_ref}/void/\n  method: post\n  operationId: Void a refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{payment_ref}/void/\n  method: post\n  operationId: Void a payment (custom checkout)\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    scope:\n    - internal\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/session_token/\n  method: post\n  operationId: forage_oauth:forage_session_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sessions/\n  method: post\n  operationId: Create session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - hosted_checkout\n    - pinpad_only\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/state_card_details\n  method: get\n  operationId: Retrieve state card details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - hosted_checkout\n    - internal\n    - pinpad_only\n    - reporting\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /o/bulk_revoke/\n  method: post\n  operationId: forage_oauth:forage_bulk_revoke_token\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /o/revoke_token/\n  method: post\n  operationId: forage_oauth:forage_revoke_token\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /o/token/\n  method: post\n  operationId: forage_oauth:forage_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/orders/\n  method: get\n  operationId: reporting:orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - internal\n    - reporting\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/payouts/\n  method: get\n  operationId: reporting:payouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - internal\n    - reporting\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/payouts/{payout_id}/transactions/\n  method: get\n  operationId: reporting:transactions_by_payout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - internal\n    - reporting\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/transactions/\n  method: get\n  operationId: reporting:transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - internal\n    - reporting\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/agentic-access/forage-agentic-access.yml
summary_line: 43 operations · 27 acting · 2 human-in-the-loop
tags:
- Company
- Payments
- EBT
- SNAP
- EBT Cash
- HSA/FSA
- Fintech
- Government Benefits
- Grocery
- Checkout
- Financial Services
---
