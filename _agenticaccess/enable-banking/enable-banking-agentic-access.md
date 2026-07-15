---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 9
api_specs:
- filename: enable-banking-api-openapi.yml
  format: yaml
  label: Enable Banking API
  slug: enable-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enable-banking/refs/heads/main/openapi/enable-banking-api-openapi.yml
consequence_counts:
  physical: 2
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Enable Banking Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payments/{payment_id}
operation_count: 14
overview: 'Enable Banking exposes 14 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 3 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Enable Banking
provider_slug: enable-banking
slug: enable-banking-agentic-access
source_filename: enable-banking-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/enable-banking-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 5\n    connected: 9\n  by_consequence:\n    write: 3\n    read: 9\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /auth\n  method: post\n  operationId: initialize_session_auth_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: post\n  operationId: authorize_session_sessions_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}\n  method: get\n  operationId: get_session_sessions__session_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}\n  method: delete\n  operationId: delete_session_sessions__session_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/details\n  method: get\n  operationId: get_account_accounts__account_id__details_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/balances\n  method: get\n  operationId: get_account_balances_accounts__account_id__balances_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/transactions\n  method: get\n  operationId: get_account_transactions_accounts__account_id__transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/transactions/{transaction_id}\n  method: get\n  operationId: get_transaction_accounts__account_id__transactions__transaction_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /payments\n  method: post\n  operationId: create_payment_payments_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{payment_id}\n  method: get\n  operationId: get_payment_payments__payment_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{payment_id}\n  method: delete\n  operationId: delete_payment_payments__payment_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{payment_id}/transactions/{transaction_id}\n  method: get\n  operationId: get_payment_transaction_payments__payment_id__transactions__transaction_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aspsps\n  method: get\n  operationId: get_aspsps_aspsps_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /application\n  method: get\n  operationId: get_application_application_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enable-banking/refs/heads/main/agentic-access/enable-banking-agentic-access.yml
summary_line: 14 operations · 5 acting
tags:
- Open Banking
- PSD2
- AISP
- PISP
- Banking
- Financial Services
- Account Aggregation
- Payment Initiation
- Europe
- Nordic
- Finland
- Compliance
- eIDAS
- SCA
- DORA
- GDPR
---
