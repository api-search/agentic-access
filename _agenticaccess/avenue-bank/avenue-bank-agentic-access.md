---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Product Reference Data API
  slug: avenue-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Accounts & Balances API
  slug: avenue-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Transactions API
  slug: avenue-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Direct Debits & Scheduled Payments API
  slug: avenue-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
- filename: avenue-bank-cds-banking-openapi.json
  format: json
  label: Avenue Bank CDR Payees API
  slug: avenue-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/openapi/avenue-bank-cds-banking-openapi.json
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts for the Consumer Data Standards Banking API surface. Every operation in this surface is a read (the POST 'For Specific Accounts' operations pass an account-id list in the request body but change no state), so all are classified connected/read. Products (PRD) operations are public/unauthenticated (subject optional); all other families require a consented consumer subject under the CDR ADR model. A governance starting point — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Avenue Bank Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Avenue Bank exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Avenue Bank
provider_slug: avenue-bank
slug: avenue-bank-agentic-access
source_filename: avenue-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/avenue-bank-cds-banking-openapi.json\ndescription: Recommended x-agentic-access execution contracts for the Consumer Data Standards Banking\n  API surface. Every operation in this surface is a read (the POST 'For Specific Accounts' operations\n  pass an account-id list in the request body but change no state), so all are classified connected/read.\n  Products (PRD) operations are public/unauthenticated (subject optional); all other families require\n  a consented consumer subject under the CDR ADR model. A governance starting point — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /banking/accounts\n  method: get\n  operationId: listBankingAccounts\n  summary: Get Accounts\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/balances\n  method: get\n  operationId: listBankingBalancesBulk\n  summary: Get Bulk Balances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/balances\n  method: post\n  operationId: listBankingBalancesSpecificAccounts\n  summary: Get Balances For Specific Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/balance\n  method: get\n  operationId: getBankingBalance\n  summary: Get Account Balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}\n  method: get\n  operationId:\
  \ getBankingAccountDetail\n  summary: Get Account Detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/transactions\n  method: get\n  operationId: listBankingTransactions\n  summary: Get Transactions For Account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: getBankingTransactionDetail\n  summary: Get Transaction Detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/direct-debits\n  method: get\n  operationId: listDirectDebits\n  summary: Get Direct Debits For Account\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/direct-debits\n  method: get\n  operationId: listDirectDebitsBulk\n  summary: Get Bulk Direct Debits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/direct-debits\n  method: post\n  operationId: listDirectDebitsSpecificAccounts\n  summary: Get Direct Debits For Specific Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/payments/scheduled\n  method: get\n  operationId: listScheduledPayments\n  summary: Get Scheduled Payments for Account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payments/scheduled\n\
  \  method: get\n  operationId: listScheduledPaymentsBulk\n  summary: Get Scheduled Payments Bulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payments/scheduled\n  method: post\n  operationId: listScheduledPaymentsSpecificAccounts\n  summary: Get Scheduled Payments For Specific Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/{accountId}/payments/plans\n  method: get\n  operationId: listInstalmentPlans\n  summary: Get Instalment Plans for Account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/accounts/payments/plans\n  method: get\n  operationId: listInstalmentPlansBulk\n  summary: Get Instalment Plans Bulk\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payees\n  method: get\n  operationId: listBankingPayees\n  summary: Get Payees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/payees/{payeeId}\n  method: get\n  operationId: getBankingPayeeDetail\n  summary: Get Payee Detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/products\n  method: get\n  operationId: listBankingProducts\n  summary: Get Products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banking/products/{productId}\n  method: get\n  operationId: getBankingProductDetail\n  summary: Get Product Detail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avenue-bank/refs/heads/main/agentic-access/avenue-bank-agentic-access.yml
summary_line: 19 operations
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Business Banking
- Bank Guarantees
- Australia
- ADI
---
