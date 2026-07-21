---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 16
api_specs:
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Product Reference Data API
  slug: judo-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Accounts & Balances API
  slug: judo-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Transactions API
  slug: judo-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Direct Debits & Scheduled Payments API
  slug: judo-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
- filename: judo-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Judo Bank CDR Payees API
  slug: judo-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/openapi/judo-bank-cds-banking-products-openapi.yml
consequence_counts:
  physical: 1
  read: 16
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Judo Bank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /banking/payments/scheduled
operation_count: 19
overview: 'Judo Bank exposes 19 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Judo Bank
provider_slug: judo-bank
slug: judo-bank-agentic-access
source_filename: judo-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/judo-bank-cds-banking-products-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 16\n    acting: 3\n  by_consequence:\n    read: 16\n    write: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /banking/accounts\n  method: get\n  operationId: listBankingAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/balances\n  method: get\n  operationId: listBankingBalancesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /banking/accounts/balances\n  method: post\n  operationId: listBankingBalancesSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banking/accounts/{accountId}/balance\n  method: get\n  operationId: getBankingBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}\n  method: get\n  operationId: getBankingAccountDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/transactions\n  method: get\n  operationId: listBankingTransactions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: getBankingTransactionDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/direct-debits\n  method: get\n  operationId: listDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/direct-debits\n  method: get\n  operationId: listDirectDebitsBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/direct-debits\n  method: post\n  operationId: listDirectDebitsSpecificAccounts\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banking/accounts/{accountId}/payments/scheduled\n  method: get\n  operationId: listScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payments/scheduled\n  method: get\n  operationId: listScheduledPaymentsBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payments/scheduled\n  method: post\n  operationId: listScheduledPaymentsSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banking/accounts/{accountId}/payments/plans\n  method: get\n  operationId: listInstalmentPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/payments/plans\n  method: get\n  operationId: listInstalmentPlansBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payees\n  method: get\n  operationId: listBankingPayees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payees/{payeeId}\n  method: get\n  operationId: getBankingPayeeDetail\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/products\n  method: get\n  operationId: listBankingProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/products/{productId}\n  method: get\n  operationId: getBankingProductDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judo-bank/refs/heads/main/agentic-access/judo-bank-agentic-access.yml
summary_line: 19 operations · 3 acting
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- SME Lending
- Product Reference Data
---
