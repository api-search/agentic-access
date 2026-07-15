---
acting_count: 0
action_class_counts:
  connected: 27
api_specs:
- filename: core-exchange
  format: yaml
  label: FDX Accounts API
  slug: fdx-accounts-api
  spec_type: OpenAPI
  url: https://github.com/plaid/core-exchange
consequence_counts:
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fdx Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Financial Data Exchange (FDX) exposes 27 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Financial Data Exchange (FDX)
provider_slug: fdx
slug: fdx-agentic-access
source_filename: fdx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fdx-corex-6.0.0.yaml, openapi/fdx-corex-6.2.0.yaml, openapi/fdx-corex-6.3.1.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 27\n  by_consequence:\n    read: 27\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: searchForAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Account\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/contact\n  method: get\n  operationId: getAccountContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Customer\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/payment-networks\n  method: get\n  operationId: getAccountPaymentNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions\n  method: get\n  operationId: searchForAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Transactions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/current\n  method: get\n  operationId: getCustomerInfo\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements\n  method: get\n  operationId: searchForAccountStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements/{statementId}\n  method: get\n  operationId: getAccountStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/asset-transfer-networks\n  method: get\n  operationId: getAccountAssetTransferNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: searchForAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    scope:\n    - Account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/contact\n  method: get\n  operationId: getAccountContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Customer\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/payment-networks\n  method: get\n  operationId: getAccountPaymentNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions\n  method: get\n  operationId: searchForAccountTransactions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Transactions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/current\n  method: get\n  operationId: getCustomerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements\n  method: get\n  operationId: searchForAccountStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements/{statementId}\n  method: get\n  operationId: getAccountStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/asset-transfer-networks\n  method: get\n  operationId: getAccountAssetTransferNetworks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: searchForAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/contact\n  method: get\n  operationId: getAccountContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Customer\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/payment-networks\n  method: get\n  operationId: getAccountPaymentNetworks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions\n  method: get\n  operationId: searchForAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Transactions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/current\n  method: get\n  operationId: getCustomerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements\n  method: get\n  operationId: searchForAccountStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements/{statementId}\n  method: get\n  operationId: getAccountStatement\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/asset-transfer-networks\n  method: get\n  operationId: getAccountAssetTransferNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/agentic-access/fdx-agentic-access.yml
summary_line: 27 operations
tags:
- Financial Data
- Open Banking
- Open Finance
- Financial Data Exchange
- Consumer Permissioned
- Account Data
- Transactions
- Investments
- Insurance
- Tax Data
- Payroll
- REST
- OAuth2
- FAPI
- CFPB 1033
---
