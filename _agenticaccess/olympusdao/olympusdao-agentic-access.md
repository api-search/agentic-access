---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: openapi.json
  format: json
  label: Olympus Protocol Metrics API
  slug: olympus-protocol-metrics-api
  spec_type: OpenAPI
  url: https://treasury-subgraph-api.olympusdao.finance/openapi.json
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Olympusdao Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'OlympusDAO exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OlympusDAO
provider_slug: olympusdao
slug: olympusdao-agentic-access
source_filename: olympusdao-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/olympus-protocol-metrics-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /ready\n  method: get\n  operationId: getReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bounds\n  method: get\n  operationId: getBounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/metrics/daily\n  method: get\n  operationId: getDailyMetrics\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/treasury-assets/daily\n  method: get\n  operationId: getDailyTreasuryAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ohm-supply/daily\n  method: get\n  operationId: getDailyOhmSupply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/health\n  method: get\n  operationId: getLegacyHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/latest/metrics\n  method: get\n  operationId: getLatestMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /operations/earliest/metrics\n  method: get\n  operationId: getEarliestMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/paginated/metrics\n  method: get\n  operationId: getPaginatedMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/latest/tokenRecords\n  method: get\n  operationId: getLatestTokenRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/earliest/tokenRecords\n  method: get\n  operationId: getEarliestTokenRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /operations/paginated/tokenRecords\n  method: get\n  operationId: getPaginatedTokenRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/latest/tokenSupplies\n  method: get\n  operationId: getLatestTokenSupplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/earliest/tokenSupplies\n  method: get\n  operationId: getEarliestTokenSupplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/paginated/tokenSupplies\n  method: get\n  operationId: getPaginatedTokenSupplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/latest/protocolMetrics\n\
  \  method: get\n  operationId: getLatestProtocolMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/earliest/protocolMetrics\n  method: get\n  operationId: getEarliestProtocolMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/paginated/protocolMetrics\n  method: get\n  operationId: getPaginatedProtocolMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/atBlock/metrics\n  method: get\n  operationId: getAtBlockMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/atBlock/tokenRecords\n  method: get\n  operationId:\
  \ getAtBlockTokenRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/atBlock/tokenSupplies\n  method: get\n  operationId: getAtBlockTokenSupplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/atBlock/internal/protocolMetrics\n  method: get\n  operationId: getAtBlockInternalProtocolMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olympusdao/refs/heads/main/agentic-access/olympusdao-agentic-access.yml
summary_line: 22 operations
tags:
- DeFi
- Protocol-Owned Liquidity
- Reserve Currency
- Treasury
- Staking
- Bonds
- OHM
- Ethereum
- Web3
---
