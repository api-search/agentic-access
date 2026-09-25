---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 31
api_specs:
- filename: kronos-seshat-agent-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Agent API
  slug: kronos-seshat-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-agent-api-openapi.yml
- filename: kronos-seshat-agent-intelligence-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Agent Intelligence API
  slug: kronos-seshat-agent-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-agent-intelligence-api-openapi.yml
- filename: kronos-seshat-analysis-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Analysis API
  slug: kronos-seshat-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-analysis-api-openapi.yml
- filename: kronos-seshat-discovery-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Discovery API
  slug: kronos-seshat-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-discovery-api-openapi.yml
- filename: kronos-seshat-experimental-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Experimental API
  slug: kronos-seshat-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-experimental-api-openapi.yml
- filename: kronos-seshat-forecast-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Forecast API
  slug: kronos-seshat-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-forecast-api-openapi.yml
- filename: kronos-seshat-market-intelligence-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Market Intelligence API
  slug: kronos-seshat-market-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-market-intelligence-api-openapi.yml
- filename: kronos-seshat-semantic-similarity-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Semantic Similarity API
  slug: kronos-seshat-semantic-similarity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-semantic-similarity-api-openapi.yml
- filename: kronos-seshat-signal-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Signal API
  slug: kronos-seshat-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-signal-api-openapi.yml
- filename: kronos-seshat-verification-api-openapi.yml
  format: yaml
  label: Kronos Quant Signal API Verification API
  slug: kronos-seshat-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/openapi/kronos-seshat-verification-api-openapi.yml
consequence_counts:
  read: 31
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kronos Seshat Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Kronos Quant Signal API exposes 32 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kronos Quant Signal API
provider_slug: kronos-seshat
slug: kronos-seshat-agentic-access
source_filename: kronos-seshat-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: generated\nsource: openapi/kronos-seshat-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 31\n    acting: 1\n  by_consequence:\n    read: 31\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /feeds/kronos/catalog\n  method: get\n  operationId: getKronosCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/sample/btc_usdt\n  method: get\n  operationId: getKronosSample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /feeds/kronos/accuracy-preview/{symbolKey}\n  method: get\n  operationId: kronos_accuracy_preview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/accuracy\n  method: get\n  operationId: getKronosAccuracy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/accuracy/candles\n  method: get\n  operationId: kronos_accuracy_candles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/accuracy/candles-preview\n  method: get\n  operationId: kronos_accuracy_candles_preview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/conviction-signals\n\
  \  method: get\n  operationId: kronos_conviction_signals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/risk\n  method: get\n  operationId: getKronosRisk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/risk/history\n  method: get\n  operationId: kronos_risk_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/predict/{symbolKey}\n  method: get\n  operationId: getKronosPrediction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/decision/{decisionId}\n  method: get\n  operationId: getKronosDecision\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/decisions\n  method: get\n  operationId: getKronosDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/forecast-evolution/{symbolKey}\n  method: get\n  operationId: getForecastEvolution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/forecast-distribution/{symbolKey}\n  method: get\n  operationId: getKronosForecastDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/historical-analogs/{symbolKey}\n  method: get\n  operationId: getHistoricalAnalogs\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/regime\n  method: get\n  operationId: getKronosRegime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/agent/track-record\n  method: get\n  operationId: getKronosAgentTrackRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/agent/votes\n  method: get\n  operationId: getKronosAgentVotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/agent/signals\n  method: get\n  operationId: getKronosAgentSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/composite-preview/{symbolKey}\n  method: get\n  operationId: kronos_composite_preview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/composite/{symbolKey}\n  method: get\n  operationId: getKronosComposite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/confluence/{symbolKey}\n  method: get\n  operationId: kronos_confluence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/benchmark-preview\n  method: get\n  operationId: kronos_benchmark_preview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/benchmark\n  method: get\n  operationId: kronos_benchmark\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/digest/{symbolKey}\n  method: get\n  operationId: kronos_digest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/market-brief/{symbolKey}\n  method: get\n  operationId: kronos_market_brief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/similar-markets\n  method: get\n  operationId: similar_markets_text\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/similar-markets/outcome-stats\n\
  \  method: get\n  operationId: similar_markets_outcome_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/agent-intelligence/behavioral-correlations\n  method: get\n  operationId: behavioral_correlations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/agent-intelligence/rationale-novelty\n  method: get\n  operationId: rationale_novelty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/market-context/{symbolKey}\n  method: get\n  operationId: kronos_market_context\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/kronos/playground/{symbolKey}\n\
  \  method: post\n  operationId: runKronosPlayground\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kronos-seshat/refs/heads/main/agentic-access/kronos-seshat-agentic-access.yml
summary_line: 32 operations · 1 acting
tags:
- Crypto
- Financial Forecast
- API
- Market Data
- Auditing
- Micropayments
---
