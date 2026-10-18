---
acting_count: 20
action_class_counts:
  acting: 20
api_specs:
- filename: riskified-automation-endpoints-api-openapi.yml
  format: yaml
  label: Riskified Automation Endpoints API
  slug: riskified-automation-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-automation-endpoints-api-openapi.yml
- filename: riskified-customer-actions-api-openapi.yml
  format: yaml
  label: Riskified Customer Actions API
  slug: riskified-customer-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-customer-actions-api-openapi.yml
- filename: riskified-customer-management-api-openapi.yml
  format: yaml
  label: Riskified Customer Management API
  slug: riskified-customer-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-customer-management-api-openapi.yml
- filename: riskified-order-pre-auth-review-and-psd2-3ds-cvv-recommendations-api-openapi.yml
  format: yaml
  label: Riskified Order Pre-Auth Review and PSD2/3DS/CVV Recommendations API
  slug: riskified-order-pre-auth-review-and-psd2-3ds-cvv-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-order-pre-auth-review-and-psd2-3ds-cvv-recommendations-api-openapi.yml
- filename: riskified-otp-recover-sync-flow-api-openapi.yml
  format: yaml
  label: Riskified OTP Recover (Sync flow) API
  slug: riskified-otp-recover-sync-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-otp-recover-sync-flow-api-openapi.yml
- filename: riskified-post-authorization-flow-api-openapi.yml
  format: yaml
  label: Riskified Post-Authorization Flow API
  slug: riskified-post-authorization-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-post-authorization-flow-api-openapi.yml
- filename: riskified-pre-authorization-flow-api-openapi.yml
  format: yaml
  label: Riskified Pre-Authorization Flow API
  slug: riskified-pre-authorization-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-pre-authorization-flow-api-openapi.yml
- filename: riskified-refunds-api-openapi.yml
  format: yaml
  label: Riskified Refunds API
  slug: riskified-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-refunds-api-openapi.yml
- filename: riskified-returns-api-openapi.yml
  format: yaml
  label: Riskified Returns API
  slug: riskified-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/openapi/riskified-returns-api-openapi.yml
consequence_counts:
  physical: 11
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Riskified Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reset_password
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/advise
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargeback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkout_denied
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkout_denied
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/decide
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/decide
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/fulfill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /claim_create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /claim_decision
operation_count: 20
overview: 'Riskified exposes 20 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 write, 11 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Riskified
provider_slug: riskified
slug: riskified-agentic-access
source_filename: riskified-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/riskified-account-secure-openapi.yml, openapi/riskified-chargeback-guarantee-openapi.yml,\n  openapi/riskified-chargeback-guarantee-post-auth-openapi.yml, openapi/riskified-otp-recovery-openapi.yml,\n  openapi/riskified-policy-protect-refunds-returns-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 20\n  by_consequence:\n    write: 8\n    safety-critical: 1\n    physical: 11\n  human_in_the_loop_required: 1\noperations:\n- path: /customer_create\n  method: post\n  operationId: customer_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer_update\n  method: post\n  operationId: customer_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reset_password\n  method: post\n  operationId: reset_password\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/advise\n  method: post\n  operationId: advise\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkout_denied\n  method: post\n  operationId: checkout_denied\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/decide\n  method: post\n  operationId: decide\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision\n  method: post\n  operationId: decision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cancel\n  method: post\n  operationId: cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargeback\n  method: post\n  operationId: chargeback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkout_denied\n  method: post\n  operationId: checkout_denied\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decide\n  method: post\n  operationId: decide\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision\n  method: post\n  operationId: decision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fulfill\n  method: post\n  operationId: fulfill\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/refund\n  method: post\n  operationId: refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/submit\n  method: post\n  operationId: submit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /initiate\n  method: post\n  operationId: initiateOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim_create\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim_decision\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim_update\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riskified/refs/heads/main/agentic-access/riskified-agentic-access.yml
summary_line: 20 operations · 20 acting · 1 human-in-the-loop
tags:
- Fraud Prevention
- Chargebacks
- E-Commerce
- Payments
- Risk Management
- Machine Learning
- Account Takeover
- Policy Abuse
- 3D
- PSD2
- Returns
---
