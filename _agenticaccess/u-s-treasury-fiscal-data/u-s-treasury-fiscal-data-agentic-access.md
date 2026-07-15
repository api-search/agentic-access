---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: treasury-fiscal-data-api-openapi.yaml
  format: yaml
  label: Treasury Fiscal Data API
  slug: fiscal-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/u-s-treasury-fiscal-data/refs/heads/main/openapi/treasury-fiscal-data-api-openapi.yaml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: U S Treasury Fiscal Data Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'U.S. Treasury Fiscal Data exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: U.S. Treasury Fiscal Data
provider_slug: u-s-treasury-fiscal-data
slug: u-s-treasury-fiscal-data-agentic-access
source_filename: u-s-treasury-fiscal-data-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/treasury-fiscal-data-api-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/accounting/od/debt_to_penny\n  method: get\n  operationId: getDebtToPenny\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/od/rates_of_exchange\n  method: get\n  operationId: getRatesOfExchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounting/od/avg_interest_rates\n\
  \  method: get\n  operationId: getAvgInterestRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/dts/dts_table_1\n  method: get\n  operationId: getDailyTreasuryStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounting/mts/mts_table_4\n  method: get\n  operationId: getMonthlyTreasuryStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/od/redemption_tables\n  method: get\n  operationId: getSavingsBondRedemptionTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounting/od/interest_expense\n  method: get\n \
  \ operationId: getInterestExpenseDebt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/od/mspd_table_1\n  method: get\n  operationId: getPublicDebtBySecurityType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/od/gift_contributions\n  method: get\n  operationId: getGiftContributionsDebt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/u-s-treasury-fiscal-data/refs/heads/main/agentic-access/u-s-treasury-fiscal-data-agentic-access.yml
summary_line: 9 operations
tags:
- Federal Government
- Finance
- Treasury
- National Debt
- Exchange Rates
- Economics
---
