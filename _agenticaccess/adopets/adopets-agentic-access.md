---
acting_count: 8
action_class_counts:
  acting: 8
api_specs:
- filename: adopets-external-openapi.yml
  format: yaml
  label: Adopets External API
  slug: adopets-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adopets/refs/heads/main/openapi/adopets-external-openapi.yml
consequence_counts:
  physical: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adopets Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization/external/payment-request/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization/external/payment-request/change
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization/external/payment-request/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization/external/payment-request/get
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization/external/payment-transaction/get
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization/external/payment-transaction/refund
operation_count: 8
overview: 'Adopets exposes 8 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 write and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Adopets
provider_slug: adopets
slug: adopets-agentic-access
source_filename: adopets-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/adopets-external-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 8\n  by_consequence:\n    write: 2\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /organization/external/system-auth/connect\n  method: post\n  operationId: connectExternalSystemUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/external/system-auth/disconnect\n  method: post\n  operationId: disconnectExternalSystemUser\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/external/payment-request/create\n  method: post\n  operationId: createPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/external/payment-request/get\n  method: post\n  operationId: getPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/external/payment-request/cancel\n  method: post\n  operationId: cancelPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/external/payment-request/change\n  method: post\n  operationId: changePaymentRequestItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /organization/external/payment-transaction/get\n  method: post\n  operationId: getPaymentTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/external/payment-transaction/refund\n  method: post\n  operationId: refundPaymentTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adopets/refs/heads/main/agentic-access/adopets-agentic-access.yml
summary_line: 8 operations · 8 acting
tags:
- Pet Adoption
- Animal Welfare
- Shelters and Rescues
- Adoption Management
- Payments
- Nonprofit Technology
- SaaS
- Company
---
