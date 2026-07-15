---
acting_count: 69
action_class_counts:
  acting: 69
  connected: 28
api_specs:
- filename: openapi
  format: yaml
  label: Worldpay Card Payments API
  slug: worldpay-card-payments-api
  spec_type: OpenAPI
  url: https://docs.worldpay.com/access/products/payments/openapi
- filename: openapi
  format: yaml
  label: Worldpay Payment Queries API
  slug: worldpay-payment-queries-api
  spec_type: OpenAPI
  url: https://developer.worldpay.com/products/access/payment-queries/openapi
consequence_counts:
  physical: 42
  read: 28
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Worldpay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accountPayouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accountPayouts/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{linkData}/3dsChallenges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{linkData}/3dsDeviceData
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{linkData}/cancellations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{linkData}/partialRefunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{linkData}/partialSettlements
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{linkData}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{linkData}/reversals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{linkData}/settlements
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apmPayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apmPayments/{paymentId}/confirmations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apmPayments/{paymentId}/partialReversals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apmPayments/{paymentId}/partialSettlements
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apmPayments/{paymentId}/reversals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apmPayments/{paymentId}/settlements
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cardPayments/customerInitiatedTransactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cardPayments/merchantInitiatedTransactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fraudsight/update/chargeback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fraudsight/update/fraud
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fraudsight/update/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /moneyTransfers/pushToCard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /parties/{partyId}/payoutInstruments
operation_count: 97
overview: 'Worldpay exposes 97 API operations that an AI agent could call, of which 69 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 27 write, and 42 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Worldpay
provider_slug: worldpay
slug: worldpay-agentic-access
source_filename: worldpay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/worldpay-3ds-openapi.yaml, openapi/worldpay-account-payouts-openapi.yaml, openapi/worldpay-apms-openapi.yaml,\n  openapi/worldpay-balance-openapi.yaml, openapi/worldpay-card-payments-openapi.yaml, openapi/worldpay-card-payouts-openapi.yaml,\n  openapi/worldpay-card-verifications-openapi.yaml, openapi/worldpay-fraudsight-openapi.yaml,\n  openapi/worldpay-fx-openapi.yaml, openapi/worldpay-hosted-payment-pages-openapi.yaml, openapi/worldpay-money-transfers-openapi.yaml,\n  openapi/worldpay-parties-openapi.yaml, openapi/worldpay-payment-queries-openapi.yaml, openapi/worldpay-payments-openapi.yaml,\n  openapi/worldpay-sca-exemptions-openapi.yaml, openapi/worldpay-split-payments-openapi.yaml,\n  openapi/worldpay-statements-openapi.yaml, openapi/worldpay-tokens-openapi.yaml, openapi/worldpay-transfers-openapi.yaml,\n  openapi/worldpay-verified-tokens-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts,\
  \ classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 97\n  by_action_class:\n    acting: 69\n    connected: 28\n  by_consequence:\n    write: 27\n    physical: 42\n    read: 28\n  human_in_the_loop_required: 0\noperations:\n- path: /verifications/customers/3ds/deviceDataInitialization\n  method: post\n  operationId: deviceDataInitialize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verifications/customers/3ds/authentication\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verifications/customers/3ds/verification\n  method: post\n  operationId: verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accountPayouts\n  method: post\n  operationId: PostPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accountPayouts/batch\n  method: post\n  operationId: PostBatchPayout\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accountPayouts/{payoutRequestId}\n  method: get\n  operationId: GetByPayoutRequestId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountPayouts/events\n  method: get\n  operationId: GetByQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apmPayments\n  method: post\n  operationId: payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apmPayments/status\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apmPayments/{paymentId}\n  method: get\n  operationId: query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apmPayments/{paymentId}/confirmations\n  method: post\n  operationId: confirmPaymentV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /apmPayments/{paymentId}/reversals\n  method: post\n  operationId: reverse\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apmPayments/{paymentId}/partialReversals\n  method: post\n  operationId: partialReverseV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apmPayments/{paymentId}/settlements\n  method: post\n  operationId: settle\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apmPayments/{paymentId}/partialSettlements\n  method: post\n  operationId: settleV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountNumber}\n  method: get\n  operationId: ReceiveTransferRequestForAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n\
  \  method: get\n  operationId: ReceiveTransferRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardPayments/customerInitiatedTransactions\n  method: post\n  operationId: authorize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardPayments/merchantInitiatedTransactions\n  method: post\n  operationId: recurring\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /payments/settlements/{linkData}\n  method: post\n  operationId: settle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/settlements/partials/{linkData}\n  method: post\n  operationId: partialSettlement\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/settlements/refunds/full/{linkData}\n  method: post\n  operationId: refund\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/settlements/refunds/partials/{linkData}\n  method: post\n  operationId: partialRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/authorizations/cancellations/{linkData}\n  method: post\n  operationId: cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n   \
  \   exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/authorizations/cancellations/partials/{linkData}\n  method: post\n  operationId: partialCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/authorizations/incrementalAuthorizations/{linkData}\n  method: post\n  operationId: increaseAuthorize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/sales/reversals/{linkData}\n  method: post\n  operationId: reversal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/events/{linkData}\n  method: get\n  operationId: eventQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/events\n  method: get\n  operationId: eventRecovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/{resource}\n  method: get\n  operationId: getPayoutsDetails\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/query\n  method: get\n  operationId: queryPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/basicDisbursement\n  method: post\n  operationId: basicDisbursement\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/fastAccess\n  method: post\n  operationId: fastAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardVerifications\n  method: post\n  operationId: cardVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /achVerifications\n  method: post\n  operationId: ACH\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardVerifications/{linkData}\n  method: get\n  operationId: getCardVerificationByResourceId\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fraudsight/assessment\n  method: post\n  operationId: assessment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fraudsight/update/payment\n  method: post\n  operationId: updatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fraudsight/update/fraud\n  method: post\n  operationId: updateFraud\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fraudsight/update/chargeback\n  method: post\n  operationId: updateChargeback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /foreignExchange/rates\n  method: get\n  operationId: getFXrates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foreignExchange/quote\n  method: post\n  operationId: postFXquote\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /foreignExchange/quote\n  method: get\n  operationId: getFXquote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foreignExchange/contract\n  method: post\n  operationId: postContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /foreignExchange/contract/{contractId}\n  method: put\n  operationId: putContract\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /foreignExchange/markup/{entity}\n  method: put\n  operationId: addMarkup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /foreignExchange/markup/{entity}\n  method: get\n  operationId: getMarkup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_pages\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /moneyTransfers/pushToCard\n  method: post\n  operationId: pushToCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /moneyTransfers/query\n  method: get\n  operationId: query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parties\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parties\n  method: get\n  operationId: browseParties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parties/{partyId}\n  method: get\n  operationId: partyQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parties/{partyId}\n  method: put\n  operationId: updateParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parties/{partyId}/deactivation\n  method: post\n  operationId:\
  \ deactivateParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parties/{partyId}/activation\n  method: post\n  operationId: reactivateParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parties/{partyId}/balanceAccounts\n  method: post\n  operationId: createBalanceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /parties/{partyId}/balanceAccounts/{balanceAccountId}\n  method: get\n  operationId: getBalanceAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parties/{partyId}/balanceAccounts/{balanceAccountId}\n  method: put\n  operationId: updateBalanceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parties/{partyId}/beneficialOwners\n  method: post\n  operationId: createBeneficialOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /parties/{partyId}/beneficialOwners/{beneficialOwnerId}\n  method: get\n  operationId: getBeneficialOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parties/{partyId}/beneficialOwners/{beneficialOwnerId}\n  method: put\n  operationId: updateBeneficialOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parties/{partyId}/beneficialOwners/{beneficialOwnerId}\n  method: delete\n  operationId: deleteBeneficialOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parties/{partyId}/identityVerification\n  method: post\n  operationId: performIdentityVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parties/{partyId}/identityVerification\n  method: get\n  operationId: getIdentityVerificationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parties/{partyId}/payoutInstruments\n  method: post\n  operationId: createPayoutInstruments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parties/{partyId}/payoutInstruments/{payoutInstrumentId}\n  method: get\n  operationId: getPayoutInstrument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parties/{partyId}/payoutInstruments/{payoutInstrumentId}\n  method: put\n  operationId: updatePayoutInstruments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentQueries/payments\n  method: get\n  operationId: queryByDateRange\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentQueries/payments/{paymentId}\n  method: get\n  operationId: retrieveByPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentQueries/archivedPayments\n  method: get\n  operationId: queryArchivedPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments/{linkData}\n  method: get\n  operationId: queryEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments/{linkData}/settlements\n  method: post\n  operationId: settle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{linkData}/partialSettlements\n  method: post\n  operationId: partialSettle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{linkData}/refunds\n  method: post\n  operationId: refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{linkData}/partialRefunds\n  method: post\n  operationId: partialRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{linkData}/cancellations\n  method: post\n  operationId: cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments\n  method: post\n  operationId: payment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{linkData}/reversals\n  method: post\n  operationId: reversal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{linkData}/3dsDeviceData\n  method: post\n  operationId: supply3dsDeviceData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{linkData}/3dsChallenges\n  method: post\n  operationId: complete3dsChallenge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exemptions/assessment\n  method: post\n  operationId: assessment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /splitPayments\n  method:\
  \ post\n  operationId: splitPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /splitPayments/{splitPaymentId}/fulfillments\n  method: post\n  operationId: fullCaptureFulfillments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /splitPayments/{splitPaymentId}/items/{itemId}/fulfillments\n  method: post\n  operationId: singItemCaptureFulfillments\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/statements\n  method: get\n  operationId: GetStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens\n  method: post\n  operationId: createSecurityToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/{tokenId}\n  method: get\n  operationId: getSecurityToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{tokenId}\n  method: put\n  operationId: updateSecurityToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/{tokenId}\n  method: delete\n  operationId: deleteSecurityToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/network\n  method: post\n  operationId: provisionNetworkToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/network/{id}\n  method: get\n  operationId: getNetworkToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/network/{id}\n  method: delete\n  operationId: deleteSecurityNetworkToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/network/cryptograms\n  method: post\n  operationId: getNetworkTokenCryptogram\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      trig\n\n# --- truncated at 32 KB (33 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/worldpay/refs/heads/main/agentic-access/worldpay-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldpay/refs/heads/main/agentic-access/worldpay-agentic-access.yml
summary_line: 97 operations · 69 acting
tags:
- Payments
- Payment Processing
- Payment Gateway
- Tokenization
- Fraud Prevention
- Recurring Billing
- Payouts
- Foreign Exchange
- Financial Services
- Fintech
---
