---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 15
api_specs:
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Address Dashboards API
  slug: address-dashboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Transaction Dashboards API
  slug: transaction-dashboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Block Dashboards API
  slug: block-dashboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Raw Data API
  slug: raw-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Stats API
  slug: stats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Outputs Database API
  slug: outputs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Broadcast API
  slug: broadcast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
consequence_counts:
  read: 15
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blockchair Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Blockchair exposes 16 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blockchair
provider_slug: blockchair
slug: blockchair-agentic-access
source_filename: blockchair-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/blockchair-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 15\n    acting: 1\n  by_consequence:\n    read: 15\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /{chain}/stats\n  method: get\n  operationId: getChainStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getMultiChainStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cross-chain/{token}/stats\n  method:\
  \ get\n  operationId: getCrossChainTokenStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/dashboards/address/{address}\n  method: get\n  operationId: getAddressDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/dashboards/addresses/{addresses}\n  method: get\n  operationId: getAddressesDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/dashboards/xpub/{extendedKey}\n  method: get\n  operationId: getXpubDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/dashboards/transaction/{hash}\n  method: get\n  operationId:\
  \ getTransactionDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/dashboards/transactions/{hashes}\n  method: get\n  operationId: getTransactionsDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/dashboards/block/{id}\n  method: get\n  operationId: getBlockDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/dashboards/blocks/{ids}\n  method: get\n  operationId: getBlocksDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/raw/block/{id}\n  method: get\n  operationId: getRawBlock\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/raw/transaction/{hash}\n  method: get\n  operationId: getRawTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/outputs\n  method: get\n  operationId: queryOutputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/blocks\n  method: get\n  operationId: queryBlocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/transactions\n  method: get\n  operationId: queryTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /{chain}/push/transaction\n  method: post\n  operationId: broadcastTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/agentic-access/blockchair-agentic-access.yml
summary_line: 16 operations · 1 acting
tags:
- Blockchain
- Cryptocurrency
- Explorer
- Bitcoin
- Ethereum
- On-Chain Data
---
