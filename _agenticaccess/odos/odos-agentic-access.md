---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 11
api_specs:
- filename: openapi.json
  format: json
  label: Odos Smart Order Router API
  slug: odos-smart-order-router-api
  spec_type: OpenAPI
  url: https://api.odos.xyz/sor/openapi.json
consequence_counts:
  physical: 6
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Odos Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sor/assemble
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sor/quote/v2
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sor/quote/v2/zap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sor/quote/v3
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sor/quote/v3/zap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sor/swap/v3
operation_count: 17
overview: 'Odos exposes 17 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Odos
provider_slug: odos
slug: odos-agentic-access
source_filename: odos-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 11\n    acting: 6\n  by_consequence:\n    read: 11\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /info/chains\n  method: get\n  operationId: get_chain_ids_info_chains_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/contract-info/{version}/{chain_id}\n  method: get\n  operationId: get_contract_info_info_contract_info__version___chain_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /info/router/{version}/{chain_id}\n  method: get\n  operationId: get_router_info_router__version___chain_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/executor/{version}/{chain_id}\n  method: get\n  operationId: get_executor_info_executor__version___chain_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/liquidity-sources/{chain_id}\n  method: get\n  operationId: get_liquidity_sources_info_liquidity_sources__chain_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/market-intelligence\n  method: get\n  operationId: get_market_intelligence_info_market_intelligence_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/tokens/{chain_id}\n  method: get\n  operationId: get_token_map_info_tokens__chain_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/current-block/{chain_id}\n  method: get\n  operationId: get_current_block_info_current_block__chain_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sor/swap/v3\n  method: post\n  operationId: swap_v3_sor_swap_v3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /sor/quote/v3\n  method: post\n  operationId: quote_v3_sor_quote_v3_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sor/quote/v3/zap\n  method: post\n  operationId: quote_zap_v3_sor_quote_v3_zap_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sor/quote/v2\n  method: post\n  operationId: quote_sor_quote_v2_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sor/quote/v2/zap\n  method: post\n  operationId: quote_zap_sor_quote_v2_zap_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sor/assemble\n  method: post\n  operationId: assemble_sor_assemble_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pricing/currencies\n  method: get\n  operationId: get_currencies_pricing_currencies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing/token/{chain_id}/{token_addr}\n  method: get\n  operationId: get_token_price_pricing_token__chain_id___token_addr__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing/token/{chain_id}\n  method: get\n  operationId: get_chain_token_prices_pricing_token__chain_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odos/refs/heads/main/agentic-access/odos-agentic-access.yml
summary_line: 17 operations · 6 acting
tags:
- DEX
- Aggregator
- DeFi
- Token Swaps
- Liquidity
- Routing
- Blockchain
- EVM
- Web3
---
