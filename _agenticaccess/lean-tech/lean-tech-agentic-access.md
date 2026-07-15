---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 37
api_specs:
- filename: lean-authentication-api-openapi.yml
  format: yaml
  label: Lean Authentication API
  slug: lean-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-authentication-api-openapi.yml
- filename: lean-customers-api-openapi.yml
  format: yaml
  label: Lean Customers API
  slug: lean-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-customers-api-openapi.yml
- filename: lean-entities-api-openapi.yml
  format: yaml
  label: Lean Entities API
  slug: lean-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-entities-api-openapi.yml
- filename: lean-data-api-openapi.yml
  format: yaml
  label: Lean Data API
  slug: lean-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-data-api-openapi.yml
- filename: lean-insights-api-openapi.yml
  format: yaml
  label: Lean Insights API
  slug: lean-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-insights-api-openapi.yml
- filename: lean-banks-api-openapi.yml
  format: yaml
  label: Lean Banks API
  slug: lean-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-banks-api-openapi.yml
- filename: lean-verifications-api-openapi.yml
  format: yaml
  label: Lean Verifications API
  slug: lean-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-verifications-api-openapi.yml
- filename: lean-payments-api-openapi.yml
  format: yaml
  label: Lean Payments API
  slug: lean-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-payments-api-openapi.yml
- filename: lean-payment-sources-api-openapi.yml
  format: yaml
  label: Lean Payment Sources API
  slug: lean-payment-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-payment-sources-api-openapi.yml
- filename: lean-payouts-api-openapi.yml
  format: yaml
  label: Lean Payouts API
  slug: lean-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-payouts-api-openapi.yml
- filename: lean-refunds-api-openapi.yml
  format: yaml
  label: Lean Refunds API
  slug: lean-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-refunds-api-openapi.yml
consequence_counts:
  physical: 7
  read: 37
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lean Tech Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /customers/v1/{customer_id}/payment-sources/{payment_source_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/account-on-file
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payouts/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/payment/destinations
operation_count: 51
overview: 'Lean Technologies exposes 51 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 7 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lean Technologies
provider_slug: lean-tech
slug: lean-tech-agentic-access
source_filename: lean-tech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lean-authentication-api-openapi.yml, openapi/lean-banks-api-openapi.yml, openapi/lean-customers-api-openapi.yml,\n  openapi/lean-data-api-openapi.yml, openapi/lean-entities-api-openapi.yml, openapi/lean-insights-api-openapi.yml,\n  openapi/lean-payment-sources-api-openapi.yml, openapi/lean-payments-api-openapi.yml, openapi/lean-payouts-api-openapi.yml,\n  openapi/lean-refunds-api-openapi.yml, openapi/lean-verifications-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    acting: 14\n    connected: 37\n  by_consequence:\n    write: 7\n    read: 37\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth2/token\n  method: post\n\
  \  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banks/v1/\n  method: get\n  operationId: listBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}\n  method: get\n  operationId: getCustomerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/app-user-id/{app_user_id}\n  method: get\n  operationId: getCustomerByAppUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /data/v2/accounts/{account_id}/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/beneficiaries\n  method: get\n  operationId: getBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/direct-debits\n  method: get\n  operationId: getDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/scheduled-payments\n  method: get\n  operationId: getScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /data/v2/accounts/{account_id}/standing-orders\n  method: get\n  operationId: getStandingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/identities\n  method: get\n  operationId: getAccountIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/identity\n  method: get\n  operationId: getIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/refreshes\n  method: post\n  operationId: triggerDataRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v2/refreshes\n  method: get\n  operationId: getDataRefreshes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/refreshes/{refresh_id}\n  method: get\n  operationId: getDataRefreshStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities\n  method: get\n  operationId: getEntitiesForCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: get\n  operationId: getEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /customers/v1/entities\n  method: get\n  operationId: retrieveEntitiesForDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/income\n  method: post\n  operationId: computeIncome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v2/expenses\n  method: get\n  operationId: getExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/assets/cashflows\n  method: get\n  operationId: getCashflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/payment-sources\n  method: get\n  operationId: listCustomerPaymentSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/payment-sources/{payment_source_id}\n  method: get\n  operationId: getPaymentSourceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/payment-sources/{payment_source_id}\n  method: delete\n  operationId: deletePaymentSource\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/intents\n  method: post\n  operationId: createPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/intents\n  method: get\n  operationId: listPaymentIntents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/v1/intents/{intent_id}\n  method: get\n  operationId: getPaymentByIntentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/v1/{payment_id}\n  method: get\n  operationId:\
  \ getPaymentByPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/account-on-file\n  method: post\n  operationId: initiateAofPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consents/account-on-file\n  method: post\n  operationId: createAofConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consents/v1\n  method: get\n  operationId:\
  \ listCustomerConsents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/{consent_id}\n  method: get\n  operationId: getConsentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/{consent_id}/balance\n  method: get\n  operationId: fetchConsentBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/{consent_id}/history\n  method: get\n  operationId: getConsentHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/v1/payment\n  method: post\n  operationId: createPayoutPayment\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/v1/payments\n  method: get\n  operationId: listPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/v1/payments/{payment_id}/history\n  method: get\n  operationId: getPayoutPaymentHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/v1/{payment_id}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/v1/intents/{payment_intent_id}\n\
  \  method: get\n  operationId: getPayoutIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/v1/payment/destinations\n  method: post\n  operationId: createPayoutDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/v1/payment/destinations\n  method: get\n  operationId: listPayoutDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/v1/payment/destinations/{destination_id}\n  method: get\n  operationId: getPayoutDestination\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/refunds\n  method: put\n  operationId: processRefunds\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/refunds/reasons\n  method: get\n  operationId: getRefundReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verifications/v1/accounts\n  method: post\n  operationId: verifyAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v1/name-verification\n  method: post\n  operationId: verifyName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/agentic-access/lean-tech-agentic-access.yml
summary_line: 51 operations · 14 acting
tags:
- Open Banking
- Open Finance
- MENA
- UAE
- Saudi Arabia
- Payments
- Pay by Bank
- A2A
- Account Information
- Payment Initiation
- Verifications
- Identity
- Fintech
---
