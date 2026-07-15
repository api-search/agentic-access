---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 16
api_specs:
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Transactions API
  slug: digits-com-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Source Sync API
  slug: digits-com-source-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Parties API
  slug: digits-com-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Chart of Accounts API
  slug: digits-com-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Financial Statements API
  slug: digits-com-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Connections API
  slug: digits-com-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Organizations API
  slug: digits-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
consequence_counts:
  read: 16
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Digits Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Digits exposes 24 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Digits
provider_slug: digits-com
slug: digits-com-agentic-access
source_filename: digits-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/digits-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 16\n    acting: 8\n  by_consequence:\n    read: 16\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /ledger/transactions/entries\n  method: get\n  operationId: ledgerTransactionServiceEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/transactions/query\n  method: post\n  operationId: ledgerTransactionServiceQueryEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ledger/transactions/{transactionId}\n  method: get\n  operationId: ledgerTransactionServiceGetTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources/transactions/sync\n  method: post\n  operationId: sourceTransactionServiceSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sources/parties/sync\n  method: post\n  operationId: sourcePartyServiceSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ledger/parties\n  method: get\n  operationId: ledgerPartyServiceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/parties/{partyId}\n  method: get\n  operationId: ledgerPartyServiceGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/categories\n  method: get\n  operationId: ledgerCategoryServiceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/departments\n  method: get\n  operationId: ledgerDepartmentServiceList\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/locations\n  method: get\n  operationId: ledgerLocationServiceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/projects\n  method: get\n  operationId: ledgerProjectServiceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/statements/balance-sheet\n  method: get\n  operationId: ledgerStatementsServiceBalanceSheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/statements/profit-and-loss\n  method: get\n  operationId: ledgerStatementsServiceProfitAndLoss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/statements/cash-flow\n  method: get\n  operationId: ledgerStatementsServiceCashFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/statements/trial-balance\n  method: get\n  operationId: ledgerStatementsServiceTrialBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/statements/ap-aging\n  method: get\n  operationId: ledgerStatementsServiceApAging\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/statements/ar-aging\n  method: get\n  operationId: ledgerStatementsServiceArAging\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /ledger/summarize\n  method: post\n  operationId: ledgerSummaryServiceSummarize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/sources\n  method: get\n  operationId: connectionSourceServiceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/sources/sync\n  method: post\n  operationId: connectionSourceServiceSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /organizations/clients\n  method: get\n  operationId: organizationClientServiceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/clients\n  method: post\n  operationId: organizationClientServiceCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/clients/bulk\n  method: post\n  operationId: organizationClientServiceBulkCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /webhooks/events\n  method: post\n  operationId: receiveWebhookEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/agentic-access/digits-com-agentic-access.yml
summary_line: 24 operations · 8 acting
tags:
- Accounting
- Bookkeeping
- Finance
- General Ledger
- AI
- FinTech
---
