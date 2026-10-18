---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 5
api_specs:
- filename: billie-authentication-api-openapi.yml
  format: yaml
  label: Billie Authentication API
  slug: billie-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billie/refs/heads/main/openapi/billie-authentication-api-openapi.yml
- filename: billie-back-end-order-creation-api-openapi.yml
  format: yaml
  label: Billie Back-end Order Creation API
  slug: billie-back-end-order-creation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billie/refs/heads/main/openapi/billie-back-end-order-creation-api-openapi.yml
- filename: billie-captures-api-openapi.yml
  format: yaml
  label: Billie Captures API
  slug: billie-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billie/refs/heads/main/openapi/billie-captures-api-openapi.yml
- filename: billie-front-end-order-creation-api-openapi.yml
  format: yaml
  label: Billie Front-end Order Creation API
  slug: billie-front-end-order-creation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billie/refs/heads/main/openapi/billie-front-end-order-creation-api-openapi.yml
- filename: billie-order-management-api-openapi.yml
  format: yaml
  label: Billie Order Management API
  slug: billie-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billie/refs/heads/main/openapi/billie-order-management-api-openapi.yml
consequence_counts:
  physical: 11
  read: 5
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Billie Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/token/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /checkout-sessions/{sessionId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hpp-checkout-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /invoices/{captureId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{captureId}/confirm-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{captureId}/credit-notes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{captureId}/update-details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{id}/cancel
operation_count: 18
overview: 'Billie exposes 18 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 1 write, 11 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Billie
provider_slug: billie
slug: billie-agentic-access
source_filename: billie-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/billie-direct-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 13\n    connected: 5\n  by_consequence:\n    physical: 11\n    read: 5\n    write: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /checkout-sessions\n  method: post\n  operationId: create_checkout_session_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /checkout-sessions/{sessionId}/authorization\n  method: get\n  operationId: get_checkout_session_authorization_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout-sessions/{sessionId}/confirm\n  method: put\n  operationId: confirm_authorization_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hpp-checkout-sessions\n  method: post\n  operationId: create_hpp_checkout_session_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices\n  method: post\n  operationId: invoice_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{captureId}\n  method: get\n  operationId: get_invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{captureId}\n  method: delete\n  operationId: invoice_cancel_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{captureId}/confirm-payment\n  method: post\n  operationId: invoice_payment_confirm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{captureId}/credit-notes\n  method: post\n  operationId: create_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /invoices/{captureId}/update-details\n  method: post\n  operationId: invoice_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal-forms\n  method: get\n  operationId: get_legal_forms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/authorization\n  method: get\n  operationId: oauth_token_validate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: oauth_token_create\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token/revoke\n  method: post\n  operationId: oauth_token_revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /orders\n  method: post\n  operationId: order_create_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /orders/{id}\n  method: get\n  operationId: order_get_details_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: post\n  operationId: order_update_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}/cancel\n  method: post\n  operationId: order_cancel_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billie/refs/heads/main/agentic-access/billie-agentic-access.yml
summary_line: 18 operations · 13 acting · 1 human-in-the-loop
tags:
- Company
- Fintech
- Payments
- Buy Now Pay Later
- B2B
- Invoicing
- Checkout
- Germany
---
