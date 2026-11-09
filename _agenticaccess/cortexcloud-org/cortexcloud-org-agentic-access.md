---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 13
api_specs:
- filename: cortexcloud-org-aggregation-api-openapi.yml
  format: yaml
  label: cortexcloud-org Aggregation API
  slug: cortexcloud-org-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cortexcloud-org/openapi/cortexcloud-org-aggregation-api-openapi.yml
- filename: cortexcloud-org-bazaar-mcp-api-openapi.yml
  format: yaml
  label: cortexcloud-org Bazaar / MCP API
  slug: cortexcloud-org-bazaar-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cortexcloud-org/openapi/cortexcloud-org-bazaar-mcp-api-openapi.yml
- filename: cortexcloud-org-catalog-api-openapi.yml
  format: yaml
  label: cortexcloud-org Catalog API
  slug: cortexcloud-org-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cortexcloud-org/openapi/cortexcloud-org-catalog-api-openapi.yml
- filename: cortexcloud-org-data-api-openapi.yml
  format: yaml
  label: cortexcloud-org Data API
  slug: cortexcloud-org-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cortexcloud-org/openapi/cortexcloud-org-data-api-openapi.yml
- filename: cortexcloud-org-discovery-api-openapi.yml
  format: yaml
  label: cortexcloud-org Discovery API
  slug: cortexcloud-org-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cortexcloud-org/openapi/cortexcloud-org-discovery-api-openapi.yml
- filename: cortexcloud-org-system-api-openapi.yml
  format: yaml
  label: cortexcloud-org System API
  slug: cortexcloud-org-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cortexcloud-org/openapi/cortexcloud-org-system-api-openapi.yml
- filename: cortexcloud-org-x402-audit-trust-api-openapi.yml
  format: yaml
  label: cortexcloud-org x402 Audit & Trust API
  slug: cortexcloud-org-x402-audit-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cortexcloud-org/openapi/cortexcloud-org-x402-audit-trust-api-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cortexcloud Org Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/data/nft-ownership
operation_count: 26
overview: 'cortexcloud-org exposes 26 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: cortexcloud-org
provider_slug: cortexcloud-org
slug: cortexcloud-org-agentic-access
source_filename: cortexcloud-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/cortexcloud-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 13\n    acting: 13\n  by_consequence:\n    read: 13\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/x402list.txt\n  method: get\n  operationId: x402list_txt__well_known_x402list_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities\n  method: get\n  operationId: capabilities_v1_capabilities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/token-balances\n  method: post\n  operationId: token_balances_v1_data_token_balances_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/token-price\n  method: post\n  operationId: token_price_v1_data_token_price_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/nft-ownership\n  method: post\n  operationId: nft_ownership_v1_data_nft_ownership_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/tx-history\n  method: post\n  operationId: tx_history_v1_data_tx_history_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/gas-oracle\n  method: get\n  operationId: gas_oracle_v1_data_gas_oracle_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/block\n  method: get\n  operationId: block_v1_data_block_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/token-risk\n  method: post\n  operationId: token_risk_v1_data_token_risk_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/wallet-intel\n  method: post\n  operationId: wallet_intel_v1_data_wallet_intel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/whale-alerts\n  method: post\n  operationId: whale_alerts_v1_data_whale_alerts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/cross-chain-compare\n  method: post\n  operationId: cross_chain_compare_v1_data_cross_chain_compare_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/token-intel\n  method: post\n  operationId: token_intel_v1_data_token_intel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/aggregate/balances\n\
  \  method: post\n  operationId: aggregate_balances_v1_aggregate_balances_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/aggregate/prices\n  method: post\n  operationId: aggregate_prices_v1_aggregate_prices_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/aggregate/nfts\n  method: post\n  operationId: aggregate_nfts_v1_aggregate_nfts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/aggregate/tx-history\n  method: post\n  operationId: aggregate_tx_history_v1_aggregate_tx_history_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/x402.json\n  method: get\n  operationId: well_known_x402__well_known_x402_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  operationId: well_known_x402_v1__well_known_x402_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /.well-known/agentsearch.txt\n  method: get\n  operationId: agentsearch_txt__well_known_agentsearch_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms_txt_llms_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/bazaar\n  method: get\n  operationId: bazaar_root__well_known_bazaar_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/pubkey\n  method: get\n  operationId: get_pubkey_x402_v1_pubkey_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/usage\n  method: get\n  operationId:\
  \ usage_x402_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/receipts\n  method: get\n  operationId: receipts_x402_v1_receipts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cortexcloud-org/agentic-access/cortexcloud-org-agentic-access.yml
summary_line: 26 operations · 13 acting
tags:
- Company
- Blockchain
- Artificial Intelligence
- Payments
- On-Chain Data
---
