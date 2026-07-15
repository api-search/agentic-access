---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Connect API
  slug: mono-africa-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Financial Data API
  slug: mono-africa-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Investment Data API
  slug: mono-africa-investment-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Creditworthiness API
  slug: mono-africa-creditworthiness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono DirectPay API
  slug: mono-africa-directpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Lookup API
  slug: mono-africa-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mono Africa Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payments/initiate
operation_count: 19
overview: 'Mono exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 7 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mono
provider_slug: mono-africa
slug: mono-africa-agentic-access
source_filename: mono-africa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mono-africa-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 8\n    connected: 11\n  by_consequence:\n    write: 7\n    read: 11\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/accounts/initiate\n  method: post\n  operationId: initiateAccountLinking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/auth\n  method: post\n  operationId: exchangeToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}\n  method: get\n  operationId: getAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/identity\n  method: get\n  operationId: getIdentity\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/income\n  method: get\n  operationId: getIncome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/statement\n  method: get\n  operationId: getStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/unlink\n  method: post\n  operationId: unlinkAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{id}/creditworthiness\n  method: post\n  operationId: assessCreditworthiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{id}/assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}/earnings\n  method: get\n  operationId: getEarnings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/payments/initiate\n  method: post\n  operationId: initiatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/payments/verify/{reference}\n  method: get\n  operationId: verifyPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/payments\n  method: get\n  operationId: getPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/lookup/bvn/initiate\n  method: post\n  operationId: lookupBvnInitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/lookup/account-number\n  method: post\n  operationId: lookupAccountNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/lookup/mashup\n  method: post\n  operationId: lookupMashup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/agentic-access/mono-africa-agentic-access.yml
summary_line: 19 operations · 8 acting
tags:
- Open Banking
- Financial Data
- Payments
- Fintech
- Account Linking
- Direct Debit
- Bank Data
- Africa
- Nigeria
- Financial Infrastructure
---
