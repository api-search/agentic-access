---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 22
api_specs:
- filename: tickerbot-io-bars-api-openapi.yml
  format: yaml
  label: tickerbot-io Bars API
  slug: tickerbot-io-bars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-bars-api-openapi.yml
- filename: tickerbot-io-devices-api-openapi.yml
  format: yaml
  label: tickerbot-io Devices API
  slug: tickerbot-io-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-devices-api-openapi.yml
- filename: tickerbot-io-etf-api-openapi.yml
  format: yaml
  label: tickerbot-io ETF API
  slug: tickerbot-io-etf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-etf-api-openapi.yml
- filename: tickerbot-io-events-api-openapi.yml
  format: yaml
  label: tickerbot-io Events API
  slug: tickerbot-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-events-api-openapi.yml
- filename: tickerbot-io-meta-api-openapi.yml
  format: yaml
  label: tickerbot-io Meta API
  slug: tickerbot-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-meta-api-openapi.yml
- filename: tickerbot-io-news-api-openapi.yml
  format: yaml
  label: tickerbot-io News API
  slug: tickerbot-io-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-news-api-openapi.yml
- filename: tickerbot-io-scan-api-openapi.yml
  format: yaml
  label: tickerbot-io Scan API
  slug: tickerbot-io-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-scan-api-openapi.yml
- filename: tickerbot-io-series-api-openapi.yml
  format: yaml
  label: tickerbot-io Series API
  slug: tickerbot-io-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-series-api-openapi.yml
- filename: tickerbot-io-signals-api-openapi.yml
  format: yaml
  label: tickerbot-io Signals API
  slug: tickerbot-io-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-signals-api-openapi.yml
- filename: tickerbot-io-tickers-api-openapi.yml
  format: yaml
  label: tickerbot-io Tickers API
  slug: tickerbot-io-tickers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-tickers-api-openapi.yml
- filename: tickerbot-io-universes-api-openapi.yml
  format: yaml
  label: tickerbot-io Universes API
  slug: tickerbot-io-universes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-universes-api-openapi.yml
- filename: tickerbot-io-webhooks-api-openapi.yml
  format: yaml
  label: tickerbot-io Webhooks API
  slug: tickerbot-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-webhooks-api-openapi.yml
- filename: tickerbot-io-websockets-api-openapi.yml
  format: yaml
  label: tickerbot-io WebSockets API
  slug: tickerbot-io-websockets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerbot-io/openapi/tickerbot-io-websockets-api-openapi.yml
consequence_counts:
  physical: 2
  read: 22
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Tickerbot Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/webhooks/{id}/enable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/webhooks/{id}/deliveries/{delivery_id}/redeliver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/webhooks/{id}/test
operation_count: 41
overview: 'tickerbot-io exposes 41 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 16 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tickerbot-io
provider_slug: tickerbot-io
slug: tickerbot-io-agentic-access
source_filename: tickerbot-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/tickerbot-io-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 22\n    acting: 19\n  by_consequence:\n    read: 22\n    write: 16\n    safety-critical: 1\n    physical: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /v2/tickers\n  method: get\n  operationId: list_tickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tickers/{ticker}\n  method: get\n  operationId: get_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/bars/{ticker}/{interval}\n  method: get\n  operationId: get_bars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tickers/{ticker}/coverage\n  method: get\n  operationId: get_ticker_coverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/etf/{ticker}/holdings\n  method: get\n  operationId: get_etf_holdings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/etf/{ticker}/sectors\n  method: get\n  operationId: get_etf_sectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stream/usage\n  method: get\n  operationId: get_stream_usage\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tickers/{ticker}/subscribe\n  method: post\n  operationId: subscribe_ticker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/signals\n  method: get\n  operationId: list_signals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/signals\n  method: post\n  operationId: create_custom_signal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/signals/{signal}\n  method: get\n  operationId: get_signal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/signals/{signal}\n  method: patch\n  operationId: update_custom_signal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/signals/{signal}\n  method: delete\n  operationId: delete_custom_signal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /v2/signals/{signal}/subscribe\n  method: post\n  operationId: subscribe_signal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/scan\n  method: get\n  operationId: get_scan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/scan\n  method: post\n  operationId: scan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/scan/subscribe\n  method: post\n  operationId: subscribe_scan\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/news\n  method: get\n  operationId: search_news\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks\n  method: post\n  operationId: create_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks\n  method: get\n  operationId: list_webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/webhooks/{id}\n  method: get\n  operationId: get_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{id}\n  method: patch\n  operationId: update_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{id}\n  method: delete\n  operationId: delete_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{id}/deliveries\n  method: get\n\
  \  operationId: list_webhook_deliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{id}/enable\n  method: post\n  operationId: enable_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/webhooks/{id}/test\n  method: post\n  operationId: test_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{id}/deliveries/{delivery_id}/redeliver\n\
  \  method: post\n  operationId: redeliver_webhook_delivery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/universes\n  method: get\n  operationId: list_universes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/universes\n  method: post\n  operationId: create_universe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/universes/system\n  method: get\n\
  \  operationId: list_system_universes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/universes/{id}\n  method: get\n  operationId: get_universe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/universes/{id}\n  method: patch\n  operationId: update_universe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/universes/{id}\n  method: delete\n  operationId: delete_universe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/devices/register\n  method: post\n  operationId: register_device\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/devices\n  method: get\n  operationId: list_devices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/devices/{device_id}\n  method: delete\n  operationId: delete_device\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /v2/series\n  method: get\n  operationId: get_series\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/events\n  method: get\n  operationId: list_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/events/subscribe\n  method: post\n  operationId: subscribe_events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/health\n  method: get\n  operationId: get_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/version\n  method: get\n  operationId: get_version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tickerbot-io/agentic-access/tickerbot-io-agentic-access.yml
summary_line: 41 operations · 19 acting · 1 human-in-the-loop
tags:
- Company
- Stock Market
- Real-Time Data
- Historical Data
- Financial-Agents
---
