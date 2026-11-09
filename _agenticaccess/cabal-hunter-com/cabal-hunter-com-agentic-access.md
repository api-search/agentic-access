---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: cabal-hunter-com-cex-funding-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Cex Funding API
  slug: cabal-hunter-com-cex-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-cex-funding-api-openapi.yml
- filename: cabal-hunter-com-cohorts-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Cohorts API
  slug: cabal-hunter-com-cohorts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-cohorts-api-openapi.yml
- filename: cabal-hunter-com-info-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Info API
  slug: cabal-hunter-com-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-info-api-openapi.yml
- filename: cabal-hunter-com-scan-batch-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Scan Batch API
  slug: cabal-hunter-com-scan-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-scan-batch-api-openapi.yml
- filename: cabal-hunter-com-scan-cabal-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Scan Cabal API
  slug: cabal-hunter-com-scan-cabal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-scan-cabal-api-openapi.yml
- filename: cabal-hunter-com-screen-list-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Screen List API
  slug: cabal-hunter-com-screen-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-screen-list-api-openapi.yml
- filename: cabal-hunter-com-trade-analysis-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Trade Analysis API
  slug: cabal-hunter-com-trade-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-trade-analysis-api-openapi.yml
- filename: cabal-hunter-com-wallet-check-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Wallet Check API
  slug: cabal-hunter-com-wallet-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-wallet-check-api-openapi.yml
- filename: cabal-hunter-com-wallet-report-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Wallet Report API
  slug: cabal-hunter-com-wallet-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-wallet-report-api-openapi.yml
- filename: cabal-hunter-com-watch-api-openapi.yml
  format: yaml
  label: Cabal-Hunter Watch API
  slug: cabal-hunter-com-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cabal-hunter-com/openapi/cabal-hunter-com-watch-api-openapi.yml
consequence_counts:
  physical: 1
  read: 9
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cabal Hunter Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/screen-list/checkout
operation_count: 16
overview: 'Cabal-Hunter exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cabal-Hunter
provider_slug: cabal-hunter-com
slug: cabal-hunter-com-agentic-access
source_filename: cabal-hunter-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/cabal-hunter-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 9\n    acting: 7\n  by_consequence:\n    read: 9\n    write: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/scan-cabal\n  method: get\n  operationId: scanCabalGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/scan-cabal\n  method: post\n  operationId: scanCabal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scan-batch\n  method: post\n  operationId: scanBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/wallet-report\n  method: get\n  operationId: walletReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/info\n  method: get\n  operationId: info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cex-funding\n  method: get\n  operationId: cexFunding\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cohorts\n  method: get\n  operationId: cohorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trade-analysis\n  method: get\n  operationId: tradeAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wallet-check\n  method: get\n  operationId: walletCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/screen-list\n  method: get\n  operationId: listScreenList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/screen-list\n  method: post\n  operationId: addScreenListWallet\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/screen-list\n  method: delete\n  operationId: clearScreenList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/screen-list/checkout\n  method: post\n  operationId: enableScreenList\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/watch\n  method: get\n  operationId: listWatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/watch\n  method: post\n  operationId: watchDump\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/watch\n  method: delete\n  operationId: unwatchDump\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/cabal-hunter-com/agentic-access/cabal-hunter-com-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- Solana
- Cryptocurrency
- Security
- Analytics
---
