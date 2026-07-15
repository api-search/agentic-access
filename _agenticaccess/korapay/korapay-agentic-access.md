---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 15
api_specs:
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Charges API
  slug: korapay-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Payouts API
  slug: korapay-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Virtual Bank Accounts API
  slug: korapay-virtual-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Balances API
  slug: korapay-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Refunds API
  slug: korapay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Currency Conversion API
  slug: korapay-currency-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Misc Utilities API
  slug: korapay-misc-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
consequence_counts:
  physical: 10
  read: 15
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Korapay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge/pay-with-bank
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charges/card
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charges/card/authorize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charges/initialize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charges/mobile-money
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charges/mobile-money/authorize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refunds/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/disburse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/disburse/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/disburse/remittance
operation_count: 30
overview: 'Kora exposes 30 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 5 write, and 10 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kora
provider_slug: korapay
slug: korapay-agentic-access
source_filename: korapay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/korapay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 15\n    connected: 15\n  by_consequence:\n    physical: 10\n    read: 15\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /charges/initialize\n  method: post\n  operationId: initializeCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charges/card\n  method: post\n  operationId:\
  \ chargeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charges/card/authorize\n  method: post\n  operationId: authorizeCardCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charges/mobile-money\n  method: post\n  operationId: chargeMobileMoney\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charges/mobile-money/authorize\n  method: post\n  operationId: authorizeMobileMoneyCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charge/pay-with-bank\n  method: post\n  operationId: chargePayWithBank\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /charge/pay-with-bank/banks\n  method: get\n  operationId: listPayWithBankBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charges/{reference}\n  method: get\n  operationId: verifyCharge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/disburse\n  method: post\n  operationId: createPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/disburse/bulk\n  method: post\n  operationId: createBulkPayout\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/disburse/remittance\n  method: post\n  operationId: createRemittancePayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts\n  method: get\n  operationId: listPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/availability\n  method: get\n  operationId: getPayoutAvailability\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /virtual-bank-account\n  method: post\n  operationId: createVirtualBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virtual-bank-account/transactions\n  method: get\n  operationId: listVirtualBankAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /virtual-bank-account/{accountReference}\n  method: get\n  operationId: getVirtualBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds/initiate\n  method: post\n  operationId: initiateRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds/{reference}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversions/rates\n  method: post\n  operationId: getExchangeRate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversions\n  method: post\n  operationId: initiateConversion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversions\n  method: get\n  operationId: listConversions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversions/{reference}\n\
  \  method: get\n  operationId: getConversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/banks\n  method: get\n  operationId: listBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/banks/resolve\n  method: post\n  operationId: resolveBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /misc/mobile-money\n  method: get\n  operationId: listMobileMoneyOperators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/mobile-money/resolve\n\
  \  method: post\n  operationId: resolveMobileMoney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /misc/payout-payment-purpose-by-country-code/{countryCode}\n  method: get\n  operationId: getPayoutPaymentPurpose\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/payout-countries-by-currency-code/{currencyCode}\n  method: get\n  operationId: getPayoutCountriesByCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/agentic-access/korapay-agentic-access.yml
summary_line: 30 operations · 15 acting
tags:
- Payments
- Payment Gateway
- Africa
- Nigeria
- Collections
- Payouts
- Disbursements
- Virtual Bank Account
- Cards
- Fintech
---
