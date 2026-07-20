---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 4
api_specs:
- filename: getpaid-openapi-original.yml
  format: yaml
  label: Getpaid API v2
  slug: getpaid-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/openapi/getpaid-openapi-original.yml
consequence_counts:
  physical: 5
  read: 4
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Getpaid Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/checkouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/checkouts/query
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payments/query
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payments/{payment_id}/refunds
operation_count: 16
overview: 'GetPaid exposes 16 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 7 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GetPaid
provider_slug: getpaid
slug: getpaid-agentic-access
source_filename: getpaid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/getpaid-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 12\n    connected: 4\n  by_consequence:\n    write: 7\n    physical: 5\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: request_access_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/checkouts\n  method: post\n  operationId: create_checkout\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments:read_write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/checkouts/{checkout_id}\n  method: get\n  operationId: get_checkout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments:read\n    - payments:read_write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/checkouts/query\n  method: post\n  operationId: query_checkouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/payments\n  method: post\n  operationId: create_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments:read_write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/payments/{payment_id}\n  method: get\n  operationId: get_payment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments:read\n    - payments:read_write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/payments/{payment_id}/refunds\n  method: post\n  operationId: refund_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n\
  \    - payments:read_write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/payments/query\n  method: post\n  operationId: query_payments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/query\n  method: post\n  operationId: query_accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/themes\n  method: get\n  operationId: get_account_themes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/applications\n  method: post\n  operationId: create_application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/applications/{application_id}\n  method: get\n  operationId: get_application\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/applications/{application_id}/refresh\n  method: post\n  operationId: refresh_application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/applications/{application_id}/cancel\n  method: post\n  operationId: cancel_application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/applications/query\n  method: post\n  operationId: query_applications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    scope:\n    - accounts:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{resource_type}/query\n  method: post\n  operationId: query_resources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - payments:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getpaid/refs/heads/main/agentic-access/getpaid-agentic-access.yml
summary_line: 16 operations · 12 acting
tags:
- Company
- Payments
- Embedded Payments
- Split Settlement
- Checkout
- Marketplace
- Onboarding
- Subscriptions
- Agent Payments
- Europe
---
