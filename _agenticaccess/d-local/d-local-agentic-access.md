---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 22
api_specs:
- filename: d-local-payments-api-openapi.yml
  format: yaml
  label: dLocal Payments API
  slug: d-local-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-payments-api-openapi.yml
- filename: d-local-refunds-api-openapi.yml
  format: yaml
  label: dLocal Refunds API
  slug: d-local-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-refunds-api-openapi.yml
- filename: d-local-cards-api-openapi.yml
  format: yaml
  label: dLocal Cards API
  slug: d-local-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-cards-api-openapi.yml
- filename: d-local-payouts-v3-api-openapi.yml
  format: yaml
  label: dLocal Payouts V3 API
  slug: d-local-payouts-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-payouts-v3-api-openapi.yml
- filename: d-local-platforms-api-openapi.yml
  format: yaml
  label: dLocal For Platforms API
  slug: d-local-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-platforms-api-openapi.yml
- filename: d-local-kyc-verifications-api-openapi.yml
  format: yaml
  label: dLocal KYC Verifications API
  slug: d-local-kyc-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-kyc-verifications-api-openapi.yml
- filename: d-local-chargebacks-api-openapi.yml
  format: yaml
  label: dLocal Chargebacks API
  slug: d-local-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-chargebacks-api-openapi.yml
- filename: d-local-enrollments-api-openapi.yml
  format: yaml
  label: dLocal Enrollments API
  slug: d-local-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-enrollments-api-openapi.yml
- filename: d-local-exchange-rates-api-openapi.yml
  format: yaml
  label: dLocal Exchange Rates API
  slug: d-local-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-exchange-rates-api-openapi.yml
consequence_counts:
  physical: 13
  read: 22
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: D Local Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/accounts/{account_id}/bank-accounts/{bank_account_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chargebacks/simulate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{authorization_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{authorization_id}/captures
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{payment_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v3
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v3/quotes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v3/{payout_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v3/{payout_id}/release
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /secure_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/transfers/{transfer_id}/cancel
operation_count: 49
overview: 'dLocal exposes 49 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 13 write, 13 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: dLocal
provider_slug: d-local
slug: d-local-agentic-access
source_filename: d-local-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/d-local-cards-api-openapi.yml, openapi/d-local-chargebacks-api-openapi.yml,\n  openapi/d-local-enrollments-api-openapi.yml, openapi/d-local-exchange-rates-api-openapi.yml,\n  openapi/d-local-kyc-verifications-api-openapi.yml, openapi/d-local-payments-api-openapi.yml,\n  openapi/d-local-payouts-v3-api-openapi.yml, openapi/d-local-platforms-api-openapi.yml, openapi/d-local-refunds-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    acting: 27\n    connected: 22\n  by_consequence:\n    write: 13\n    read: 22\n    physical: 13\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /secure_cards\n  method: post\n  operationId:\
  \ createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /secure_cards/{card_id}\n  method: get\n  operationId: retrieveCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secure_cards/{card_id}\n  method: delete\n  operationId: deleteCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chargebacks/{chargeback_id}\n  method: get\n  operationId: retrieveChargeback\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chargebacks/{chargeback_id}/status\n  method: get\n  operationId: retrieveChargebackStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chargebacks/simulate\n  method: post\n  operationId: simulateChargeback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrollments\n  method: post\n  operationId: createEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrollments/{enrollment_id}\n  method: get\n  operationId: getEnrollment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollments/{enrollment_id}/cancel\n  method: post\n  operationId: cancelEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange-rates\n  method: get\n  operationId: getExchangeRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verifications\n  method: post\n  operationId: createVerification\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verifications/{verification_id}\n  method: get\n  operationId: getVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verifications/{verification_id}/state\n  method: patch\n  operationId: updateVerificationState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verifications/{verification_id}/documents\n  method: get\n  operationId: getVerificationDocuments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verifications/{verification_id}/documents/{document_id}\n  method: patch\n  operationId: updateVerificationDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{payment_id}\n  method: get\n  operationId: retrievePayment\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{payment_id}/status\n  method: get\n  operationId: retrievePaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{payment_id}/cancel\n  method: post\n  operationId: cancelAlternativePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /secure_payments\n  method: post\n  operationId: createAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{authorization_id}/captures\n  method: post\n  operationId: captureAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{authorization_id}/cancel\n  method: post\n  operationId: cancelAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-methods\n  method: get\n  operationId: searchPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/v3\n  method: post\n  operationId: requestPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/v3/{payout_id}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/v3/{payout_id}/cancel\n  method: post\n  operationId: cancelPayout\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/v3/{payout_id}/release\n  method: post\n  operationId: releasePayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/v3/balance\n  method: get\n  operationId: getPayoutsBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/v3/quotes\n\
  \  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/update\n  method: patch\n\
  \  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/block\n  method: post\n  operationId: blockAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/unblock\n  method: post\n  operationId: unblockAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/cancel\n  method: post\n  operationId: cancelAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/balance\n  method: get\n  operationId: getAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/credentials\n  method: get\n  operationId: getAccountCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/kyc\n  method: get\n  operationId: getAccountKyc\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/bank-accounts\n  method: post\n  operationId: addBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/bank-accounts\n  method: get\n  operationId: getBankAccountList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/bank-accounts/{bank_account_id}\n  method: get\n  operationId: getBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/bank-accounts/{bank_account_id}\n\
  \  method: delete\n  operationId: disableBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/transfers\n  method: post\n  operationId: createTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transfers/{transfer_id}\n  method: get\n  operationId: getTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/transfers/{transfer_id}/cancel\n  method: post\n  operationId: cancelTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds/{refund_id}\n  method: get\n  operationId: retrieveRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /refunds/{refund_id}/status\n  method: get\n  operationId: retrieveRefundStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{payment_id}/refunds\n  method: get\n  operationId: retrieveOrderRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/agentic-access/d-local-agentic-access.yml
summary_line: 49 operations · 27 acting · 1 human-in-the-loop
tags:
- Payments
- Payouts
- EmergingMarkets
- LatAm
- Africa
- Asia
- FX
- Fintech
---
