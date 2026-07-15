---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 13
api_specs:
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Collections API
  slug: fincra-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Payouts / Disbursements API
  slug: fincra-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Conversions / FX API
  slug: fincra-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Quotes API
  slug: fincra-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Beneficiaries API
  slug: fincra-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Virtual Accounts API
  slug: fincra-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Banks & Account Resolution API
  slug: fincra-banks-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
- filename: fincra-openapi.yml
  format: yaml
  label: Fincra Webhooks
  slug: fincra-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/openapi/fincra-openapi.yml
consequence_counts:
  physical: 3
  read: 13
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fincra Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/charges/authorize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /disbursements/payouts
operation_count: 23
overview: 'Fincra exposes 23 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 7 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fincra
provider_slug: fincra
slug: fincra-agentic-access
source_filename: fincra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fincra-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 10\n    connected: 13\n  by_consequence:\n    physical: 3\n    read: 13\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /checkout/charges\n  method: post\n  operationId: initiateCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/charges/authorize\n  method: post\n\
  \  operationId: authorizeCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/charges/{reference}\n  method: get\n  operationId: getChargeByReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/charges/verify/{reference}\n  method: get\n  operationId: verifyCharge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disbursements/payouts\n  method: post\n  operationId: initiatePayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disbursements/payouts\n  method: get\n  operationId: getAllPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disbursements/payouts/reference/{transactionReference}\n  method: get\n  operationId: verifyPayoutByReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disbursements/payouts/customer-reference/{customerReference}\n  method: get\n  operationId: verifyPayoutByCustomerReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /quotes/generate\n  method: post\n  operationId: generateQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversions/initiate\n  method: post\n  operationId: initiateConversion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversions\n  method: get\n  operationId: listConversions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversions/{reference}\n  method: get\n  operationId:\
  \ verifyConversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/beneficiaries/business/{businessId}\n  method: post\n  operationId: createBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/beneficiaries/business/{businessId}\n  method: get\n  operationId: listBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/beneficiaries/business/{businessId}/{beneficiaryId}\n  method: get\n  operationId: fetchBeneficiary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/beneficiaries/business/{businessId}/{beneficiaryId}\n  method: patch\n  operationId: updateBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/beneficiaries/business/{businessId}/{beneficiaryId}\n  method: delete\n  operationId: deleteBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/virtual-accounts/requests\n  method: post\n  operationId: requestVirtualAccount\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/virtual-accounts/business\n  method: get\n  operationId: listVirtualAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/virtual-accounts/{virtualAccountId}\n  method: get\n  operationId: fetchVirtualAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/virtual-accounts/{virtualAccountId}/payins\n  method: get\n  operationId: listVirtualAccountPayins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/banks\n\
  \  method: get\n  operationId: listBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/accounts/resolve\n  method: post\n  operationId: resolveAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fincra/refs/heads/main/agentic-access/fincra-agentic-access.yml
summary_line: 23 operations · 10 acting
tags:
- Payments
- Cross-Border
- Collections
- Payouts
- FX
- Fintech
- Africa
---
