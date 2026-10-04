---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 37
api_specs:
- filename: messari-ai-api-openapi.yml
  format: yaml
  label: Messari AI API
  slug: messari-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-ai-api-openapi.yml
- filename: messari-assets-api-openapi.yml
  format: yaml
  label: Messari Assets API
  slug: messari-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-assets-api-openapi.yml
- filename: messari-datasets-api-openapi.yml
  format: yaml
  label: Messari Datasets API
  slug: messari-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-datasets-api-openapi.yml
- filename: messari-exchanges-api-openapi.yml
  format: yaml
  label: Messari Exchanges API
  slug: messari-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-exchanges-api-openapi.yml
- filename: messari-markets-api-openapi.yml
  format: yaml
  label: Messari Markets API
  slug: messari-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-markets-api-openapi.yml
- filename: messari-monitoring-api-openapi.yml
  format: yaml
  label: Messari Monitoring API
  slug: messari-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-monitoring-api-openapi.yml
- filename: messari-networks-api-openapi.yml
  format: yaml
  label: Messari Networks API
  slug: messari-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-networks-api-openapi.yml
- filename: messari-news-api-openapi.yml
  format: yaml
  label: Messari News API
  slug: messari-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-news-api-openapi.yml
- filename: messari-protocols-api-openapi.yml
  format: yaml
  label: Messari Protocols API
  slug: messari-protocols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-protocols-api-openapi.yml
- filename: messari-research-api-openapi.yml
  format: yaml
  label: Messari Research API
  slug: messari-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-research-api-openapi.yml
- filename: messari-token-unlocks-api-openapi.yml
  format: yaml
  label: Messari Token Unlocks API
  slug: messari-token-unlocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-token-unlocks-api-openapi.yml
consequence_counts:
  read: 37
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Messari Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /openai/chat-completions
operation_count: 42
overview: 'Messari exposes 42 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Messari
provider_slug: messari
slug: messari-agentic-access
source_filename: messari-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/messari-ai-api-openapi.yml, openapi/messari-assets-api-openapi.yml, openapi/messari-datasets-api-openapi.yml,\n  openapi/messari-exchanges-api-openapi.yml, openapi/messari-markets-api-openapi.yml, openapi/messari-monitoring-api-openapi.yml,\n  openapi/messari-networks-api-openapi.yml, openapi/messari-news-api-openapi.yml, openapi/messari-protocols-api-openapi.yml,\n  openapi/messari-research-api-openapi.yml, openapi/messari-token-unlocks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 5\n    connected: 37\n  by_consequence:\n    write: 4\n    safety-critical: 1\n    read: 37\n  human_in_the_loop_required: 1\noperations:\n- path: /chat-completions\n\
  \  method: post\n  operationId: postChatCompletions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/chat-completions\n  method: post\n  operationId: postOpenaiChatCompletions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/deep-research\n  method: post\n  operationId: postV1DeepResearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deep-research\n  method: get\n  operationId: getV1DeepResearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deep-research/{id}\n  method: get\n  operationId: getV1DeepResearchById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets\n  method: get\n  operationId: getV1Assets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/{assetIdentifier}\n  method: get\n  operationId: getV1AssetsByAssetIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/assets/{asset}/metrics\n  method: get\n  operationId: getV1AssetsByAssetMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/{asset}/timeseries/{metric}\n  method: get\n  operationId: getV1AssetsByAssetTimeseriesByMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets\n  method: get\n  operationId: getV2Assets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/{ids}/details\n  method: get\n  operationId: getV2AssetsByIdsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/{asset}/time-series/{metric}\n  method: get\n\
  \  operationId: getV2AssetsByAssetTimeSeriesByMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets\n  method: get\n  operationId: getV1Datasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{slug}/{granularity}/data\n  method: get\n  operationId: getV1DatasetsBySlugByGranularityData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchanges\n  method: get\n  operationId: getExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchanges/{exchange}\n  method: get\n  operationId: getExchangesByExchange\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets\n  method: get\n  operationId: getV1Markets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/{marketIdentifier}\n  method: get\n  operationId: getV1MarketsByMarketIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/{market}/metrics\n  method: get\n  operationId: getV1MarketsByMarketMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/{market}/timeseries/{metric}\n  method: get\n  operationId: getV1MarketsByMarketTimeseriesByMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitoring-views\n  method: get\n  operationId: getV2MonitoringViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists\n  method: get\n  operationId: getV1Watchlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists\n  method: post\n  operationId: postV1Watchlists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{id}\n  method: patch\n  operationId: patchV1WatchlistsById\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/networks\n  method: get\n  operationId: getV2Networks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/networks/{network}/metrics\n  method: get\n  operationId: getV2NetworksByNetworkMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/networks/{network}/timeseries/{metric}\n  method: get\n  operationId: getV2NetworksByNetworkTimeseriesByMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/news-feed\n  method: get\n\
  \  operationId: getV1NewsFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/news-sources\n  method: get\n  operationId: getV1NewsSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: post\n  operationId: postV1Events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/developments\n  method: get\n  operationId: getV2Developments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/events\n  method: get\n  operationId: getV2Events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /protocols\n  method: get\n  operationId: getProtocols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /protocols/{protocol}/metrics\n  method: get\n  operationId: getProtocolsByProtocolMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dex\n  method: get\n  operationId: getDex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lending\n  method: get\n  operationId: getLending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liquid-staking\n  method: get\n  operationId: getLiquidStaking\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports\n  method: get\n  operationId: getV1Reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/{reportId}\n  method: get\n  operationId: getV1ReportsByReportId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/tags\n  method: get\n  operationId: getV1ReportsTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/{assetId}/unlocks\n  method: get\n  operationId: getV1AssetsByAssetIdUnlocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v1/assets/{assetId}/vesting-schedule\n  method: get\n  operationId: getV1AssetsByAssetIdVestingSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/agentic-access/messari-agentic-access.yml
summary_line: 42 operations · 5 acting · 1 human-in-the-loop
tags:
- Web3
- Crypto
- Research
- Analytics
- Asset Data
- Fundamentals
- News
- Token Unlocks
---
