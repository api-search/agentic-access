---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 19
api_specs:
- filename: cow-protocol-account-api-openapi.yml
  format: yaml
  label: CoW Swap Account API
  slug: cow-protocol-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-account-api-openapi.yml
- filename: cow-protocol-app-data-api-openapi.yml
  format: yaml
  label: CoW Swap App Data API
  slug: cow-protocol-app-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-app-data-api-openapi.yml
- filename: cow-protocol-auction-api-openapi.yml
  format: yaml
  label: CoW Swap Auction API
  slug: cow-protocol-auction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-auction-api-openapi.yml
- filename: cow-protocol-notify-api-openapi.yml
  format: yaml
  label: CoW Swap Notify API
  slug: cow-protocol-notify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-notify-api-openapi.yml
- filename: cow-protocol-orders-api-openapi.yml
  format: yaml
  label: CoW Swap Orders API
  slug: cow-protocol-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-orders-api-openapi.yml
- filename: cow-protocol-quote-api-openapi.yml
  format: yaml
  label: CoW Swap Quote API
  slug: cow-protocol-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-quote-api-openapi.yml
- filename: cow-protocol-quotes-api-openapi.yml
  format: yaml
  label: CoW Swap Quotes API
  slug: cow-protocol-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-quotes-api-openapi.yml
- filename: cow-protocol-restricted-api-openapi.yml
  format: yaml
  label: CoW Swap Restricted API
  slug: cow-protocol-restricted-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-restricted-api-openapi.yml
- filename: cow-protocol-reveal-api-openapi.yml
  format: yaml
  label: CoW Swap Reveal API
  slug: cow-protocol-reveal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-reveal-api-openapi.yml
- filename: cow-protocol-settle-api-openapi.yml
  format: yaml
  label: CoW Swap Settle API
  slug: cow-protocol-settle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-settle-api-openapi.yml
- filename: cow-protocol-settle-fast-path-api-openapi.yml
  format: yaml
  label: CoW Swap Settle Fast Path API
  slug: cow-protocol-settle-fast-path-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-settle-fast-path-api-openapi.yml
- filename: cow-protocol-solve-api-openapi.yml
  format: yaml
  label: CoW Swap Solve API
  slug: cow-protocol-solve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-solve-api-openapi.yml
- filename: cow-protocol-solver-competition-api-openapi.yml
  format: yaml
  label: CoW Swap Solver Competition API
  slug: cow-protocol-solver-competition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-solver-competition-api-openapi.yml
- filename: cow-protocol-token-api-openapi.yml
  format: yaml
  label: CoW Swap Token API
  slug: cow-protocol-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-token-api-openapi.yml
- filename: cow-protocol-trades-api-openapi.yml
  format: yaml
  label: CoW Swap Trades API
  slug: cow-protocol-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-trades-api-openapi.yml
- filename: cow-protocol-transactions-api-openapi.yml
  format: yaml
  label: CoW Swap Transactions API
  slug: cow-protocol-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-transactions-api-openapi.yml
- filename: cow-protocol-users-api-openapi.yml
  format: yaml
  label: CoW Swap Users API
  slug: cow-protocol-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-users-api-openapi.yml
- filename: cow-protocol-version-api-openapi.yml
  format: yaml
  label: CoW Swap Version API
  slug: cow-protocol-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cow-protocol/openapi/cow-protocol-version-api-openapi.yml
consequence_counts:
  physical: 5
  read: 19
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cow Protocol Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/orders/{UID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /restricted/api/v1/debug/simulation
operation_count: 34
overview: 'CoW Swap exposes 34 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 10 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CoW Swap
provider_slug: cow-protocol
slug: cow-protocol-agentic-access
source_filename: cow-protocol-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/driver.yml, openapi/openapi.json, openapi/orderbook.yml, openapi/solvers.yml,\n  openapi/x402.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 19\n    acting: 15\n  by_consequence:\n    read: 19\n    write: 10\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /quote\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solve\n  method: post\n  operationId: solve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reveal\n  method: post\n  operationId: revealCalldata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settle\n  method: post\n  operationId: settle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settle_fast_path\n  method: post\n  operationId: settleFastPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notify\n  method: post\n  operationId: receiveNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quote\n  method: post\n  operationId: getPaidQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/orders\n  method: delete\n  operationId: cancelOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/orders/by_uids\n  method: post\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orders/{UID}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orders/{UID}\n\
  \  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/orders/{UID}/status\n  method: get\n  operationId: getOrderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/{txHash}/orders\n  method: get\n  operationId: getOrdersByTxHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/trades\n  method: get\n  operationId: getTradesV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auction\n  method: get\n  operationId: getCurrentBatchAuction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/{owner}/orders\n  method: get\n  operationId: getUserOrdersPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/token/{token}/native_price\n  method: get\n  operationId: getTokenNativePrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quote\n  method: post\n  operationId: quote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quote/stream\n  method: post\n  operationId: quoteStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/solver_competition/{auction_id}\n  method: get\n  operationId: getSolverCompetitionByAuctionIdV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/solver_competition/by_tx_hash/{tx_hash}\n  method: get\n  operationId: getSolverCompetitionByTxHashV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v2/solver_competition/latest\n  method: get\n  operationId: getSolverCompetitionLatestV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/version\n  method: get\n  operationId: getApiVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app_data/{app_data_hash}\n  method: get\n  operationId: getAppDataByHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app_data/{app_data_hash}\n  method: put\n  operationId: registerAppDataByHash\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app_data\n  method: put\n  operationId: registerAppData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/{address}/total_surplus\n  method: get\n  operationId: getAddressTotalSurplus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restricted/api/v1/debug/simulation\n  method: post\n  operationId: debugSimulationPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restricted/api/v1/debug/simulation/{uid}\n  method: get\n  operationId: debugSimulation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restricted/api/v1/debug/order/{uid}\n  method: get\n  operationId: debugOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solve\n  method: post\n  operationId: solve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notify\n  method: post\n  operationId: notify\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quote\n  method: post\n  operationId: getPaidQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cow-protocol/agentic-access/cow-protocol-agentic-access.yml
summary_line: 34 operations · 15 acting
tags:
- DeFi
- Ethereum
- Swap
- Liquidity
- Governance
- AMM
---
