---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: chainaware-ai-behaviour-prediction-api-api-openapi.yml
  format: yaml
  label: ChainAware.ai Behaviour Prediction API
  slug: chainaware-ai-behaviour-prediction-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/openapi/chainaware-ai-behaviour-prediction-api-api-openapi.yml
- filename: chainaware-ai-credit-score-api-api-openapi.yml
  format: yaml
  label: ChainAware.ai Credit Score API
  slug: chainaware-ai-credit-score-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/openapi/chainaware-ai-credit-score-api-api-openapi.yml
- filename: chainaware-ai-fraud-api-api-openapi.yml
  format: yaml
  label: ChainAware.ai Fraud API
  slug: chainaware-ai-fraud-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/openapi/chainaware-ai-fraud-api-api-openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chainaware Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'ChainAware.ai exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ChainAware.ai
provider_slug: chainaware-ai
slug: chainaware-ai-agentic-access
source_filename: chainaware-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/chainaware-ai-enterprise-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /fraud/check\n  method: post\n  operationId: checkWalletFraud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fraud/audit\n  method: post\n  operationId: auditWalletBehaviour\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rug/pull-check\n  method: post\n  operationId: checkRugPull\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /segmentation/wallet-segment\n  method: post\n  operationId: getWalletSegment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/credit-score\n  method: post\n  operationId: getCreditScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/agentic-access/chainaware-ai-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Blockchain
- Web3
- DeFi
- Fraud Prevention
- AML
- Compliance
- Credit Scoring
- Risk Scoring
- Smart Contract Security
- Agent Trust
- MCP
- A2A
- x402
- Agents
- Agent-Native
- Estonia
---
