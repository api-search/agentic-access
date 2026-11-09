---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: swift-payment-pre-validation-api-openapi.yml
  format: yaml
  label: Payment Pre-validation API
  slug: payment-pre-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-payment-pre-validation-api-openapi.yml
- filename: swift-account-numbers-api-openapi.yml
  format: yaml
  label: SWIFT Account Numbers API
  slug: swift-account-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-account-numbers-api-openapi.yml
- filename: swift-bbans-api-openapi.yml
  format: yaml
  label: SWIFT BBANs API
  slug: swift-bbans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-bbans-api-openapi.yml
- filename: swift-bics-api-openapi.yml
  format: yaml
  label: SWIFT BICs API
  slug: swift-bics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-bics-api-openapi.yml
- filename: swift-country-codes-api-openapi.yml
  format: yaml
  label: SWIFT Country Codes API
  slug: swift-country-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-country-codes-api-openapi.yml
- filename: swift-currency-codes-api-openapi.yml
  format: yaml
  label: SWIFT Currency Codes API
  slug: swift-currency-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-currency-codes-api-openapi.yml
- filename: swift-leis-api-openapi.yml
  format: yaml
  label: SWIFT LEIs API
  slug: swift-leis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-leis-api-openapi.yml
- filename: swift-national-ids-api-openapi.yml
  format: yaml
  label: SWIFT National IDs API
  slug: swift-national-ids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-national-ids-api-openapi.yml
- filename: swift-ibans-api-openapi.yml
  format: yaml
  label: SWIFT IBANs API
  slug: swift-ibans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-ibans-api-openapi.yml
- filename: swift-account-information-api-openapi.yml
  format: yaml
  label: SWIFT Account Information API
  slug: swift-account-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-account-information-api-openapi.yml
- filename: swift-distributions-api-openapi.yml
  format: yaml
  label: SWIFT Distributions API
  slug: swift-distributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-distributions-api-openapi.yml
- filename: swift-fileact-api-openapi.yml
  format: yaml
  label: SWIFT Fileact API
  slug: swift-fileact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-fileact-api-openapi.yml
- filename: swift-fin-api-openapi.yml
  format: yaml
  label: SWIFT Fin API
  slug: swift-fin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-fin-api-openapi.yml
- filename: swift-get-changed-payment-transactions-api-openapi.yml
  format: yaml
  label: SWIFT Get Changed Payment Transactions API
  slug: swift-get-changed-payment-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-get-changed-payment-transactions-api-openapi.yml
- filename: swift-get-payment-transaction-details-api-openapi.yml
  format: yaml
  label: SWIFT Get Payment Transaction Details API
  slug: swift-get-payment-transaction-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-get-payment-transaction-details-api-openapi.yml
- filename: swift-iban-national-ids-api-openapi.yml
  format: yaml
  label: SWIFT Iban National IDs API
  slug: swift-iban-national-ids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-iban-national-ids-api-openapi.yml
- filename: swift-interact-api-openapi.yml
  format: yaml
  label: SWIFT Interact API
  slug: swift-interact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-interact-api-openapi.yml
- filename: swift-pmis-api-openapi.yml
  format: yaml
  label: SWIFT Pmis API
  slug: swift-pmis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-pmis-api-openapi.yml
- filename: swift-reporting-api-openapi.yml
  format: yaml
  label: SWIFT Reporting API
  slug: swift-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-reporting-api-openapi.yml
- filename: swift-status-confirmations-api-openapi.yml
  format: yaml
  label: SWIFT Status Confirmations API
  slug: swift-status-confirmations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-status-confirmations-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Swift Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'SWIFT exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SWIFT
provider_slug: swift
slug: swift-agentic-access
source_filename: swift-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/swift-swiftref-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/bics/{bic}\n  method: get\n  operationId: getBic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bics/{bic}/validity\n  method: get\n  operationId: validateBic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bics/{bic}/lei\n  method: get\n  operationId: getBicLei\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bics/{bic}/national_ids\n  method: get\n  operationId: getBicNationalIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bics/{bic}/reachability\n  method: get\n  operationId: getBicSepaReachability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bics/{bic}/ssis\n  method: get\n  operationId: getBicSsis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ibans/{iban}\n  method: get\n  operationId: getIban\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/ibans/{iban}/validity\n  method: get\n  operationId: validateIban\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ibans/{iban}/bic\n  method: get\n  operationId: getBicForIban\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bbans/{bban}/iban\n  method: get\n  operationId: getIbanForBban\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/leis/{lei}\n  method: get\n  operationId: getLei\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/leis/{lei}/validity\n  method: get\n  operationId: validateLei\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/leis/{lei}/bic\n  method: get\n  operationId: getBicForLei\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/national_ids/{national_id}\n  method: get\n  operationId: getNationalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/national_ids/{national_id}/validity\n  method: get\n  operationId: validateNationalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/national_ids/{national_id}/bics\n  method: get\n  operationId: getBicsForNationalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/iban_national_ids/{iban_national_id}/bic\n  method: get\n  operationId: getBicForIbanNationalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/country_codes/{country_code}\n  method: get\n  operationId: getCountryCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/country_codes/{country_code}/validity\n  method: get\n  operationId: validateCountryCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/currency_codes/{currency_code}\n  method: get\n  operationId: getCurrencyCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v2/currency_codes/{currency_code}/validity\n  method: get\n  operationId: validateCurrencyCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account_numbers/{account_number}/validity\n  method: get\n  operationId: validateAccountNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/swift/agentic-access/swift-agentic-access.yml
summary_line: 22 operations
tags:
- Banking
- Cross-Border Payments
- Financial Messaging
- Financial Services
- GPI
- ISO 20022
- Payments
- SWIFT
---
