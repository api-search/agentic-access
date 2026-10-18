---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 16
api_specs:
- filename: trustly-accounts-api-openapi.yml
  format: yaml
  label: Trustly Group Accounts API
  slug: trustly-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-accounts-api-openapi.yml
- filename: trustly-api-api-openapi.yml
  format: yaml
  label: Trustly Group API
  slug: trustly-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-api-api-openapi.yml
- filename: trustly-countries-api-openapi.yml
  format: yaml
  label: Trustly Group Countries API
  slug: trustly-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-countries-api-openapi.yml
- filename: trustly-customers-api-openapi.yml
  format: yaml
  label: Trustly Group Customers API
  slug: trustly-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-customers-api-openapi.yml
- filename: trustly-identity-api-openapi.yml
  format: yaml
  label: Trustly Group Identity API
  slug: trustly-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-identity-api-openapi.yml
- filename: trustly-networkcheckapi-api-openapi.yml
  format: yaml
  label: Trustly Group Network Check API
  slug: trustly-networkcheckapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-networkcheckapi-api-openapi.yml
- filename: trustly-payments-api-openapi.yml
  format: yaml
  label: Trustly Group Payments API
  slug: trustly-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-payments-api-openapi.yml
- filename: trustly-transactions-api-openapi.yml
  format: yaml
  label: Trustly Group Transactions API
  slug: trustly-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-transactions-api-openapi.yml
- filename: trustly-verifycustomer-api-openapi.yml
  format: yaml
  label: Trustly Group Verify Customer API
  slug: trustly-verifycustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-verifycustomer-api-openapi.yml
- filename: trustly-account-data-api-openapi.yml
  format: yaml
  label: Trustly Group Account Data API
  slug: trustly-account-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-account-data-api-openapi.yml
- filename: trustly-dispute-management-api-openapi.yml
  format: yaml
  label: Trustly Group Dispute Management API
  slug: trustly-dispute-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-dispute-management-api-openapi.yml
- filename: trustly-payment-providers-api-openapi.yml
  format: yaml
  label: Trustly Group Payment Providers API
  slug: trustly-payment-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/openapi/trustly-payment-providers-api-openapi.yml
consequence_counts:
  physical: 2
  read: 16
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trustly Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/{transactionId}/deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/{transactionId}/refund
operation_count: 31
overview: 'Trustly Group exposes 31 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 13 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Trustly Group
provider_slug: trustly
slug: trustly-agentic-access
source_filename: trustly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/trustly-account-data-api-openapi.yml, openapi/trustly-accounts-api-openapi.yml,\n  openapi/trustly-countries-api-openapi.yml, openapi/trustly-customers-api-openapi.yml, openapi/trustly-dispute-management-api-openapi.yml,\n  openapi/trustly-identity-api-openapi.yml, openapi/trustly-networkcheckapi-api-openapi.yml,\n  openapi/trustly-payment-providers-api-openapi.yml, openapi/trustly-payments-api-openapi.yml,\n  openapi/trustly-transactions-api-openapi.yml, openapi/trustly-verifycustomer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 16\n    acting: 15\n  by_consequence:\n    read: 16\n    write: 13\n    physical: 2\n  human_in_the_loop_required:\
  \ 0\noperations:\n- path: /transactions/{transactionId}/accountSummary\n  method: get\n  operationId: accountData_get-transaction-account-summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionId}/payment/paymentProvider/account/balance\n  method: get\n  operationId: accountData_get-transactions-account-balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionId}/payment/paymentProvider/user\n  method: get\n  operationId: accountData_get-user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionId}/payment/paymentProvider/accounts\n  method: get\n  operationId: accountData_list-selected-accounts\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback\n  method: post\n  operationId: accounts_post-account-feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/tokenize\n  method: post\n  operationId: accounts_post-accounts-tokenize?-verifyAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/verify\n  method: post\n  operationId: accounts_get-accounts-verify\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /countries\n  method: get\n  operationId: countries_get-countries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: customers_post-customers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: customers_get-customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: get\n  operationId: customers_get-customers-customerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: post\n  operationId: customers_post-customers-customerId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/recovery/dispute\n  method: post\n  operationId: disputeManagement_post-dispute-recovery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{transactionId}/user\n  method: get\n  operationId: identity_get-trustly-id-user-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionId}/user/detail\n  method: get\n  operationId: identity_get-trustly-id-user-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionId}/feedback\n  method: post\n  operationId: identity_post-transaction-feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/lookup\n\
  \  method: get\n  operationId: networkCheckApi_get-customer-lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentProviders\n  method: get\n  operationId: paymentProviders_get-paymentProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: payments_list-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{paymentId}\n  method: get\n  operationId: payments_get-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionId}/cancel\n  method: post\n  operationId: transactions_post-transactions-cancel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{transactionId}/capture\n  method: post\n  operationId: transactions_post-transactions-transactionId-capture\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{transactionId}/deposit\n  method: post\n  operationId: transactions_post-transactions-deposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /establish\n  method: post\n  operationId: transactions_post-establish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions\n  method: get\n  operationId: transactions_list-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionId}/capture/preAuth\n  method: post\n  operationId: transactions_post-transactions-transactionId-capture-preauth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{transactionId}/reclaim\n  method: post\n  operationId: transactions_post-transactions-transactionId-reclaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{transactionId}/refresh\n  method: post\n  operationId: transactions_post-transactions-refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{transactionId}/refund\n\
  \  method: post\n  operationId: transactions_post-transactions-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{transactionId}\n  method: get\n  operationId: transactions_get-transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionId}/payment/customer/verify\n  method: get\n  operationId: verifyCustomer_get-verify-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustly/refs/heads/main/agentic-access/trustly-agentic-access.yml
summary_line: 31 operations · 15 acting
tags:
- Company
- Payments
- Pay by Bank
- Open Banking
- Account-to-Account
- Payouts
- Direct Debit
- Bank Account Verification
- Identity Verification
- Fintech
- Webhook
- MCP
---
