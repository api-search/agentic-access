---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Companies API
  slug: puzzle-io-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Transactions API
  slug: puzzle-io-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Ledger Accounts API
  slug: puzzle-io-ledger-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Journal Entries API
  slug: puzzle-io-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Financial Reports API
  slug: puzzle-io-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Metrics API
  slug: puzzle-io-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Categories API
  slug: puzzle-io-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Integrations API
  slug: puzzle-io-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Puzzle Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Puzzle exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Puzzle
provider_slug: puzzle-io
slug: puzzle-io-agentic-access
source_filename: puzzle-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/puzzle-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /rest/v0/companies\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v0/company/{id}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v0/company/{id}/transactions\n  method: get\n \
  \ operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v0/company/{id}/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v0/company/{id}/journal-entries\n  method: get\n  operationId: listJournalEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v0/company/{id}/reports/income-statement\n  method: get\n  operationId: getIncomeStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v0/company/{id}/reports/balance-sheet\n  method: get\n  operationId: getBalanceSheet\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v0/company/{id}/metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v0/company/{id}/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v0/company/{id}/integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/agentic-access/puzzle-io-agentic-access.yml
summary_line: 10 operations
tags:
- Accounting
- Fintech
- General Ledger
- Financial Reporting
- Bookkeeping
- Startups
- Embedded Accounting
- Metrics
---
