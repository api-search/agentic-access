---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 32
api_specs:
- filename: commonwealth-bank-accounts-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Accounts API API
  slug: commonwealth-bank-accounts-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-accounts-api-api-openapi.yml
- filename: commonwealth-bank-balances-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Balances API API
  slug: commonwealth-bank-balances-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-balances-api-api-openapi.yml
- filename: commonwealth-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Balances API
  slug: commonwealth-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-balances-api-openapi.yml
- filename: commonwealth-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Direct Debits API
  slug: commonwealth-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-direct-debits-api-openapi.yml
- filename: commonwealth-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Scheduled Payments API
  slug: commonwealth-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: commonwealth-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Account Transactions API
  slug: commonwealth-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-account-transactions-api-openapi.yml
- filename: commonwealth-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Accounts API
  slug: commonwealth-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-accounts-api-openapi.yml
- filename: commonwealth-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Payees API
  slug: commonwealth-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-payees-api-openapi.yml
- filename: commonwealth-bank-banking-products-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Banking Products API
  slug: commonwealth-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-banking-products-api-openapi.yml
- filename: commonwealth-bank-customer-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Customer API API
  slug: commonwealth-bank-customer-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-customer-api-api-openapi.yml
- filename: commonwealth-bank-payees-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Payees API API
  slug: commonwealth-bank-payees-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-payees-api-api-openapi.yml
- filename: commonwealth-bank-products-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Products API API
  slug: commonwealth-bank-products-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-products-api-api-openapi.yml
- filename: commonwealth-bank-regular-payments-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Regular Payments API API
  slug: commonwealth-bank-regular-payments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-regular-payments-api-api-openapi.yml
- filename: commonwealth-bank-transaction-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Transaction API API
  slug: commonwealth-bank-transaction-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-transaction-api-api-openapi.yml
consequence_counts:
  physical: 3
  read: 32
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Commonwealth Bank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/direct-debits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /banking/payments/scheduled
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/scheduled
operation_count: 38
overview: 'Commonwealth Bank exposes 38 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 3 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Commonwealth Bank
provider_slug: commonwealth-bank
slug: commonwealth-bank-agentic-access
source_filename: commonwealth-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/commonwealth-bank-cdr-accounts-openapi.json, openapi/commonwealth-bank-cdr-balances-openapi.json,\n  openapi/commonwealth-bank-cdr-customer-openapi.json, openapi/commonwealth-bank-cdr-payees-openapi.json,\n  openapi/commonwealth-bank-cdr-products-openapi.json, openapi/commonwealth-bank-cdr-regular-payments-openapi.json,\n  openapi/commonwealth-bank-cdr-transactions-openapi.json, openapi/commonwealth-bank-cds-banking-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 32\n    acting: 6\n  by_consequence:\n    read: 32\n    write: 3\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId:\
  \ listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccountDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/balance\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/balances\n  method: get\n  operationId: listBalancesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/balances\n  method: post\n  operationId: listBalancesSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/customer\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /common/customer/detail\n  method: get\n  operationId: getCustomerDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payees\n  method: get\n  operationId: listPayees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payees/{payeeId}\n  method: get\n  operationId: getPayeeDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productId}\n  method: get\n  operationId: getProductDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/direct-debits\n  method: get\n  operationId: listDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/direct-debits\n  method: get\n  operationId: listDirectDebitsBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/direct-debits\n\
  \  method: post\n  operationId: listDirectDebitsSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/payments/scheduled\n  method: get\n  operationId: listScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/scheduled\n  method: get\n  operationId: listScheduledPaymentsBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/scheduled\n  method: post\n  operationId: listScheduledPaymentsSpecificAccounts\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: getTransactionDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts\n  method: get\n  operationId: listBankingAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /banking/accounts/balances\n  method: get\n  operationId: listBankingBalancesBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/balances\n  method: post\n  operationId: listBankingBalancesSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banking/accounts/{accountId}/balance\n  method: get\n  operationId: getBankingBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}\n  method: get\n  operationId: getBankingAccountDetail\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/transactions\n  method: get\n  operationId: listBankingTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: getBankingTransactionDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/direct-debits\n  method: get\n  operationId: listDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/direct-debits\n  method: get\n  operationId: listDirectDebitsBulk\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/direct-debits\n  method: post\n  operationId: listDirectDebitsSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banking/accounts/{accountId}/payments/scheduled\n  method: get\n  operationId: listScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payments/scheduled\n  method: get\n  operationId: listScheduledPaymentsBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /banking/payments/scheduled\n  method: post\n  operationId: listScheduledPaymentsSpecificAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banking/accounts/{accountId}/payments/plans\n  method: get\n  operationId: listInstalmentPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/payments/plans\n  method: get\n  operationId: listInstalmentPlansBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payees\n  method: get\n  operationId: listBankingPayees\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payees/{payeeId}\n  method: get\n  operationId: getBankingPayeeDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/products\n  method: get\n  operationId: listBankingProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/products/{productId}\n  method: get\n  operationId: getBankingProductDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/agentic-access/commonwealth-bank-agentic-access.yml
summary_line: 38 operations · 6 acting
tags:
- Financial
- Banks
- Consumer Banking
- Business Banking
- Open Banking
- CDR
- Product Reference Data
- ADI
- Australia
---
