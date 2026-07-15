---
acting_count: 73
action_class_counts:
  acting: 73
  connected: 65
api_specs:
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Applications API
  slug: unit-co-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Customers API
  slug: unit-co-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Accounts API
  slug: unit-co-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Cards API
  slug: unit-co-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Card Authorizations API
  slug: unit-co-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Payments API
  slug: unit-co-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Counterparties API
  slug: unit-co-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Checks API
  slug: unit-co-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Transactions API
  slug: unit-co-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Statements and Tax Forms API
  slug: unit-co-statements-tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Events and Webhooks API
  slug: unit-co-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Risk and Fraud Prevention API
  slug: unit-co-risk-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Credit and Repayments API
  slug: unit-co-credit-repayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Fees and Rewards API
  slug: unit-co-fees-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit API Tokens API
  slug: unit-co-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
consequence_counts:
  physical: 22
  read: 65
  safety-critical: 8
  write: 43
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Unit Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{accountId}/activate-daca
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{accountId}/deactivate-daca
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{accountId}/enter-daca
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /recurring-payments/{paymentId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /recurring-repayments/{recurringRepaymentId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /stop-payments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /stop-payments/{stopPaymentId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /webhooks/{webhookId}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/relationships/customers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /accounts/{accountId}/relationships/customers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cash-deposits/barcodes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /check-deposits/{checkDepositId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-deposits/{checkDepositId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-payments/{checkPaymentId}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-payments/{checkPaymentId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-payments/{checkPaymentId}/return
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payments/{paymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /received-payments/{paymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /received-payments/{paymentId}/advance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /received-payments/{paymentId}/reprocess
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /recurring-payments
operation_count: 138
overview: 'Unit exposes 138 API operations that an AI agent could call, of which 73 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 65 read, 43 write, 22 physical, and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Unit
provider_slug: unit-co
slug: unit-co-agentic-access
source_filename: unit-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/unit-co-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 138\n  by_action_class:\n    connected: 65\n    acting: 73\n  by_consequence:\n    read: 65\n    write: 43\n    safety-critical: 8\n    physical: 22\n  human_in_the_loop_required: 8\noperations:\n- path: /applications\n  method: get\n  operationId: getApplicationsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}\n  method: patch\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/cancel\n  method: post\n  operationId: cancelApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/documents\n  method: get\n  operationId: getApplicationDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}/documents\n  method: post\n  operationId: createApplicationDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/documents/{documentId}/multipart\n  method: put\n  operationId: uploadApplicationDocumentFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/documents/{documentId}/verify\n  method: put\n  operationId: verifyDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/documents/{documentId}/download\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}/missing-fields\n  method: get\n  operationId: getApplicationMissingFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /application-forms\n  method: get\n  operationId: getApplicationFormsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /application-forms\n  method: post\n  operationId: createApplicationForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /application-forms/{applicationFormId}\n  method: get\n  operationId: getApplicationForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beneficial-owner/{beneficialOwnerId}\n  method: patch\n  operationId: updateBusinessBeneficialOwner\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: getCustomersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/archive\n  method: post\n  operationId: archiveCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/authorized-users\n  method: post\n  operationId: addAuthorizedUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/authorized-users\n  method: delete\n  operationId: removeAuthorizedUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: getAccountsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n\
  \  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/limits\n  method: get\n  operationId: getAccountLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/freeze\n  method: post\n  operationId: freezeAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/unfreeze\n  method: post\n  operationId: unfreezeAccount\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/close\n  method: post\n  operationId: closeAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/reopen\n  method: post\n  operationId: reopenAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /accounts/{accountId}/enter-daca\n  method: post\n  operationId: enterDaca\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /accounts/{accountId}/activate-daca\n  method: post\n  operationId: activateDaca\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /accounts/{accountId}/deactivate-daca\n  method: post\n  operationId: deactivateDaca\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account-end-of-day\n  method: get\n  operationId: getAccountBalanceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/repayment-information\n  method: get\n  operationId: getRepaymentInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/deposit-products\n  method: get\n  operationId: getDepositProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/relationships/customers\n  method:\
  \ post\n  operationId: addAccountOwners\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/relationships/customers\n  method: delete\n  operationId: removeAccountOwners\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards\n  method: get\n  operationId: getCardsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardId}\n  method: patch\n  operationId: updateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/report-lost\n  method: post\n  operationId: reportLostCard\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/report-stolen\n  method: post\n  operationId: reportStolenCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/close\n  method: post\n  operationId: closeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/freeze\n\
  \  method: post\n  operationId: freezeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/unfreeze\n  method: post\n  operationId: unfreezeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/replace\n  method: post\n  operationId: replaceCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /cards/{cardId}/limits\n  method: get\n  operationId: getCardLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardId}/secure-data/pin/status\n  method: get\n  operationId: getCardPinStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atm-locations\n  method: get\n  operationId: getAtmLocationsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations\n  method: get\n  operationId: getAuthorizationsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/{authorizationId}\n  method: get\n  operationId:\
  \ getAuthorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization-requests\n  method: get\n  operationId: getAuthorizationRequestsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization-requests/{authorizationId}\n  method: get\n  operationId: getAuthorizationRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization-requests/{authorizationId}/approve\n  method: post\n  operationId: approveAuthorizationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /authorization-requests/{authorizationId}/decline\n  method: post\n  operationId: declineAuthorizationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: get\n  operationId: getPaymentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{paymentId}\n  method: patch\n  operationId: updatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/cancel\n  method: post\n  operationId: cancelPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /received-payments\n  method: get\n  operationId: getReceivedPaymentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /received-payments/{paymentId}\n  method: get\n  operationId: getReceivedPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /received-payments/{paymentId}\n  method: patch\n  operationId: updateReceivedPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /received-payments/{paymentId}/advance\n\
  \  method: post\n  operationId: advanceReceivedPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /received-payments/{paymentId}/reprocess\n  method: post\n  operationId: reprocessReceivedPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /returns/{transactionId}\n  method: post\n  operationId: returnReceivedAchTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurring-payments\n  method: get\n  operationId: getRecurringPaymentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring-payments\n  method: post\n  operationId: createRecurringPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurring-payments/{paymentId}\n  method: get\n  operationId: getRecurringPayment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring-payments/{paymentId}/disable\n  method: post\n  operationId: disableRecurringPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /recurring-payments/{paymentId}/enable\n  method: post\n  operationId: enableRecurringPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cash-deposits/barcodes\n\
  \  method: post\n  operationId: generateCashDepositBarcode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cash-deposits/barcodes/{barcodeNumber}/image\n  method: get\n  operationId: getBarcodeImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /store-locations\n  method: get\n  operationId: getCashDepositStoreLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counterparties\n  method: get\n  operationId: getCounterpartiesList\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counterparties\n  method: post\n  operationId: createCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /counterparties/{counterpartyId}\n  method: get\n  operationId: getCounterparty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counterparties/{counterpartyId}\n  method: patch\n  operationId: updateCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /counterparties/{counterpartyId}\n  method: delete\n  operationId: deleteCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /counterparties/{counterpartyId}/balance\n  method: get\n  operationId: getCounterpartyBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /institutions/{routingNumber}\n  method: get\n  operationId: getInstitution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-deposits\n  method: get\n  operationId: getCheckDepositsList\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-deposits\n  method: post\n  operationId: createCheckDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-deposits/{checkDepositId}\n  method: get\n  operationId: getCheckDeposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-deposits/{checkDepositId}\n  method: patch\n  operationId: updateCheckDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-deposits/{checkDepositId}/confirm\n  method: post\n  operationId: confirmCheckDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-deposits/{checkDepositId}/front\n  method: get\n  operationId: getFrontCheckDepositImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-payments\n  method: get\n  operationId: getCheckPaymentsList\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-payments\n  method: post\n  operationId: createCheckPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-payments/{checkPaymentId}\n  method: get\n  operationId: getCheckPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-payments/{checkPaymentId}/approve\n  method: post\n  operationId: approveCheckPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-payments/{checkPaymentId}/cancel\n  method: post\n  operationId: cancelCheckPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-payments/{checkPaymentId}/return\n  method: post\n  operationId: returnCheckPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /transactions\n  method: get\n  operationId: getTransactionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions/{transactionId}\n  method: patch\n  operationId: updateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statements\n  method: get\n  operationId: getStatementsList\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements/{statementId}/html\n  method: get\n  operationId: getStatementHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements/{statementId}/pdf\n  method: get\n  operationId: getStatementPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements/{accountId}/bank/pdf\n  method: get\n  operationId: getStatementBankPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tax-forms\n  method: get\n  operationId: getTaxFormsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /tax-forms/{taxFormId}\n  method: get\n  operationId: getTaxForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tax-forms/{taxFormId}/pdf\n  method: get\n  operationId: getTaxFormPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: getEventsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}\n  method: post\n  operationId: fireEvent\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 90\n\n# --- truncated at 32 KB (40 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/agentic-access/unit-co-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/agentic-access/unit-co-agentic-access.yml
summary_line: 138 operations · 73 acting · 8 human-in-the-loop
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
- Lending
- JSON:API
---
