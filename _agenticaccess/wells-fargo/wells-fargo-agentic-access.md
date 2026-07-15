---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: wells-fargo-gateway-api-openapi.yml
  format: yaml
  label: Wells Fargo Gateway API
  slug: gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/openapi/wells-fargo-gateway-api-openapi.yml
- filename: wells-fargo-account-transactions-api-openapi.yml
  format: yaml
  label: Wells Fargo Account Transactions API
  slug: account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/openapi/wells-fargo-account-transactions-api-openapi.yml
- filename: wells-fargo-ach-payments-api-openapi.yml
  format: yaml
  label: Wells Fargo ACH Payments API
  slug: ach-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/openapi/wells-fargo-ach-payments-api-openapi.yml
consequence_counts:
  physical: 4
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wells Fargo Agentic Access
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
  method: POST
  path: /v2/ach/batches
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/ach/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/ach/payments/{paymentId}
operation_count: 14
overview: 'wells-fargo exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: wells-fargo
provider_slug: wells-fargo
slug: wells-fargo-agentic-access
source_filename: wells-fargo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wells-fargo-account-transactions-api-openapi.yml, openapi/wells-fargo-ach-payments-api-openapi.yml,\n  openapi/wells-fargo-gateway-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 10\n    acting: 4\n  by_consequence:\n    read: 10\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/accounts/{accountId}/transactions\n  method: get\n  operationId: listAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/{accountId}/transactions/{transactionId}\n\
  \  method: get\n  operationId: getTransactionDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/{accountId}/balances\n  method: get\n  operationId: getAccountBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ach/payments\n  method: post\n  operationId: initiateAchPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments:write\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ach/payments\n  method: get\n  operationId: listAchPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ach/payments/{paymentId}\n  method: get\n  operationId: getAchPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ach/payments/{paymentId}\n  method: delete\n  operationId: cancelAchPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n \
  \     purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ach/batches\n  method: post\n  operationId: submitAchBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ach/returns\n  method: get\n  operationId: listAchReturns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/agentic-access/wells-fargo-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Fortune 100
---
