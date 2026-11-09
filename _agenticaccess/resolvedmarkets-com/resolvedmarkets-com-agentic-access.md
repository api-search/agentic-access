---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 37
api_specs:
- filename: resolvedmarkets-com-account-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Account API
  slug: resolvedmarkets-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-account-api-openapi.yml
- filename: resolvedmarkets-com-admin-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Admin API
  slug: resolvedmarkets-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-admin-api-openapi.yml
- filename: resolvedmarkets-com-backtest-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Backtest API
  slug: resolvedmarkets-com-backtest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-backtest-api-openapi.yml
- filename: resolvedmarkets-com-exchange-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Exchange API
  slug: resolvedmarkets-com-exchange-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-exchange-api-openapi.yml
- filename: resolvedmarkets-com-markets-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Markets API
  slug: resolvedmarkets-com-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-markets-api-openapi.yml
- filename: resolvedmarkets-com-payments-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Payments API
  slug: resolvedmarkets-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-payments-api-openapi.yml
- filename: resolvedmarkets-com-public-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Public API
  slug: resolvedmarkets-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-public-api-openapi.yml
- filename: resolvedmarkets-com-snapshots-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Snapshots API
  slug: resolvedmarkets-com-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-snapshots-api-openapi.yml
- filename: resolvedmarkets-com-strategies-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Strategies API
  slug: resolvedmarkets-com-strategies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-strategies-api-openapi.yml
- filename: resolvedmarkets-com-system-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com System API
  slug: resolvedmarkets-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-system-api-openapi.yml
- filename: resolvedmarkets-com-trades-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Trades API
  slug: resolvedmarkets-com-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-trades-api-openapi.yml
- filename: resolvedmarkets-com-wallets-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Wallets API
  slug: resolvedmarkets-com-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-wallets-api-openapi.yml
- filename: resolvedmarkets-com-webhooks-api-openapi.yml
  format: yaml
  label: resolvedmarkets-com Webhooks API
  slug: resolvedmarkets-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/resolvedmarkets-com/openapi/resolvedmarkets-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 3
  read: 37
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Resolvedmarkets Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/api-keys/{key}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/create-invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/create-stripe-session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/nowpayments
operation_count: 49
overview: 'resolvedmarkets-com exposes 49 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 8 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: resolvedmarkets-com
provider_slug: resolvedmarkets-com
slug: resolvedmarkets-com-agentic-access
source_filename: resolvedmarkets-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/resolvedmarkets-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 37\n    acting: 12\n  by_consequence:\n    read: 37\n    physical: 3\n    write: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-stats\n  method: get\n  operationId: getPublicStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/public-stats/schema.json\n  method: get\n  operationId: getDatasetSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/packs\n  method: get\n  operationId: listCreditPacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/currencies\n  method: get\n  operationId: listSupportedCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/estimate\n  method: get\n  operationId: estimateInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/create-invoice\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/create-stripe-session\n  method: post\n  operationId: createStripeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/subscription\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories\n  method:\
  \ get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/live\n  method: get\n  operationId: listLiveMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/by-slug/{slug}\n  method: get\n  operationId: getMarketBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/by-slug/{slug}/orderbook\n  method: get\n  operationId: getOrderbookBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/{id}/orderbook\n  method: get\n  operationId: getOrderbook\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/{id}/snapshots\n  method: get\n  operationId: listMarketSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/{id}/trades\n  method: get\n  operationId: listMarketTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/{id}/summary\n  method: get\n  operationId: getMarketSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/history/recent\n  method: get\n  operationId: listRecentMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/markets/history\n  method: get\n  operationId: listMarketHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats\n  method: get\n  operationId: getSystemStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/snapshot\n  method: get\n  operationId: getSnapshotAtTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/snapshot/latest\n  method: get\n  operationId: getLatestSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/debug\n  method: get\n  operationId: getDebugStats\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/diagnostics/r2\n  method: get\n  operationId: getR2Diagnostics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys/validate\n  method: get\n  operationId: validateApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exchange/orderbook\n  method: get\n  operationId: getExchangeOrderbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exchange/snapshots\n  method: get\n  operationId: listExchangeSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v1/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys/{key}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/user/tier\n  method: get\n\
  \  operationId: getUserTier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backtest/templates\n  method: get\n  operationId: listBacktestTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backtest/run\n  method: post\n  operationId: runBacktest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/backtest/agent\n  method: post\n  operationId: runBacktestAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/backtest/runs/{runId}\n  method: get\n  operationId: getBacktestRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backtest/runs/{runId}/stream\n  method: get\n  operationId: streamBacktestRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backtest/history\n  method: get\n  operationId: listBacktestHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backtest/agent/chats\n  method: get\n  operationId: listAgentChats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/strategies\n  method: get\n  operationId: listStrategies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/strategies\n  method: post\n  operationId: saveStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/strategies/{id}\n  method: delete\n  operationId: deleteStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/chat/me\n  method: get\n  operationId: getChatOwnerStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/chat/ws-ticket\n  method: post\n  operationId: issueChatWsTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/chat/sessions\n  method: get\n  operationId: listChatSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/chat/sessions/{id}/messages\n  method: get\n  operationId: getChatSessionMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/nowpayments\n\
  \  method: post\n  operationId: nowpaymentsWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/stripe\n  method: post\n  operationId: stripeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/clerk\n  method: post\n  operationId: clerkWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/wallets/{address}/fills\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/resolvedmarkets-com/agentic-access/resolvedmarkets-com-agentic-access.yml
summary_line: 49 operations · 12 acting · 1 human-in-the-loop
tags:
- Data
- Finance
- Prediction Markets
- Backtesting
---
