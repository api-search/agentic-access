---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 12
api_specs:
- filename: cipherowl-openapi.json
  format: json
  label: CipherOwl SRR API
  slug: cipherowl-srr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cipherowl/refs/heads/main/openapi/cipherowl-openapi.json
consequence_counts:
  read: 12
  safety-critical: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Cipherowl Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/private-data/v1/overrides/chains/{chain}/addresses
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/private-data/v1/overrides/chains/{chain}/addresses/{address}
operation_count: 16
overview: 'CipherOwl exposes 16 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 2 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CipherOwl
provider_slug: cipherowl
slug: cipherowl-agentic-access
source_filename: cipherowl-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/cipherowl-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 12\n    acting: 4\n  by_consequence:\n    read: 12\n    write: 2\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /api/report/v1/graph/chains/{chain}/addresses/{address}\n  method: get\n  operationId: graph_api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/onchain/v1/chains/{chain}/balances:batchget\n  method: post\n  operationId: OnChainService_BatchGetBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/onchain/v1/chains/{chain}/addresses/{address}/balance\n  method: get\n  operationId: OnChainService_GetBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/onchain/v1/chains\n  method: get\n  operationId: OnChainService_GetSupportedChains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/private-data/v1/overrides/chains/{chain}/addresses/{address}\n  method: delete\n  operationId: PrivateDataService_DeleteEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/private-data/v1/overrides/chains/{chain}/addresses/{address}\n  method: get\n  operationId: PrivateDataService_GetEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/private-data/v1/overrides/chains/{chain}/addresses\n  method: get\n  operationId: PrivateDataService_ListEntriesForChain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/private-data/v1/overrides/chains/{chain}/addresses\n  method: post\n  operationId: PrivateDataService_UpsertEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/report/v1/risk-assessment/chains/{chain}/addresses/{address}\n  method: get\n  operationId: risk_assessment_api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reason/v2/chains/{chain}/addresses/{address}/risk-breakdown\n  method: get\n  operationId: RiskReasonService_GetAddressRiskBreakdown2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reason/v2/chains/{chain}/addresses/{address}/detail\n  method: get\n  operationId: RiskReasonService_GetAddressRiskReasonDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /api/reason/v2/chains/{chain}/addresses/{address}/risk-score\n  method: get\n  operationId: RiskReasonService_GetAddressRiskScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chain-capabilities/v1\n  method: get\n  operationId: RiskReasonService_GetChainCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/report/v1/sar/chains/{chain}/addresses/{address}\n  method: get\n  operationId: sar_report_api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/screen/v1/chains/{chain}/batch\n  method: post\n  operationId: ScreenService_BatchScreenAddresses\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/screen/v1/chains/{chain}/addresses/{address}\n  method: get\n  operationId: ScreenService_ScreenAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cipherowl/refs/heads/main/agentic-access/cipherowl-agentic-access.yml
summary_line: 16 operations · 4 acting · 2 human-in-the-loop
tags:
- Blockchain
- Compliance
- Crypto
- Security
- Risk
- Sanctions Screening
- AML
- Digital Assets
- Stablecoins
- Web3
---
