---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: avora-agent-forge-agent-api-openapi.yml
  format: yaml
  label: AVORA Agent Forge Agent API
  slug: avora-agent-forge-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avora-agent-forge/refs/heads/main/openapi/avora-agent-forge-agent-api-openapi.yml
- filename: avora-agent-forge-public-evidence-api-openapi.yml
  format: yaml
  label: AVORA Agent Forge Public Evidence API
  slug: avora-agent-forge-public-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avora-agent-forge/refs/heads/main/openapi/avora-agent-forge-public-evidence-api-openapi.yml
consequence_counts:
  physical: 1
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Avora Agent Forge Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/agent/pro-scan
operation_count: 8
overview: 'AVORA Agent Forge exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AVORA Agent Forge
provider_slug: avora-agent-forge
slug: avora-agent-forge-agentic-access
source_filename: avora-agent-forge-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/avora-agent-forge-commerce-openapi.json, openapi/avora-agent-forge-public-sector-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/agent/scan\n  method: get\n  operationId: scanSolanaTokenFree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/payment-order\n  method: get\n  operationId: createPaidEvidenceOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/offers\n  method: get\n  operationId: listEvidenceOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/pro-scan\n  method: post\n  operationId: verifyPaymentAndDeliverEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/revenue\n  method: get\n  operationId: getVerifiedRevenueStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gov/v1/health\n  method: get\n  operationId: getPublicAiServiceHealth\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gov/v1/scan\n  method: get\n  operationId: createSignedSolanaTokenAssessment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/jwks.json\n  method: get\n  operationId: getReceiptVerificationKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avora-agent-forge/refs/heads/main/agentic-access/avora-agent-forge-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- Blockchain
- Crypto
- Solana
- Token Risk
- Due Diligence
- On-chain Evidence
- Fraud Intelligence
- AI Agents
- MCP
- A2A
- Signed Receipts
- Provenance
- Non-custodial Payments
- USDC
- Solana Pay
- Public-sector AI Interoperability
---
