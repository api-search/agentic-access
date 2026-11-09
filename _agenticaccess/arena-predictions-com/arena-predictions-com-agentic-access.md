---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 29
api_specs:
- filename: arena-predictions-com-api-keys-api-openapi.yml
  format: yaml
  label: Arena API keys API
  slug: arena-predictions-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-api-keys-api-openapi.yml
- filename: arena-predictions-com-identity-api-openapi.yml
  format: yaml
  label: Arena Identity API
  slug: arena-predictions-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-identity-api-openapi.yml
- filename: arena-predictions-com-markets-api-openapi.yml
  format: yaml
  label: Arena Markets API
  slug: arena-predictions-com-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-markets-api-openapi.yml
- filename: arena-predictions-com-portfolio-api-openapi.yml
  format: yaml
  label: Arena Portfolio API
  slug: arena-predictions-com-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-portfolio-api-openapi.yml
- filename: arena-predictions-com-records-api-openapi.yml
  format: yaml
  label: Arena Records API
  slug: arena-predictions-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-records-api-openapi.yml
- filename: arena-predictions-com-status-api-openapi.yml
  format: yaml
  label: Arena Status API
  slug: arena-predictions-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-status-api-openapi.yml
- filename: arena-predictions-com-trading-api-openapi.yml
  format: yaml
  label: Arena Trading API
  slug: arena-predictions-com-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-trading-api-openapi.yml
- filename: arena-predictions-com-usage-api-openapi.yml
  format: yaml
  label: Arena Usage API
  slug: arena-predictions-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-usage-api-openapi.yml
consequence_counts:
  physical: 3
  read: 29
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Arena Predictions Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api_keys/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /portfolio/orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/orders/{orderId}/amend
operation_count: 37
overview: 'Arena exposes 37 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 4 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Arena
provider_slug: arena-predictions-com
slug: arena-predictions-com-agentic-access
source_filename: arena-predictions-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/arena-predictions-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 29\n    acting: 8\n  by_consequence:\n    read: 29\n    write: 4\n    safety-critical: 1\n    physical: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n\
  \  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys/{id}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n     \
  \ purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api_keys/{id}/rotate\n  method: post\n  operationId: rotateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leaderboard\n  method: get\n  operationId: getLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - records:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /traders/{traderId}\n  method: get\n  operationId: getTrader\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - records:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /traders/{traderId}/picks\n  method: get\n  operationId: getTraderPicks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - records:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /traders/{traderId}/track-record\n  method: get\n  operationId: getTraderTrackRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - records:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eval\n  method: get\n  operationId: getEvalBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - records:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/eval\n  method: get\n  operationId: getMyEval\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - portfolio:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/scoreboard\n  method: get\n  operationId: getMyScoreboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - portfolio:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - portfolio:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments\n  method: get\n  operationId: listInstruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/search\n  method: get\n  operationId: searchInstruments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/{ref}\n  method: get\n  operationId: getInstrument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/{ref}/quotes\n  method: get\n  operationId: getInstrumentQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/{ref}/book\n  method: get\n  operationId: getInstrumentBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotes\n  method: get\n  operationId: getQuotes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /games\n  method: get\n  operationId: listGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /games/{ref}\n  method: get\n  operationId: getGame\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio\n  method: get\n  operationId: getPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - portfolio:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/trades\n  method: get\n  operationId: listTrades\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - portfolio:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - trade:write\n    - trade:write:kalshi\n    - trade:write:poly-intl\n    - trade:write:prophetx\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/orders/{orderId}\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - trade:write\n    - trade:write:kalshi\n    - trade:write:poly-intl\n    - trade:write:prophetx\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/orders/{orderId}/amend\n  method: post\n  operationId: amendLiveOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - trade:write:kalshi\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /backtest\n  method: post\n  operationId: runBacktest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - markets:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /evals\n  method: post\n  operationId: createEval\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - markets:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs\n  method: get\n  operationId: listRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs/{run_id}\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history\n  method: get\n  operationId: getHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/candles\n  method: get\n  operationId: getHistoryCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/as_of\n  method: get\n  operationId: getHistoryAsOf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/export\n  method: get\n  operationId: exportHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - markets:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/arena-predictions-com/agentic-access/arena-predictions-com-agentic-access.yml
summary_line: 37 operations · 8 acting · 1 human-in-the-loop
tags:
- Prediction Markets
- Paper Trading
- Sandbox
- CLI
---
