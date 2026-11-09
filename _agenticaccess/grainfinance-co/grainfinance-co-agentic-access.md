---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 19
api_specs:
- filename: grainfinance-co-conversions-api-openapi.yml
  format: yaml
  label: Grain Conversions API
  slug: grainfinance-co-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-conversions-api-openapi.yml
- filename: grainfinance-co-customers-api-openapi.yml
  format: yaml
  label: Grain Customers API
  slug: grainfinance-co-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-customers-api-openapi.yml
- filename: grainfinance-co-dual-hedges-api-openapi.yml
  format: yaml
  label: Grain Dual Hedges API
  slug: grainfinance-co-dual-hedges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-dual-hedges-api-openapi.yml
- filename: grainfinance-co-grain-api-api-openapi.yml
  format: yaml
  label: Grain Grain API
  slug: grainfinance-co-grain-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-grain-api-api-openapi.yml
- filename: grainfinance-co-hedges-api-openapi.yml
  format: yaml
  label: Grain Hedges API
  slug: grainfinance-co-hedges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-hedges-api-openapi.yml
- filename: grainfinance-co-payouts-api-openapi.yml
  format: yaml
  label: Grain Payouts API
  slug: grainfinance-co-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-payouts-api-openapi.yml
- filename: grainfinance-co-pricing-api-openapi.yml
  format: yaml
  label: Grain Pricing API
  slug: grainfinance-co-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-pricing-api-openapi.yml
- filename: grainfinance-co-vendors-api-openapi.yml
  format: yaml
  label: Grain Vendors API
  slug: grainfinance-co-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-vendors-api-openapi.yml
- filename: grainfinance-co-wallets-api-openapi.yml
  format: yaml
  label: Grain Wallets API
  slug: grainfinance-co-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grainfinance-co/openapi/grainfinance-co-wallets-api-openapi.yml
consequence_counts:
  physical: 3
  read: 19
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Grainfinance Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/{proposalId}/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wallets/{walletId}/withdraw
operation_count: 36
overview: 'Grain exposes 36 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 14 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Grain
provider_slug: grainfinance-co
slug: grainfinance-co-agentic-access
source_filename: grainfinance-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: generated\nsource: openapi/grainfinance-co-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 17\n    connected: 19\n  by_consequence:\n    write: 14\n    read: 19\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /conversions/quote\n  method: post\n  operationId: Quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversions/accept-quote\n  method: post\n  operationId: Accept\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversions/{conversionId}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversions\n  method: get\n  operationId: List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /customers\n  method: get\n  operationId: List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/update\n  method: post\n  operationId: Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: delete\n  operationId: Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/dual-hedges/accept-offline-quote\n  method: post\n  operationId: Offline Accept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/dual-hedges/{dualHedgeId}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/dual-hedges/{dualHedgeId}/cancel\n  method: post\n  operationId: Cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/dual-hedges\n  method: get\n  operationId: List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/hedges/{hedgeId}/drawdown/quote\n  method: post\n  operationId: Drawdown Quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/hedges/{hedgeId}/drawdown/accept\n  method: post\n  operationId: Drawdown Accept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/hedges/{hedgeId}/drawdown/{drawdownId}\n  method: get\n  operationId: Get Drawdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/hedges/{hedgeId}/drawdown\n  method: get\n  operationId: List Drawdowns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/hedges/quote\n  method: post\n  operationId: Real-time Quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /customers/{customerId}/hedges/accept-quote\n  method: post\n  operationId: Real-time Accept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/hedges/accept-offline-quote\n  method: post\n  operationId: Offline Accept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/hedges/{hedgeId}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /customers/{customerId}/hedges/{hedgeId}/cancel\n  method: post\n  operationId: Cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/hedges\n  method: get\n  operationId: List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dual-hedge-offline-rates\n  method: get\n  operationId: Offline Quotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offline-rates\n  method: get\n  operationId: Offline Quotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts\n  method: post\n  operationId: Review\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts\n  method: get\n  operationId: List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/{proposalId}/submit\n  method: post\n  operationId: Submit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /payouts/{payoutId}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rates/currency-pairs-exchange-rate\n  method: get\n  operationId: Rate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendors/{vendorId}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendors\n  method: post\n  operationId: Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /vendors\n  method: get\n  operationId: List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets\n  method: get\n  operationId: List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{walletId}\n  method: get\n  operationId: Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{walletId}/withdraw\n  method: post\n  operationId: Withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/grainfinance-co/agentic-access/grainfinance-co-agentic-access.yml
summary_line: 36 operations · 17 acting
tags:
- Fintech
- Payments
- Currency
- Embedded
---
