---
acting_count: 0
action_class_counts:
  connected: 23
api_specs:
- filename: pyth-hermes-openapi-original.json
  format: json
  label: Pyth Hermes (Pyth Core)
  slug: pyth-hermes-pyth-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pyth/refs/heads/main/openapi/pyth-hermes-openapi-original.json
- filename: pyth-benchmarks-openapi-original.json
  format: json
  label: Pyth Benchmarks
  slug: pyth-benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pyth/refs/heads/main/openapi/pyth-benchmarks-openapi-original.json
consequence_counts:
  read: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pyth Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Pyth exposes 23 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pyth
provider_slug: pyth
slug: pyth-agentic-access
source_filename: pyth-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/pyth-benchmarks-openapi-original.json, openapi/pyth-hermes-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 23\n  by_consequence:\n    read: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/shims/tradingview/history\n  method: get\n  operationId: tradingview_history_route_v1_shims_tradingview_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shims/tradingview/groups\n  method: get\n  operationId: get_groups_v1_shims_tradingview_groups_get\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shims/tradingview/symbol_info\n  method: get\n  operationId: get_symbol_info_v1_shims_tradingview_symbol_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shims/tradingview/symbols\n  method: get\n  operationId: tradingview_symbols_route_v1_shims_tradingview_symbols_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shims/tradingview/search\n  method: get\n  operationId: tradingview_search_route_v1_shims_tradingview_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shims/tradingview/config\n  method: get\n  operationId: tradingview_config_route_v1_shims_tradingview_config_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shims/tradingview/streaming\n  method: get\n  operationId: tradingview_streaming_route_v1_shims_tradingview_streaming_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price_feeds/\n  method: get\n  operationId: price_feeds_route_v1_price_feeds__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price_feeds/{id}\n  method: get\n  operationId: price_feed_route_v1_price_feeds__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price_differences/\n  method: get\n  operationId: price_differences_route_v1_price_differences__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/updates/price/{timestamp}\n  method: get\n  operationId: price_updates_timestamp_route_v1_updates_price__timestamp__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/updates/price/{timestamp}/{interval}\n  method: get\n  operationId: price_updates_interval_route_v1_updates_price__timestamp___interval__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get_price_feed\n  method: get\n  operationId: get_price_feed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get_vaa\n  method: get\n  operationId: get_vaa\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get_vaa_ccip\n  method: get\n  operationId: get_vaa_ccip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/latest_price_feeds\n  method: get\n  operationId: latest_price_feeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/latest_vaas\n  method: get\n  operationId: latest_vaas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/price_feed_ids\n  method: get\n  operationId: price_feed_ids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/price_feeds\n  method: get\n  operationId: price_feeds_metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/updates/price/latest\n  method: get\n  operationId: latest_price_updates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/updates/price/stream\n  method: get\n  operationId: price_stream_sse_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/updates/price/{publish_time}\n  method: get\n  operationId: timestamp_price_updates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/updates/publisher_stake_caps/latest\n\
  \  method: get\n  operationId: latest_publisher_stake_caps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pyth/refs/heads/main/agentic-access/pyth-agentic-access.yml
summary_line: 23 operations
tags:
- Company
- Crypto Web3
- Oracle
- Price Feeds
- Market Data
- DeFi
- Blockchain
- Financial Data
---
