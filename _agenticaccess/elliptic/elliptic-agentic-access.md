---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 24
api_specs:
- filename: elliptic-assets-api-openapi.yml
  format: yaml
  label: Elliptic Assets API
  slug: elliptic-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-assets-api-openapi.yml
- filename: elliptic-count-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Count Analyses API
  slug: elliptic-count-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-count-analyses-api-openapi.yml
- filename: elliptic-criteria-api-openapi.yml
  format: yaml
  label: Elliptic Criteria API
  slug: elliptic-criteria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-criteria-api-openapi.yml
- filename: elliptic-customers-api-openapi.yml
  format: yaml
  label: Elliptic Customers API
  slug: elliptic-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-customers-api-openapi.yml
- filename: elliptic-health-api-openapi.yml
  format: yaml
  label: Elliptic Health API
  slug: elliptic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-health-api-openapi.yml
- filename: elliptic-risk-rules-api-openapi.yml
  format: yaml
  label: Elliptic Risk Rules API
  slug: elliptic-risk-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-risk-rules-api-openapi.yml
- filename: elliptic-sanctions-api-openapi.yml
  format: yaml
  label: Elliptic Sanctions API
  slug: elliptic-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-sanctions-api-openapi.yml
- filename: elliptic-screenings-api-openapi.yml
  format: yaml
  label: Elliptic Screenings API
  slug: elliptic-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-screenings-api-openapi.yml
- filename: elliptic-transaction-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Transaction Analyses API
  slug: elliptic-transaction-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-transaction-analyses-api-openapi.yml
- filename: elliptic-transaction-workflow-api-openapi.yml
  format: yaml
  label: Elliptic Transaction Workflow API
  slug: elliptic-transaction-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-transaction-workflow-api-openapi.yml
- filename: elliptic-tron-nodeintelligence-api-openapi.yml
  format: yaml
  label: Elliptic Tron NodeIntelligence API
  slug: elliptic-tron-nodeintelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-tron-nodeintelligence-api-openapi.yml
- filename: elliptic-users-api-openapi.yml
  format: yaml
  label: Elliptic Users API
  slug: elliptic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-users-api-openapi.yml
- filename: elliptic-wallet-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Analyses API
  slug: elliptic-wallet-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-analyses-api-openapi.yml
- filename: elliptic-wallet-analyses-count-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Analyses Count API
  slug: elliptic-wallet-analyses-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-analyses-count-api-openapi.yml
- filename: elliptic-wallet-api-openapi.yml
  format: yaml
  label: Elliptic Wallet API
  slug: elliptic-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-api-openapi.yml
- filename: elliptic-wallet-workflow-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Workflow API
  slug: elliptic-wallet-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-workflow-api-openapi.yml
consequence_counts:
  read: 24
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Elliptic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'Elliptic exposes 40 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Elliptic
provider_slug: elliptic
slug: elliptic-agentic-access
source_filename: elliptic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aml-api-oauth.json, openapi/aml-api-v2.json, openapi/aml-api-v3.json, openapi/data-fabric.yaml,\n  openapi/ia-api.json, openapi/sanctions-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 24\n    acting: 16\n  by_consequence:\n    read: 24\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /analyses/count\n  method: get\n  operationId: count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n    - profile\n- path: /customers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/investigator\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/workflow_status\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyses/synchronous\n  method: post\n  operationId: analysisSync\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyses\n  method: post\n  operationId: analysisBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyses\n  method: get\n  operationId: getAllAnalyses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyses/count\n  method: get\n  operationId: count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /analyses/{mc_analysis_id}\n  method: get\n  operationId: getAnalysisById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyses/{mc_analysis_id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyses/{mc_analysis_id}/screenings/{screening_id}\n  method: get\n  operationId: getAnalysisByScreeningId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyses/workflow_status\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyses/assigned_team_user\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/count\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/synchronous\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/{wallet_analysis_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/{wallet_analysis_id}/screenings/{screening_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/workflow_status\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/assigned_team_user\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk_rules\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /criteria/categories\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/node-intelligence/tron/transactions\n  method: post\n  operationId: submitTransactionLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/node-intelligence/tron/wallet\n  method: post\n  operationId: submitWalletLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/node-intelligence/tron/node\n  method: post\n  operationId: submitNodeLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/node-intelligence/queries/{query_id}\n  method: get\n  operationId: pollQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /copilot/wallet/{screeningId}\n  method: get\n  operationId: getWalletSummary\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /copilot/wallet/riskgraph/{direction}/{screeningId}\n  method: post\n  operationId: postWalletRiskGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /copilot/wallet/entities/{direction}/{screeningId}\n  method: get\n  operationId: getWalletEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /copilot/transaction/{screeningId}\n  method: get\n  operationId: getTransactionSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /copilot/transaction/riskgraph/{screeningId}\n  method: post\n  operationId: postTransactionRiskGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /copilot/transaction/entities/{screeningId}\n  method: get\n  operationId: getTransactionEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /copilot/customers/summary/{customerId}\n  method: get\n  operationId: getCustomerSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /copilot/customers/summary/{customerId}/transaction-assets\n  method: get\n  operationId: getTransactionAssetsByCustomerId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sanctions\n  method: get\n  operationId: SanctionsController_getSanctionedAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/agentic-access/elliptic-agentic-access.yml
summary_line: 40 operations · 16 acting
tags:
- Blockchain
- Crypto
- Compliance
- AML
- Transaction Screening
- Wallet Screening
- Risk Scoring
- Analytics
---
