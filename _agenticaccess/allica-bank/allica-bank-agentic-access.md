---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 26
api_specs:
- filename: allica-bank-account-access-api-openapi.yml
  format: yaml
  label: Allica Bank Account Access API
  slug: allica-bank-account-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-account-access-api-openapi.yml
- filename: allica-bank-accounts-api-openapi.yml
  format: yaml
  label: Allica Bank Accounts API
  slug: allica-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-accounts-api-openapi.yml
- filename: allica-bank-balances-api-openapi.yml
  format: yaml
  label: Allica Bank Balances API
  slug: allica-bank-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-balances-api-openapi.yml
- filename: allica-bank-beneficiaries-api-openapi.yml
  format: yaml
  label: Allica Bank Beneficiaries API
  slug: allica-bank-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-beneficiaries-api-openapi.yml
- filename: allica-bank-direct-debits-api-openapi.yml
  format: yaml
  label: Allica Bank Direct Debits API
  slug: allica-bank-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-direct-debits-api-openapi.yml
- filename: allica-bank-domestic-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Payments API
  slug: allica-bank-domestic-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-payments-api-openapi.yml
- filename: allica-bank-domestic-scheduled-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Scheduled Payments API
  slug: allica-bank-domestic-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-scheduled-payments-api-openapi.yml
- filename: allica-bank-domestic-standing-orders-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Standing Orders API
  slug: allica-bank-domestic-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-standing-orders-api-openapi.yml
- filename: allica-bank-file-payments-api-openapi.yml
  format: yaml
  label: Allica Bank File Payments API
  slug: allica-bank-file-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-file-payments-api-openapi.yml
- filename: allica-bank-offers-api-openapi.yml
  format: yaml
  label: Allica Bank Offers API
  slug: allica-bank-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-offers-api-openapi.yml
- filename: allica-bank-parties-api-openapi.yml
  format: yaml
  label: Allica Bank Parties API
  slug: allica-bank-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-parties-api-openapi.yml
- filename: allica-bank-payment-details-api-openapi.yml
  format: yaml
  label: Allica Bank Payment Details API
  slug: allica-bank-payment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-payment-details-api-openapi.yml
- filename: allica-bank-products-api-openapi.yml
  format: yaml
  label: Allica Bank Products API
  slug: allica-bank-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-products-api-openapi.yml
- filename: allica-bank-scheduled-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Scheduled Payments API
  slug: allica-bank-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-scheduled-payments-api-openapi.yml
- filename: allica-bank-standing-orders-api-openapi.yml
  format: yaml
  label: Allica Bank Standing Orders API
  slug: allica-bank-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-standing-orders-api-openapi.yml
- filename: allica-bank-transactions-api-openapi.yml
  format: yaml
  label: Allica Bank Transactions API
  slug: allica-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-transactions-api-openapi.yml
consequence_counts:
  physical: 9
  read: 26
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Allica Bank Agentic Access
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
  path: /domestic-scheduled-payment-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domestic-scheduled-payments
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
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /file-payment-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /file-payment-consents/{ConsentId}/file
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /file-payments
operation_count: 37
overview: 'Allica Bank exposes 37 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 2 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Allica Bank
provider_slug: allica-bank
slug: allica-bank-agentic-access
source_filename: allica-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/allica-bank-account-information-openapi.yaml, openapi/allica-bank-payment-initiation-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    acting: 11\n    connected: 26\n  by_consequence:\n    write: 2\n    read: 26\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /account-access-consents\n  method: post\n  operationId: CreateAccountAccessConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /account-access-consents/{ConsentId}\n  method: get\n  operationId: GetAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-access-consents/{ConsentId}\n  method: delete\n  operationId: DeleteAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: GetAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}\n  method:\
  \ get\n  operationId: GetAccountsAccountId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/balances\n  method: get\n  operationId: GetAccountsAccountIdBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/beneficiaries\n  method: get\n  operationId: GetAccountsAccountIdBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/direct-debits\n  method: get\n  operationId: GetAccountsAccountIdDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/offers\n  method: get\n  operationId: GetAccountsAccountIdOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/parties\n  method: get\n  operationId: GetAccountsAccountIdParties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/party\n  method: get\n  operationId: GetAccountsAccountIdParty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/product\n  method: get\n  operationId: GetAccountsAccountIdProduct\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/scheduled-payments\n  method: get\n  operationId: GetAccountsAccountIdScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/standing-orders\n  method: get\n  operationId: GetAccountsAccountIdStandingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/transactions\n  method: get\n  operationId: GetAccountsAccountIdTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balances\n\
  \  method: get\n  operationId: GetBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-payment-consents\n  method: post\n  operationId: CreateDomesticPaymentConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-payment-consents/{ConsentId}\n  method: get\n  operationId: GetDomesticPaymentConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-payment-consents/{ConsentId}/funds-confirmation\n\
  \  method: get\n  operationId: GetDomesticPaymentConsentsConsentIdFundsConfirmation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-payments\n  method: post\n  operationId: CreateDomesticPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-payments/{DomesticPaymentId}\n  method: get\n  operationId: GetDomesticPaymentsDomesticPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /domestic-payments/{DomesticPaymentId}/payment-details\n  method: get\n  operationId: GetDomesticPaymentsDomesticPaymentIdPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-scheduled-payment-consents\n  method: post\n  operationId: CreateDomesticScheduledPaymentConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-scheduled-payment-consents/{ConsentId}\n  method: get\n  operationId: GetDomesticScheduledPaymentConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-scheduled-payments\n  method: post\n  operationId: CreateDomesticScheduledPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-scheduled-payments/{DomesticScheduledPaymentId}\n  method: get\n  operationId: GetDomesticScheduledPaymentsDomesticScheduledPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-scheduled-payments/{DomesticScheduledPaymentId}/payment-details\n  method: get\n  operationId:\
  \ GetDomesticScheduledPaymentsDomesticScheduledPaymentIdPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-standing-order-consents\n  method: post\n  operationId: CreateDomesticStandingOrderConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-standing-order-consents/{ConsentId}\n  method: get\n  operationId: GetDomesticStandingOrderConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /domestic-standing-orders\n  method: post\n  operationId: CreateDomesticStandingOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-standing-orders/{DomesticStandingOrderId}\n  method: get\n  operationId: GetDomesticStandingOrdersDomesticStandingOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-standing-orders/{DomesticStandingOrderId}/payment-details\n  method: get\n  operationId: GetDomesticStandingOrdersDomesticStandingOrderIdPaymentDetails\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file-payment-consents\n  method: post\n  operationId: CreateFilePaymentConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file-payment-consents/{ConsentId}\n  method: get\n  operationId: GetFilePaymentConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file-payment-consents/{ConsentId}/file\n  method: post\n  operationId: CreateFilePaymentConsentsConsentIdFile\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file-payments\n  method: post\n  operationId: CreateFilePayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file-payments/{FilePaymentId}\n  method: get\n  operationId: GetFilePaymentsFilePaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/agentic-access/allica-bank-agentic-access.yml
summary_line: 37 operations · 11 acting
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- SME
- Business Banking
- Fintech
---
