---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: truist-personal-small-business-accounts-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Accounts API
  slug: truist-personal-small-business-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-personal-small-business-accounts-openapi.yml
- filename: truist-personal-small-business-transactions-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Transactions API
  slug: truist-personal-small-business-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-personal-small-business-transactions-openapi.yml
- filename: truist-commercial-accounts-openapi.yml
  format: yaml
  label: Truist Commercial Accounts API
  slug: truist-commercial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-commercial-accounts-openapi.yml
- filename: truist-commercial-account-transactions-openapi.yml
  format: yaml
  label: Truist Commercial Account Transactions API
  slug: truist-commercial-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-commercial-account-transactions-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Truist Financial Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Truist Financial exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Truist Financial
provider_slug: truist-financial
slug: truist-financial-agentic-access
source_filename: truist-financial-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/truist-commercial-account-transactions-openapi.yml, openapi/truist-commercial-accounts-openapi.yml,\n  openapi/truist-personal-small-business-accounts-openapi.yml, openapi/truist-personal-small-business-transactions-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /commercial/accounts/{accountId}/transactions\n  method: get\n  operationId: listCommercialTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - commercial.transactions:read\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /commercial/accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: getCommercialTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - commercial.transactions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/accounts\n  method: get\n  operationId: listCommercialAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - commercial.accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/accounts/{accountId}\n  method: get\n  operationId: getCommercialAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - commercial.accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/accounts/{accountId}/balances\n  method: get\n  operationId: getCommercialAccountBalances\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - commercial.accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/accounts/summary\n  method: get\n  operationId: getCommercialAccountSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - commercial.accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal/accounts\n  method: get\n  operationId: listPersonalAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal/accounts/{accountId}\n  method: get\n  operationId: getPersonalAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /personal/accounts/{accountId}/balances\n  method: get\n  operationId: getPersonalAccountBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal/accounts/{accountId}/transactions\n  method: get\n  operationId: listPersonalTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal/accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: getPersonalTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/agentic-access/truist-financial-agentic-access.yml
summary_line: 11 operations
tags:
- Banking
- Financial Services
- Open Banking
- Commercial Banking
- Personal Banking
- Payments
- Accounts
- Transactions
- Fortune 500
---
