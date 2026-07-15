---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: fiscaldata-openapi.yml
  format: yaml
  label: Treasury Debt API
  slug: fiscaldata-debt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscaldata/refs/heads/main/openapi/fiscaldata-openapi.yml
- filename: fiscaldata-openapi.yml
  format: yaml
  label: Average Interest Rates API
  slug: fiscaldata-average-interest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscaldata/refs/heads/main/openapi/fiscaldata-openapi.yml
- filename: fiscaldata-openapi.yml
  format: yaml
  label: Daily Treasury Statement API
  slug: fiscaldata-daily-treasury-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscaldata/refs/heads/main/openapi/fiscaldata-openapi.yml
- filename: fiscaldata-openapi.yml
  format: yaml
  label: Monthly Treasury Statement API
  slug: fiscaldata-monthly-treasury-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscaldata/refs/heads/main/openapi/fiscaldata-openapi.yml
- filename: fiscaldata-openapi.yml
  format: yaml
  label: Treasury Reporting Rates of Exchange API
  slug: fiscaldata-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscaldata/refs/heads/main/openapi/fiscaldata-openapi.yml
- filename: fiscaldata-openapi.yml
  format: yaml
  label: Treasury Securities API
  slug: fiscaldata-securities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscaldata/refs/heads/main/openapi/fiscaldata-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fiscaldata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'U.S. Treasury Fiscal Data exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: U.S. Treasury Fiscal Data
provider_slug: fiscaldata
slug: fiscaldata-agentic-access
source_filename: fiscaldata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fiscaldata-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/accounting/od/debt_to_penny\n  method: get\n  operationId: getDebtToPenny\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounting/od/interest_expense\n  method: get\n  operationId: getInterestExpense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounting/od/avg_interest_rates\n\
  \  method: get\n  operationId: getAverageInterestRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/dts/operating_cash_balance\n  method: get\n  operationId: getOperatingCashBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/dts/deposits_withdrawals_operating_cash\n  method: get\n  operationId: getDepositsWithdrawalsOperatingCash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/mts/mts_table_4\n  method: get\n  operationId: getMtsReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/mts/mts_table_5\n\
  \  method: get\n  operationId: getMtsOutlays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/od/rates_of_exchange\n  method: get\n  operationId: getRatesOfExchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/od/auctions_query\n  method: get\n  operationId: getAuctionsQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiscaldata/refs/heads/main/agentic-access/fiscaldata-agentic-access.yml
summary_line: 9 operations
tags:
- Government Data
- Treasury
- Economic Indicators
- Interest Rates
- Open Data
- National Debt
- Government Reports
- Public Domain
- Federal Finance
---
