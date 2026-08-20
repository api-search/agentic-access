---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 6
api_specs:
- filename: bmo-account-validation-openapi.json
  format: json
  label: BMO Account Validation API
  slug: bmo-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-account-validation-openapi.json
- filename: bmo-account-information-openapi.json
  format: json
  label: BMO Account Information API
  slug: bmo-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-account-information-openapi.json
- filename: bmo-ach-payments-openapi.json
  format: json
  label: BMO ACH Payments API
  slug: bmo-ach-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-ach-payments-openapi.json
- filename: bmo-wire-payments-us-openapi.json
  format: json
  label: BMO Wire Payments (U.S.) API
  slug: bmo-wire-payments-us-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-wire-payments-us-openapi.json
- filename: bmo-wire-payments-ca-openapi.json
  format: json
  label: BMO Wire Payments (Canada) API
  slug: bmo-wire-payments-ca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-wire-payments-ca-openapi.json
- filename: bmo-eft-payments-openapi.json
  format: json
  label: BMO EFT Payments API
  slug: bmo-eft-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-eft-payments-openapi.json
- filename: bmo-interac-instant-payments-openapi.json
  format: json
  label: BMO Instant Payments (Interac) API
  slug: bmo-interac-instant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-interac-instant-payments-openapi.json
- filename: bmo-image-retrieval-swagger.json
  format: json
  label: BMO Image Retrieval API
  slug: bmo-image-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-image-retrieval-swagger.json
- filename: bmo-authorize-token-swagger.json
  format: json
  label: BMO Authorize & Token API
  slug: bmo-authorize-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-authorize-token-swagger.json
- filename: bmo-client-data-encryption-key-swagger.json
  format: json
  label: BMO Client Data Encryption Key API
  slug: bmo-client-data-encryption-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-client-data-encryption-key-swagger.json
- filename: bmo-push-notification-openapi.json
  format: json
  label: BMO Push Notification API
  slug: bmo-push-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-push-notification-openapi.json
consequence_counts:
  physical: 18
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bmo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentStatusUpdate/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/ach/payment-initiation/customer-credit-transfer-initiation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/ach/payment-initiation/customer-direct-debit-initiation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/ach/payment-initiation/get-transaction-status/get
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/eft/payment-initiation/customer-credit-transfer-initiation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/eft/payment-initiation/customer-direct-debit-initiation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/eft/payment-initiation/get-transaction-status/get
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/interac-etransfer/payment-execution/customer-payment-cancellation-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/interac-etransfer/payment-initiation/creditor-payment-activation-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/interac-etransfer/payment-initiation/customer-credit-transfer-initiation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/interac-etransfer/payment-initiation/get-emt-recipient-payment-options/get
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/interac-etransfer/payment-initiation/get-request-for-payment-transaction
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/interac-etransfer/payment-initiation/get-transaction
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/wires/payment-initiation/creditor-payment-activation-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/wires/payment-initiation/customer-credit-transfer-initiation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/wires/payment-initiation/customer-credit-transfer-initiation/us
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/wires/payment-initiation/get-transaction-status/get
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tpp/wires/payment-initiation/get-transaction-status/us/get
operation_count: 30
overview: 'BMO exposes 30 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 6 write, and 18 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BMO
provider_slug: bmo
slug: bmo-agentic-access
source_filename: bmo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/bmo-account-information-openapi.json, openapi/bmo-account-validation-openapi.json,\n  openapi/bmo-ach-payments-openapi.json, openapi/bmo-authorize-token-swagger.json, openapi/bmo-client-data-encryption-key-swagger.json,\n  openapi/bmo-eft-payments-openapi.json, openapi/bmo-image-retrieval-swagger.json, openapi/bmo-interac-instant-payments-openapi.json,\n  openapi/bmo-push-notification-openapi.json, openapi/bmo-wire-payments-ca-openapi.json, openapi/bmo-wire-payments-us-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 6\n    acting: 24\n  by_consequence:\n    read: 6\n    write: 6\n    physical: 18\n  human_in_the_loop_required: 0\n\
  operations:\n- path: /accounts\n  method: get\n  operationId: Search for Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - FinancialInformation\n- path: /accounts/{accountId}\n  method: get\n  operationId: Get an Account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - FinancialInformation\n- path: /accounts/{accountId}/transactions\n  method: get\n  operationId: Search for Account Transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - FinancialInformation\n- path: /accounts/validate/get\n  method: post\n  operationId: ValidateAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - AccountValidation\n- path: /tpp/ach/payment-initiation/customer-credit-transfer-initiation\n  method: post\n  operationId: CreditPaymentInitiation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppach.payment-initiation.create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/ach/payment-initiation/customer-direct-debit-initiation\n  method: post\n  operationId: DebitPaymentInitiation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppach.payment-initiation.create\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/ach/payment-initiation/get-transaction-status/get\n  method: post\n  operationId: PaymentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppach.payment-initiation.read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/ach/customer-access-entitlement/commercial-user-access-arrangement/get\n  method: post\n  operationId: ACHCompanyIDList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bmo.tppach.payment-initiation.read\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth20/authorize\n  method: get\n  operationId: Retrieve authorization code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth20/token\n  method: post\n  operationId: Request Access Tokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issued-device-administration/client-data-encryption-key/get\n  method: post\n  operationId: post-retrievecryptoinstruction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/eft/payment-initiation/customer-credit-transfer-initiation\n  method: post\n  operationId: CustomerCreditTransferInitiation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppeft.payment-initiation.create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/eft/payment-initiation/customer-direct-debit-initiation\n  method: post\n  operationId: CustomerDebitTransferInitiation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppeft.payment-initiation.create\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/eft/payment-initiation/get-transaction-status/get\n  method: post\n  operationId: GetTransactionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppeft.payment-initiation.read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/eft/customer-access-entitlement/commercial-user-access-arrangement/get\n  method: post\n  operationId: GetServiceAgreementList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bmo.tppeft.payment-initiation.read\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/transaction-images-accounts\n  method: get\n  operationId: Search for Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ItemImage\n- path: /accounts/{accountId}/transaction-images/get\n  method: post\n  operationId: Search for Images\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - ItemImage\n- path: /accounts/{accountId}/transaction-images/{imageId}\n  method: get\n  operationId: Retrieve Images\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ItemImage\n- path: /tpp/interac-etransfer/payment-initiation/get-transaction\n  method: post\n  operationId: TPP-EMTGetTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppinterac.payment-initiation.read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/interac-etransfer/payment-initiation/get-request-for-payment-transaction\n  method: post\n  operationId: TPP-EMTGetRequestForPaymentTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppinterac.payment-initiation.create\n    audience: null\n    token:\n   \
  \   max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/interac-etransfer/payment-initiation/creditor-payment-activation-request\n  method: post\n  operationId: TPP-EMTCreditorPaymentActivationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppinterac.payment-initiation.create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/interac-etransfer/payment-initiation/get-emt-recipient-payment-options/get\n  method: post\n  operationId: TPP-EMTRecipientPaymentOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    scope:\n    - bmo.tppinterac.payment-initiation.read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/interac-etransfer/payment-initiation/customer-credit-transfer-initiation\n  method: post\n  operationId: TPP-EMTCustomerCreditTransferInitiation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppinterac.payment-initiation.create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/interac-etransfer/payment-execution/customer-payment-cancellation-request\n  method: post\n  operationId: TPP-EMTCustomerCancelTransferInitiation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppinterac.payment-execution.create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentStatusUpdate/v1\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/wires/payment-initiation/customer-credit-transfer-initiation\n  method: post\n  operationId: TppCustomerCreditTransferInitiation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    scope:\n    - bmo.tppwiresca.payment-initiation.create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/wires/payment-initiation/get-transaction-status/get\n  method: post\n  operationId: TppGetPaymentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppwiresca.payment-initiation.read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/wires/payment-initiation/customer-credit-transfer-initiation/us\n  method: post\n  operationId: TppCustomerCreditTransferInitiation\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppwiresus.payment-initiation.create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/wires/payment-initiation/get-transaction-status/us/get\n  method: post\n  operationId: TppGetPaymentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppwiresus.payment-initiation.read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tpp/wires/payment-initiation/creditor-payment-activation-request\n  method: post\n  operationId: TppCreditorPaymentActivationRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bmo.tppwiresus.payment-initiation.create\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/agentic-access/bmo-agentic-access.yml
summary_line: 30 operations · 24 acting
tags:
- Financial-Services
- Banking
- United States
- Open Finance
- Payments
- Commercial Banking
- Treasury Management
- Account Validation
---
