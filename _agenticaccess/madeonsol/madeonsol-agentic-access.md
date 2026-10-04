---
acting_count: 0
action_class_counts:
  connected: 35
api_specs:
- filename: madeonsol-robinhood-chain-api-openapi.yml
  format: yaml
  label: MadeOnSol Robinhood Chain API
  slug: madeonsol-robinhood-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeonsol/refs/heads/main/openapi/madeonsol-robinhood-chain-api-openapi.yml
- filename: madeonsol-solana-api-openapi.yml
  format: yaml
  label: MadeOnSol Solana API
  slug: madeonsol-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeonsol/refs/heads/main/openapi/madeonsol-solana-api-openapi.yml
consequence_counts:
  read: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Madeonsol Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 35
overview: 'MadeOnSol exposes 35 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MadeOnSol
provider_slug: madeonsol
slug: madeonsol-agentic-access
source_filename: madeonsol-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: generated\nsource: openapi/madeonsol.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 35\n  by_consequence:\n    read: 35\n  human_in_the_loop_required: 0\noperations:\n- path: /api/x402/kol/coordination\n  method: get\n  operationId: kol_coordination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/kol/feed\n  method: get\n  operationId: kol_feed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/kol/leaderboard\n  method: get\n  operationId:\
  \ kol_leaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/kol/pairs\n  method: get\n  operationId: kol_pairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/kol/tokens/hot\n  method: get\n  operationId: kol_tokens_hot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/kol/tokens/trending\n  method: get\n  operationId: kol_tokens_trending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/kol/tokens/{mint}/entry-order\n  method: get\n  operationId: kol_tokens_mint_entry-order\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/kol/compare\n  method: get\n  operationId: kol_compare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/kol/alerts/recent\n  method: get\n  operationId: kol_alerts_recent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/deployer-hunter/alerts\n  method: get\n  operationId: deployer-hunter_alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/wallet/{address}\n  method: get\n  operationId: wallet_address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/x402/wallet/{address}/pnl\n  method: get\n  operationId: wallet_address_pnl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/wallet/{address}/positions\n  method: get\n  operationId: wallet_address_positions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/wallet/{address}/trades\n  method: get\n  operationId: wallet_address_trades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/tokens/{mint}/risk\n  method: get\n  operationId: tokens_mint_risk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/tokens/{mint}/buyer-quality\n\
  \  method: get\n  operationId: tokens_mint_buyer-quality\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/token/{mint}\n  method: get\n  operationId: token_mint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/signals/{name}/performance\n  method: get\n  operationId: signals_name_performance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/tokens/{mint}/candles\n  method: get\n  operationId: tokens_mint_candles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/tokens/{mint}/flow\n  method: get\n  operationId: tokens_mint_flow\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/tokens/{mint}/top-traders\n  method: get\n  operationId: tokens_mint_top-traders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/tokens/{mint}/cap-table\n  method: get\n  operationId: tokens_mint_cap-table\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/tokens/almost-bonded\n  method: get\n  operationId: tokens_almost-bonded\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/sniper/recent\n  method: get\n  operationId: sniper_recent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/deployer-hunter/{address}/trajectory\n  method: get\n  operationId: deployer-hunter_address_trajectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/rhc/kol/feed\n  method: get\n  operationId: rhc_kol_feed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/rhc/kol/hot-tokens\n  method: get\n  operationId: rhc_kol_hot-tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/rhc/kol/leaderboard\n  method: get\n  operationId: rhc_kol_leaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/x402/rhc/tokens/{mint}\n  method: get\n  operationId: rhc_tokens_mint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/rhc/tokens/{mint}/buyer-quality\n  method: get\n  operationId: rhc_tokens_mint_buyer-quality\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/rhc/tokens/{mint}/kol-consensus\n  method: get\n  operationId: rhc_tokens_mint_kol-consensus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/rhc/tokens/{mint}/risk\n  method: get\n  operationId: rhc_tokens_mint_risk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/x402/rhc/tokens/{mint}/holders\n  method: get\n  operationId: rhc_tokens_mint_holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/rhc/wallet/{address}/pnl\n  method: get\n  operationId: rhc_wallet_address_pnl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/rhc/deployer-hunter/alerts\n  method: get\n  operationId: rhc_deployer-hunter_alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madeonsol/refs/heads/main/agentic-access/madeonsol-agentic-access.yml
summary_line: 35 operations
tags:
- Blockchain
- Analytics
- Solana
- Robinhood Chain
---
