---
acting_count: 5
action_class_counts:
  acting: 5
api_specs:
- filename: chainaware-ai-enterprise-api-openapi.yml
  format: yaml
  label: ChainAware Enterprise API
  slug: chainaware-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/openapi/chainaware-ai-enterprise-api-openapi.yml
consequence_counts:
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chainaware Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'ChainAware.ai exposes 5 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ChainAware.ai
provider_slug: chainaware-ai
slug: chainaware-ai-agentic-access
source_filename: chainaware-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/chainaware-ai-enterprise-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\ncuration_note: >-\n  Heuristic caveat (API Evangelist, 2026-09-19): the classifier treats every POST as an acting/write\n  operation, but all five ChainAware operations are POST-bodied READS — each computes or returns a cached\n  score for an address and mutates nothing on the caller's behalf (docs: \"All endpoints operate in real\n  time against on-chain data\"; see conventions/chainaware-ai-conventions.yml reversibility: na). A\n  deployment binding these contracts should treat them as connected/read with the 3600 s TTL ceiling; the\n  only real side effects on ChainAware's surfaces are the MCP batch-job and token-audit\
  \ queueing tools, which\n  this file does not cover because no OpenAPI describes them. The per-call x402 cost ($0.15 USDC) is the\n  consequence worth gating, not a state change.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 5\n  by_consequence:\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /fraud/check\n  method: post\n  operationId: checkWalletFraud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fraud/audit\n  method: post\n  operationId: auditWalletBehaviour\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /rug/pull-check\n  method: post\n  operationId: checkRugPull\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /segmentation/wallet-segment\n  method: post\n  operationId: getWalletSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/credit-score\n  method: post\n  operationId: getCreditScore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainaware-ai/refs/heads/main/agentic-access/chainaware-ai-agentic-access.yml
summary_line: 5 operations · 5 acting
tags:
- Blockchain
- Web3
- DeFi
- Fraud Detection
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
- agent-native
- Estonia
---
