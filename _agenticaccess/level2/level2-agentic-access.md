---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: level2-strategy-builder-openapi.yml
  format: yaml
  label: Level2 Strategy Builder API
  slug: strategy-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-strategy-builder-openapi.yml
- filename: level2-tradestation-integration-openapi.yml
  format: yaml
  label: Level2 TradeStation Integration API
  slug: tradestation-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-tradestation-integration-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Level2 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /broker/users/{userId}/strategies/{strategyId}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /broker/users/{userId}/strategies/{strategyId}/deploy
operation_count: 15
overview: 'level2 exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 5 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: level2
provider_slug: level2
slug: level2-agentic-access
source_filename: level2-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/level2-strategy-builder-openapi.yml, openapi/level2-tradestation-integration-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 8\n    acting: 7\n  by_consequence:\n    read: 8\n    write: 5\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /checkForCandlestick/{api_key}/{ticker}/{timeframe}\n  method: get\n  operationId: checkForCandlestick\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getTickerTrend/{api_key}/{ticker}/{timeframe}\n  method: get\n  operationId: getTickerTrend\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /olhc/{api_key}/{ticker}/{timeframe}/{range}\n  method: get\n  operationId: getOHLCData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /similar/{api_key}/{ticker}\n  method: get\n  operationId: getSimilarStocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summary/{api_key}/{ticker}\n  method: get\n  operationId: getCompanySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/users\n  method: post\n  operationId: createBrokerUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/users/{userId}\n  method: get\n  operationId: getBrokerUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/users/{userId}/strategies\n  method: get\n  operationId: listUserStrategies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/users/{userId}/strategies\n  method: post\n  operationId: createUserStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /broker/users/{userId}/strategies/{strategyId}\n  method: get\n  operationId: getUserStrategy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/users/{userId}/strategies/{strategyId}\n  method: put\n  operationId: updateUserStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/users/{userId}/strategies/{strategyId}\n  method: delete\n  operationId: deleteUserStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /broker/users/{userId}/strategies/{strategyId}/deploy\n  method: post\n  operationId: deployUserStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/users/{userId}/strategies/{strategyId}/stop\n  method: post\n  operationId: stopUserStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /broker/users/{userId}/strategies/{strategyId}/backtest\n  method: post\n  operationId: backtestUserStrategy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/agentic-access/level2-agentic-access.yml
summary_line: 15 operations · 7 acting · 1 human-in-the-loop
tags: []
---
