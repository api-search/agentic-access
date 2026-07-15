---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 13
api_specs:
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Accounts API
  slug: pismo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Customers API
  slug: pismo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Cards API
  slug: pismo-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Authorizations API
  slug: pismo-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Transactions and Statements API
  slug: pismo-transactions-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Programs API
  slug: pismo-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
- filename: pismo-openapi.yml
  format: yaml
  label: Pismo Events API
  slug: pismo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/openapi/pismo-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pismo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /accounts/v1/accounts/{accountId}/entity
operation_count: 22
overview: 'Pismo exposes 22 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pismo
provider_slug: pismo
slug: pismo-agentic-access
source_filename: pismo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pismo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 9\n    connected: 13\n  by_consequence:\n    write: 8\n    read: 13\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/v1/accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/v1/accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/v1/accounts/{accountId}\n  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/v1/accounts/{accountId}/status\n  method: patch\n  operationId: updateAccountStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/v1/accounts/{accountId}/entity\n  method: patch\n  operationId: transferAccountOwnership\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/v1/account-balances\n  method: get\n  operationId: getAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1/customers/{customerId}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/v2/cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/v1/cards/{cardId}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/v1/customers/{customerId}/accounts/{accountId}/cards\n  method: get\n  operationId: listCardsForCustomerAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/v1/accounts/{accountId}/authorizations\n\
  \  method: get\n  operationId: listAccountAuthorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/v1/accounts/{accountId}/authorizations/{authorizationId}\n  method: get\n  operationId: getAccountAuthorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/v1/simulate-authorizations\n  method: post\n  operationId: simulateAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/v1/transactions/{transactionId}\n  method: get\n  operationId: getTransactionById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements/v1/accounts/{accountId}/next\n  method: get\n  operationId: getCurrentStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements/v1/accounts/{accountId}/statements/{statementId}\n  method: get\n  operationId: getStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/v2/accounts/{accountId}/statements/{statementId}/transactions\n  method: get\n  operationId: getStatementTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/v1/programs\n  method: post\n  operationId: createProgram\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /programs/v1/programs/{programId}\n  method: get\n  operationId: getProgram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pismo/refs/heads/main/agentic-access/pismo-agentic-access.yml
summary_line: 22 operations · 9 acting
tags:
- Banking
- Card Issuing
- Payments
- Fintech
- Core Banking
- Cloud Native
---
