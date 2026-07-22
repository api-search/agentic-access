---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 54
api_specs:
- filename: natwest-account-transaction-openapi.yml
  format: yaml
  label: NatWest Account and Transaction API
  slug: natwest-account-and-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-account-transaction-openapi.yml
- filename: natwest-payment-initiation-openapi.yml
  format: yaml
  label: NatWest Payment Initiation API
  slug: natwest-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-payment-initiation-openapi.yml
- filename: natwest-confirmation-of-funds-openapi.yml
  format: yaml
  label: NatWest Confirmation of Funds API
  slug: natwest-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-confirmation-of-funds-openapi.yml
consequence_counts:
  physical: 15
  read: 54
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Natwest Agentic Access
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
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /international-payment-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /international-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /international-scheduled-payment-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /international-scheduled-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /international-standing-order-consents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /international-standing-orders
operation_count: 74
overview: 'NatWest Group exposes 74 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 54 read, 5 write, and 15 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NatWest Group
provider_slug: natwest
slug: natwest-agentic-access
source_filename: natwest-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/natwest-account-transaction-openapi.yml, openapi/natwest-confirmation-of-funds-openapi.yml,\n  openapi/natwest-payment-initiation-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 74\n  by_action_class:\n    acting: 20\n    connected: 54\n  by_consequence:\n    write: 5\n    read: 54\n    physical: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /account-access-consents\n  method: post\n  operationId: CreateAccountAccessConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /account-access-consents/{ConsentId}\n  method: get\n  operationId: GetAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-access-consents/{ConsentId}\n  method: delete\n  operationId: DeleteAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: GetAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /accounts/{AccountId}\n  method: get\n  operationId: GetAccountsAccountId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/balances\n  method: get\n  operationId: GetAccountsAccountIdBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/beneficiaries\n  method: get\n  operationId: GetAccountsAccountIdBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/direct-debits\n  method: get\n  operationId: GetAccountsAccountIdDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/offers\n  method: get\n  operationId: GetAccountsAccountIdOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/parties\n  method: get\n  operationId: GetAccountsAccountIdParties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/party\n  method: get\n  operationId: GetAccountsAccountIdParty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/product\n  method: get\n  operationId: GetAccountsAccountIdProduct\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/scheduled-payments\n  method: get\n  operationId: GetAccountsAccountIdScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/standing-orders\n  method: get\n  operationId: GetAccountsAccountIdStandingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/statements\n  method: get\n  operationId: GetAccountsAccountIdStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/statements/{StatementId}\n  method: get\n  operationId: GetAccountsAccountIdStatementsStatementId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/statements/{StatementId}/file\n  method: get\n  operationId: GetAccountsAccountIdStatementsStatementIdFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/statements/{StatementId}/transactions\n  method: get\n  operationId: GetAccountsAccountIdStatementsStatementIdTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/transactions\n\
  \  method: get\n  operationId: GetAccountsAccountIdTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balances\n  method: get\n  operationId: GetBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beneficiaries\n  method: get\n  operationId: GetBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct-debits\n  method: get\n  operationId: GetDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers\n  method: get\n \
  \ operationId: GetOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /party\n  method: get\n  operationId: GetParty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: GetProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-payments\n  method: get\n  operationId: GetScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /standing-orders\n  method: get\n  operationId: GetStandingOrders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements\n  method: get\n  operationId: GetStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: GetTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funds-confirmation-consents\n  method: post\n  operationId: CreateFundsConfirmationConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - fundsconfirmations\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /funds-confirmation-consents/{ConsentId}\n  method: get\n  operationId: GetFundsConfirmationConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - fundsconfirmations\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funds-confirmation-consents/{ConsentId}\n  method: delete\n  operationId: DeleteFundsConfirmationConsentsConsentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - fundsconfirmations\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funds-confirmations\n  method: post\n  operationId: CreateFundsConfirmations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - fundsconfirmations\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-payment-consents\n  method: post\n  operationId: CreateDomesticPaymentConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-payment-consents/{ConsentId}\n  method: get\n  operationId: GetDomesticPaymentConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-payment-consents/{ConsentId}/funds-confirmation\n \
  \ method: get\n  operationId: GetDomesticPaymentConsentsConsentIdFundsConfirmation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-payments\n  method: post\n  operationId: CreateDomesticPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-payments/{DomesticPaymentId}\n  method: get\n  operationId: GetDomesticPaymentsDomesticPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-payments/{DomesticPaymentId}/payment-details\n\
  \  method: get\n  operationId: GetDomesticPaymentsDomesticPaymentIdPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-scheduled-payment-consents\n  method: post\n  operationId: CreateDomesticScheduledPaymentConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-scheduled-payment-consents/{ConsentId}\n  method: get\n  operationId: GetDomesticScheduledPaymentConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /domestic-scheduled-payments\n  method: post\n  operationId: CreateDomesticScheduledPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-scheduled-payments/{DomesticScheduledPaymentId}\n  method: get\n  operationId: GetDomesticScheduledPaymentsDomesticScheduledPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-scheduled-payments/{DomesticScheduledPaymentId}/payment-details\n  method: get\n  operationId: GetDomesticScheduledPaymentsDomesticScheduledPaymentIdPaymentDetails\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-standing-order-consents\n  method: post\n  operationId: CreateDomesticStandingOrderConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-standing-order-consents/{ConsentId}\n  method: get\n  operationId: GetDomesticStandingOrderConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-standing-orders\n  method: post\n\
  \  operationId: CreateDomesticStandingOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domestic-standing-orders/{DomesticStandingOrderId}\n  method: get\n  operationId: GetDomesticStandingOrdersDomesticStandingOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domestic-standing-orders/{DomesticStandingOrderId}/payment-details\n  method: get\n  operationId: GetDomesticStandingOrdersDomesticStandingOrderIdPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file-payment-consents\n  method: post\n  operationId: CreateFilePaymentConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file-payment-consents/{ConsentId}\n  method: get\n  operationId: GetFilePaymentConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file-payment-consents/{ConsentId}/file\n  method: post\n  operationId: CreateFilePaymentConsentsConsentIdFile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file-payment-consents/{ConsentId}/file\n  method: get\n  operationId: GetFilePaymentConsentsConsentIdFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file-payments\n  method: post\n  operationId: CreateFilePayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /file-payments/{FilePaymentId}\n  method: get\n  operationId: GetFilePaymentsFilePaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file-payments/{FilePaymentId}/payment-details\n  method: get\n  operationId: GetFilePaymentsFilePaymentIdPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file-payments/{FilePaymentId}/report-file\n  method: get\n  operationId: GetFilePaymentsFilePaymentIdReportFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-payment-consents\n  method: post\n  operationId: CreateInternationalPaymentConsents\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /international-payment-consents/{ConsentId}\n  method: get\n  operationId: GetInternationalPaymentConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-payment-consents/{ConsentId}/funds-confirmation\n  method: get\n  operationId: GetInternationalPaymentConsentsConsentIdFundsConfirmation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-payments\n\
  \  method: post\n  operationId: CreateInternationalPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /international-payments/{InternationalPaymentId}\n  method: get\n  operationId: GetInternationalPaymentsInternationalPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-payments/{InternationalPaymentId}/payment-details\n  method: get\n  operationId: GetInternationalPaymentsInternationalPaymentIdPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-scheduled-payment-consents\n  method: post\n  operationId: CreateInternationalScheduledPaymentConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /international-scheduled-payment-consents/{ConsentId}\n  method: get\n  operationId: GetInternationalScheduledPaymentConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-scheduled-payment-consents/{ConsentId}/funds-confirmation\n  method: get\n  operationId: GetInternationalScheduledPaymentConsentsConsentIdFundsConfirmation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-scheduled-payments\n  method: post\n  operationId: CreateInternationalScheduledPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /international-scheduled-payments/{InternationalScheduledPaymentId}\n  method: get\n  operationId: GetInternationalScheduledPaymentsInternationalScheduledPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /international-scheduled-payments/{InternationalScheduledPaymentId}/payment-details\n  method: get\n  operationId: GetInternationalScheduledPaymentsInternationalScheduledPaymentIdPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-standing-order-consents\n  method: post\n  operationId: CreateInternationalStandingOrderConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /international-standing-order-consents/{ConsentId}\n  method: get\n  operationId: GetInternationalStandingOrderConsentsConsentId\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-standing-orders\n  method: post\n  operationId: CreateInternationalStandingOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /international-standing-orders/{InternationalStandingOrderPaymentId}\n  method: get\n  operationId: GetInternationalStandingOrdersInternationalStandingOrderPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international-standing-orders/{InternationalStandingOrderPaymentId}/payment-details\n\
  \  method: get\n  operationId: GetInternationalStandingOrdersInternationalStandingOrderPaymentIdPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/agentic-access/natwest-agentic-access.yml
summary_line: 74 operations · 20 acting
tags:
- Banking
- Open Banking
- Financial Services
- Payments
- PSD2
- FAPI
- Fintech
- Account Information
---
