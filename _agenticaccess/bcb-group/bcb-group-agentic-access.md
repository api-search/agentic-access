---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 12
api_specs:
- filename: bcb-group-payments-openapi.json
  format: json
  label: BCB Group Payments API
  slug: bcb-group-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bcb-group/refs/heads/main/openapi/bcb-group-payments-openapi.json
consequence_counts:
  physical: 6
  read: 12
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bcb Group Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{accountId}/virtual/{iban}/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/{accountId}/verification-of-payee/{end2endId}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/{accountId}/verification-of-payee/{end2endId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payments/register-webhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payments/reverse-deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v5/payments/authorise
operation_count: 24
overview: 'BCB Group exposes 24 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 6 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BCB Group
provider_slug: bcb-group
slug: bcb-group-agentic-access
source_filename: bcb-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/bcb-group-payments-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 12\n    acting: 12\n  by_consequence:\n    read: 12\n    physical: 6\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v4/accounts/balance/{accountId}\n  method: get\n  operationId: Accounts_BalanceV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts\n  method: get\n  operationId: Accounts_ListAccountsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v3/accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: Accounts_TransactionDetailV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/{accountId}/transactions\n  method: get\n  operationId: Accounts_TransactionsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/{accountId}/verification-of-payee/{end2endId}/approve\n  method: post\n  operationId: Payments_VerificationOfPayeeApproveV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/bank-lookup\n  method: get\n  operationId: Tools_BankLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/accounts\n  method: post\n  operationId: Beneficiaries_CreateBeneficiaryV4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/beneficiaries\n  method: get\n  operationId: Beneficiaries_ListBeneficiariesV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/{accountId}/blinc-beneficiaries\n  method: get\n  operationId: Accounts_BlincBeneficiariesV3\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/blinc-accounts/{blincId}\n  method: get\n  operationId: Accounts_BlincAccountV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/{accountId}/verification-of-payee/{end2endId}/cancel\n  method: post\n  operationId: Payments_VerificationOfPayeeCancelV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/oauth/token\n  method: post\n  operationId: Auth_GetTokenV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/payments/register-webhook\n  method: post\n  operationId: Notifications_PaymentsStatusWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/payments/authorise\n  method: post\n  operationId: Payments_AuthorisePaymentV5\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/payments/{accountId}/transaction/{transactionId}\n  method: get\n  operationId: Payments_PaymentByIdV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/{accountId}/nonce/{nonce}\n  method: get\n  operationId: Payments_getPaymentByNonceV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/{accountId}\n  method: get\n  operationId: Payments_ListPaymentsForAccountV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/payments/reverse-deposit\n  method: post\n  operationId: Payments_ReverseDepositV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{accountId}/virtual/all-account-data\n  method: get\n  operationId: VirtualAccounts_ListAccountsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountId}/virtual/{iban}/payment\n  method: post\n  operationId: VirtualAccounts_AuthorisePaymentV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{accountId}/virtual/{iban}/close\n\
  \  method: post\n  operationId: VirtualAccounts_CloseVirtualAccountV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountId}/virtual\n  method: post\n  operationId: VirtualAccounts_CreateVirtualAccountV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{accountId}/virtual/{iban}/owner-address\n  method: put\n  operationId: VirtualAccounts_UpdateOwnerAddressV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{accountId}/virtual/{iban}/owner-bank-details\n  method: put\n  operationId: VirtualAccounts_UpdateOwnerBankDetailsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bcb-group/refs/heads/main/agentic-access/bcb-group-agentic-access.yml
summary_line: 24 operations · 12 acting
tags:
- Company
- Crypto
- Payments
- Banking
- Digital Assets
- Stablecoins
- Financial Services
- Fintech
---
