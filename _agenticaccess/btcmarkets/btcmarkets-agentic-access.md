---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 27
api_specs:
- filename: btcmarkets-account-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Account APIs API
  slug: btcmarkets-account-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-account-apis-api-openapi.yml
- filename: btcmarkets-batch-order-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Batch Order APIs API
  slug: btcmarkets-batch-order-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-batch-order-apis-api-openapi.yml
- filename: btcmarkets-fund-management-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Fund Management APIs API
  slug: btcmarkets-fund-management-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-fund-management-apis-api-openapi.yml
- filename: btcmarkets-market-data-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Market Data APIs API
  slug: btcmarkets-market-data-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-market-data-apis-api-openapi.yml
- filename: btcmarkets-misc-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Misc APIs API
  slug: btcmarkets-misc-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-misc-apis-api-openapi.yml
- filename: btcmarkets-order-placement-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Order Placement APIs API
  slug: btcmarkets-order-placement-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-order-placement-apis-api-openapi.yml
- filename: btcmarkets-report-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Report APIs API
  slug: btcmarkets-report-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-report-apis-api-openapi.yml
- filename: btcmarkets-trade-apis-api-openapi.yml
  format: yaml
  label: BTC Markets Trade APIs API
  slug: btcmarkets-trade-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/openapi/btcmarkets-trade-apis-api-openapi.yml
consequence_counts:
  physical: 7
  read: 27
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Btcmarkets Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/batchorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v3/batchorders/{ids}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v3/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v3/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v3/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/withdrawals
operation_count: 35
overview: 'BTC Markets exposes 35 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 1 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BTC Markets
provider_slug: btcmarkets
slug: btcmarkets-agentic-access
source_filename: btcmarkets-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/btcmarkets-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    acting: 8\n    connected: 27\n  by_consequence:\n    physical: 7\n    read: 27\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/orders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/orders\n  method: delete\n  operationId: cancelOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{id}\n  method: get\n  operationId: getOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/orders/{id}\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orders/{id}\n  method: put\n  operationId: replaceOrderById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/batchorders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/batchorders/{ids}\n  method: get\n  operationId: getOrderByIds\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/batchorders/{ids}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/trades\n  method: get\n  operationId: getTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/trades/{id}\n  method: get\n  operationId: getTradeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/markets\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/markets/{marketId}/ticker\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/markets/{marketId}/trades\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/markets/{marketId}/orderbook\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/markets/{marketId}/candles\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/markets/tickers\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/markets/orderbooks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/withdrawals\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/withdrawals\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/withdrawals/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v3/deposits\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/deposits/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/transfers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/transfers/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/addresses\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/withdrawal-fees\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/assets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reports\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/reports/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/me/trading-fees\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v3/accounts/me/withdrawal-limits\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/me/balances\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/me/transactions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/time\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btcmarkets/refs/heads/main/agentic-access/btcmarkets-agentic-access.yml
summary_line: 35 operations · 8 acting
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Australia
---
