---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: bykaranteli-x402-api-openapi.yml
  format: yaml
  label: ByKaranteli X402 API
  slug: bykaranteli-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bykaranteli/refs/heads/main/openapi/bykaranteli-x402-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bykaranteli Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'ByKaranteli exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ByKaranteli
provider_slug: bykaranteli
slug: bykaranteli-agentic-access
source_filename: bykaranteli-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/bykaranteli-x402-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this API to AI agents — review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /api/x402\n  method: get\n  operationId: x402Catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/liqmap-levels\n  method: get\n  operationId: liqmap-levels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n    \
  \  model: x402-per-call\n      currency: USD\n      amount: 0.005\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/options-flow\n  method: get\n  operationId: options-flow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.005\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/flow-vpin\n  method: get\n  operationId: flow-vpin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.002\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/premium-history\n  method: get\n  operationId: premium-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.005\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/cot-history\n  method: get\n  operationId: cot-history\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.005\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/liquidations-raw\n  method: get\n  operationId: liquidations-raw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.01\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/oi-history\n\
  \  method: get\n  operationId: oi-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.005\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/funding-history\n  method: get\n  operationId: funding-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.005\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n\
  \    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/options-oi-history\n  method: get\n  operationId: options-oi-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.005\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/dvol-history\n  method: get\n  operationId: dvol-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.002\n      asset: USDC\n      networks:\n      -\
  \ solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/slippage-history\n  method: get\n  operationId: slippage-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.002\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/listings-history\n  method: get\n  operationId: listings-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model:\
  \ x402-per-call\n      currency: USD\n      amount: 0.002\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\n- path: /api/x402/spot-microstructure\n  method: get\n  operationId: spot-microstructure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: payment settlement is onchain and self-auditing\n    cost:\n      model: x402-per-call\n      currency: USD\n      amount: 0.01\n      asset: USDC\n      networks:\n      - solana:5eykt4UsFv8P8NJdTREpY1vzqKqZKvdp\n      - eip155:8453\n      billed: per successful response\n    human-in-the-loop: recommended (spend approval)\nx-payment-correction:\n  note: 'The heuristic classifier read all 14 operations as consequence: read, which is true of the DATA\n    but false of the CALL. Thirteen of the fourteen settle\
  \ a USDC micropayment per successful response,\n    so they are read-with-spend, not free reads. Per-operation cost blocks and a spend-approval recommendation\n    have been added above from the provider''s own /api/x402 catalog and per-operation x-payment-info.\n    Only x402Catalog is genuinely free.'\n  operations_corrected: 13\n  source: https://bykaranteli.com/api/x402\n  detail: finops/bykaranteli-finops.yml\nx-free-surface-note: The free public REST surface (/api/public/*, /api/v1/public/*) and the 20 anonymous\n  MCP tools at https://mcp.bykaranteli.com are genuinely unauthenticated read-only reads with no spend\n  consequence. They are not classified here because they have no OpenAPI to classify from.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bykaranteli/refs/heads/main/agentic-access/bykaranteli-agentic-access.yml
summary_line: 14 operations
tags:
- Cryptocurrency
- Crypto Derivatives
- Market Data
- Funding Rates
- Open Interest
- Liquidations
- Options
- ETF Flows
- Financial Data
- MCP
- x402
- Agents
---
