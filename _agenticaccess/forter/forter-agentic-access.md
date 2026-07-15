---
acting_count: 8
action_class_counts:
  acting: 8
api_specs:
- filename: forter-openapi.yml
  format: yaml
  label: Forter Order Decision API
  slug: forter-order-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
- filename: forter-openapi.yml
  format: yaml
  label: Forter Account Protection API
  slug: forter-account-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
- filename: forter-openapi.yml
  format: yaml
  label: Forter Chargeback and Compensation API
  slug: forter-chargeback-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
- filename: forter-openapi.yml
  format: yaml
  label: Forter Data Privacy API
  slug: forter-data-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
consequence_counts:
  physical: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Forter Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/dispute/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/status/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders/{orderId}
operation_count: 8
overview: 'Forter exposes 8 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Forter
provider_slug: forter
slug: forter-agentic-access
source_filename: forter-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/forter-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 8\n  by_consequence:\n    physical: 4\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/orders/{orderId}\n  method: post\n  operationId: submitOrderV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{orderId}\n  method: post\n  operationId: submitOrderV3\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/status/{orderId}\n  method: post\n  operationId: submitOrderStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/signup/{accountId}\n  method: post\n  operationId: submitSignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/authentication-result/{loginId}\n  method: post\n  operationId: submitAuthenticationResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/unified/compensation/request/{id}\n  method: post\n  operationId: submitCompensationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/dispute/{id}\n  method: post\n  operationId: submitDispute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/profile-access/{id}\n  method: post\n  operationId: submitProfileAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/agentic-access/forter-agentic-access.yml
summary_line: 8 operations · 8 acting
tags:
- Fraud Detection
- Fraud Prevention
- Identity
- Trust
- Payments
- Chargebacks
- Account Protection
- E-commerce
- Risk
- Machine Learning
---
