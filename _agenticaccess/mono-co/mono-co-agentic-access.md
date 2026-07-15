---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: mono-co-openapi.yml
  format: yaml
  label: Account Linking and Auth
  slug: account-linking-auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Account Information
  slug: account-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Transactions and Statements
  slug: transactions-statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Identity and Income
  slug: identity-income
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: DirectPay Payments
  slug: directpay-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Direct Debit and Mandates
  slug: direct-debit-mandates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
- filename: mono-co-openapi.yml
  format: yaml
  label: Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/openapi/mono-co-openapi.yml
consequence_counts:
  physical: 3
  read: 9
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mono Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payments/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payments/initiate-mandate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payments/mandates/{id}/debit
operation_count: 16
overview: 'Mono exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 4 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mono
provider_slug: mono-co
slug: mono-co-agentic-access
source_filename: mono-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mono-co-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 7\n    connected: 9\n  by_consequence:\n    write: 4\n    read: 9\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/accounts/initiate\n  method: post\n  operationId: initiateAccountLinking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/auth\n  method: post\n  operationId: exchangeToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{id}\n  method: get\n  operationId: getAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/balance\n  method: get\n  operationId: getAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/transactions\n  method: get\n  operationId: getAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/statement\n  method: get\n\
  \  operationId: getAccountStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/identity\n  method: get\n  operationId: getAccountIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/income\n  method: get\n  operationId: getAccountIncome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/unlink\n  method: post\n  operationId: unlinkAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/payments/initiate\n  method: post\n  operationId: initiatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/payments/verify/{reference}\n  method: get\n  operationId: verifyPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers\n\
  \  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/payments/initiate-mandate\n  method: post\n  operationId: initiateMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/payments/mandates/{id}/balance\n  method: get\n  operationId: mandateBalanceInquiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/payments/mandates/{id}/debit\n  method: post\n  operationId: debitMandate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mono-co/refs/heads/main/agentic-access/mono-co-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- Open Banking
- Financial Data
- Payments
- Direct Debit
- Africa
---
