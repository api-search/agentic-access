---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: algbra-account-transaction-api-openapi.yml
  format: yaml
  label: Algbra Account and Transaction Information API (AIS)
  slug: algbra-account-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/openapi/algbra-account-transaction-api-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Algbra Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Algbra exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Algbra
provider_slug: algbra
slug: algbra-agentic-access
source_filename: algbra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/algbra-account-transaction-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 2\n    connected: 6\n  by_consequence:\n    write: 2\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /account-access-consents\n  method: post\n  operationId: CreateAccountAccessConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-access-consents/{ConsentId}\n  method:\
  \ get\n  operationId: GetAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-access-consents/{ConsentId}\n  method: delete\n  operationId: DeleteAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: GetAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}\n  method: get\n  operationId: GetAccountsAccountId\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/balances\n  method: get\n  operationId: GetAccountsAccountIdBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/beneficiaries\n  method: get\n  operationId: GetAccountsAccountIdBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/transactions\n  method: get\n  operationId: GetAccountsAccountIdTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/agentic-access/algbra-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Fintech
- Ethical Finance
- Banking as a Service
---
