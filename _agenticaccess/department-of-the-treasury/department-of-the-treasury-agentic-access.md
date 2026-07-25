---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: department-of-the-treasury-auctions-api-openapi.yml
  format: yaml
  label: Department of the Treasury Auctions API
  slug: department-of-the-treasury-auctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-auctions-api-openapi.yml
- filename: department-of-the-treasury-debt-api-openapi.yml
  format: yaml
  label: Department of the Treasury Debt API
  slug: department-of-the-treasury-debt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-debt-api-openapi.yml
- filename: department-of-the-treasury-exchange-rates-api-openapi.yml
  format: yaml
  label: Department of the Treasury Exchange Rates API
  slug: department-of-the-treasury-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-exchange-rates-api-openapi.yml
- filename: department-of-the-treasury-interest-rates-api-openapi.yml
  format: yaml
  label: Department of the Treasury Interest Rates API
  slug: department-of-the-treasury-interest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-interest-rates-api-openapi.yml
- filename: department-of-the-treasury-sanctions-lists-api-openapi.yml
  format: yaml
  label: Department of the Treasury Sanctions Lists API
  slug: department-of-the-treasury-sanctions-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-sanctions-lists-api-openapi.yml
- filename: department-of-the-treasury-search-api-openapi.yml
  format: yaml
  label: Department of the Treasury Search API
  slug: department-of-the-treasury-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-search-api-openapi.yml
- filename: department-of-the-treasury-spending-api-openapi.yml
  format: yaml
  label: Department of the Treasury Spending API
  slug: department-of-the-treasury-spending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-spending-api-openapi.yml
- filename: department-of-the-treasury-treasury-operations-api-openapi.yml
  format: yaml
  label: Department of the Treasury Treasury Operations API
  slug: department-of-the-treasury-treasury-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/openapi/department-of-the-treasury-treasury-operations-api-openapi.yml
consequence_counts:
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Department Of The Treasury Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Department of the Treasury exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Department of the Treasury
provider_slug: department-of-the-treasury
slug: department-of-the-treasury-agentic-access
source_filename: department-of-the-treasury-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fiscal-data-api-openapi.yml, openapi/ofac-sdn-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 9\n    acting: 1\n  by_consequence:\n    read: 9\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/accounting/od/debt_to_penny\n  method: get\n  operationId: getDebtToPenny\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/dts/operating_cash_balance\n  method: get\n  operationId: getOperatingCashBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/mts/mts_table_1\n  method: get\n  operationId: getMonthlyTreasuryStatementTable1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounting/od/securities_sales\n  method: get\n  operationId: getSecuritiesSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounting/od/avg_interest_rates\n  method: get\n  operationId: getAverageInterestRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/od/rates_of_exchange\n  method: get\n  operationId: getRatesOfExchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/accounting/od/utf\n  method: get\n  operationId: getMSPD\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/sdn\n  method: get\n  operationId: getSdnList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/consolidated\n  method: get\n  operationId: getConsolidatedList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: searchSanctions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/agentic-access/department-of-the-treasury-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- Federal Government
- Finance
- Debt
- Sanctions
---
