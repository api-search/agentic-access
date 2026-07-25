---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 17
api_specs:
- filename: zopa-account-access-api-openapi.yml
  format: yaml
  label: zopa Account Access API
  slug: zopa-account-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-account-access-api-openapi.yml
- filename: zopa-accounts-api-openapi.yml
  format: yaml
  label: zopa Accounts API
  slug: zopa-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-accounts-api-openapi.yml
- filename: zopa-balances-api-openapi.yml
  format: yaml
  label: zopa Balances API
  slug: zopa-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-balances-api-openapi.yml
- filename: zopa-beneficiaries-api-openapi.yml
  format: yaml
  label: zopa Beneficiaries API
  slug: zopa-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-beneficiaries-api-openapi.yml
- filename: zopa-direct-debits-api-openapi.yml
  format: yaml
  label: zopa Direct Debits API
  slug: zopa-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-direct-debits-api-openapi.yml
- filename: zopa-domestic-payments-api-openapi.yml
  format: yaml
  label: zopa Domestic Payments API
  slug: zopa-domestic-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-domestic-payments-api-openapi.yml
- filename: zopa-domestic-standing-orders-api-openapi.yml
  format: yaml
  label: zopa Domestic Standing Orders API
  slug: zopa-domestic-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-domestic-standing-orders-api-openapi.yml
- filename: zopa-offers-api-openapi.yml
  format: yaml
  label: zopa Offers API
  slug: zopa-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-offers-api-openapi.yml
- filename: zopa-parties-api-openapi.yml
  format: yaml
  label: zopa Parties API
  slug: zopa-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-parties-api-openapi.yml
- filename: zopa-standing-orders-api-openapi.yml
  format: yaml
  label: zopa Standing Orders API
  slug: zopa-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-standing-orders-api-openapi.yml
- filename: zopa-statements-api-openapi.yml
  format: yaml
  label: zopa Statements API
  slug: zopa-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-statements-api-openapi.yml
- filename: zopa-transactions-api-openapi.yml
  format: yaml
  label: zopa Transactions API
  slug: zopa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/openapi/zopa-transactions-api-openapi.yml
consequence_counts:
  physical: 4
  read: 17
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zopa Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-payment-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-standing-order-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-standing-orders
operation_count: 23
overview: 'zopa exposes 23 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 2 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: zopa
provider_slug: zopa
slug: zopa-agentic-access
source_filename: zopa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/zopa-account-info-openapi-original.yml, openapi/zopa-payment-initiation-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 6\n    connected: 17\n  by_consequence:\n    write: 2\n    read: 17\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /account-access-consents\n  method: post\n  operationId: CreateAccountAccessConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /account-access-consents/{ConsentId}\n  method: get\n  operationId: GetAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-access-consents/{ConsentId}\n  method: delete\n  operationId: DeleteAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: GetAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}\n  method:\
  \ get\n  operationId: GetAccountsAccountId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/balances\n  method: get\n  operationId: GetAccountsAccountIdBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/beneficiaries\n  method: get\n  operationId: GetAccountsAccountIdBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/direct-debits\n  method: get\n  operationId: GetAccountsAccountIdDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/offers\n  method: get\n  operationId: GetAccountsAccountIdOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/party\n  method: get\n  operationId: GetAccountsAccountIdParty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/standing-orders\n  method: get\n  operationId: GetAccountsAccountIdStandingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/statements\n  method: get\n  operationId: GetAccountsAccountIdStatements\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/transactions\n  method: get\n  operationId: GetAccountsAccountIdTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /party\n  method: get\n  operationId: GetParty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-payment-consents\n  method: post\n  operationId: CreateDomesticPaymentConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-payment-consents/{ConsentId}\n  method: get\n  operationId: GetDomesticPaymentConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-payment-consents/{ConsentId}/funds-confirmation\n  method: get\n  operationId: GetDomesticPaymentConsentsConsentIdFundsConfirmation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-payments\n  method: post\n  operationId: CreateDomesticPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-payments/{DomesticPaymentId}\n  method: get\n  operationId: GetDomesticPaymentsDomesticPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-standing-order-consents\n  method: post\n  operationId: CreateDomesticStandingOrderConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-standing-order-consents/{ConsentId}\n  method: get\n\
  \  operationId: GetDomesticStandingOrderConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-standing-orders\n  method: post\n  operationId: CreateDomesticStandingOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-standing-orders/{DomesticStandingOrderId}\n  method: get\n  operationId: GetDomesticStandingOrdersDomesticStandingOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zopa/refs/heads/main/agentic-access/zopa-agentic-access.yml
summary_line: 23 operations · 6 acting
tags:
- Company
- Banking
- Fintech
- Open Banking
- PSD2
- Payments
- Account Information
- Payment Initiation
- FAPI
- United Kingdom
- Digital Bank
- Lending
---
