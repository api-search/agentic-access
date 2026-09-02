---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: glassnode-addresses-api-openapi.yml
  format: yaml
  label: Glassnode Addresses API
  slug: glassnode-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-addresses-api-openapi.yml
- filename: glassnode-derivatives-api-openapi.yml
  format: yaml
  label: Glassnode Derivatives API
  slug: glassnode-derivatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-derivatives-api-openapi.yml
- filename: glassnode-distribution-api-openapi.yml
  format: yaml
  label: Glassnode Distribution API
  slug: glassnode-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-distribution-api-openapi.yml
- filename: glassnode-indicators-api-openapi.yml
  format: yaml
  label: Glassnode Indicators API
  slug: glassnode-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-indicators-api-openapi.yml
- filename: glassnode-macro-api-openapi.yml
  format: yaml
  label: Glassnode Macro API
  slug: glassnode-macro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-macro-api-openapi.yml
- filename: glassnode-market-api-openapi.yml
  format: yaml
  label: Glassnode Market API
  slug: glassnode-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-market-api-openapi.yml
- filename: glassnode-metadata-api-openapi.yml
  format: yaml
  label: Glassnode Metadata API
  slug: glassnode-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-metadata-api-openapi.yml
- filename: glassnode-options-api-openapi.yml
  format: yaml
  label: Glassnode Options API
  slug: glassnode-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-options-api-openapi.yml
- filename: glassnode-supply-api-openapi.yml
  format: yaml
  label: Glassnode Supply API
  slug: glassnode-supply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-supply-api-openapi.yml
- filename: glassnode-transactions-api-openapi.yml
  format: yaml
  label: Glassnode Transactions API
  slug: glassnode-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-transactions-api-openapi.yml
- filename: glassnode-treasuries-api-openapi.yml
  format: yaml
  label: Glassnode Treasuries API
  slug: glassnode-treasuries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-treasuries-api-openapi.yml
- filename: glassnode-user-api-openapi.yml
  format: yaml
  label: Glassnode User API
  slug: glassnode-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-user-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Glassnode Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Glassnode exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Glassnode
provider_slug: glassnode
slug: glassnode-agentic-access
source_filename: glassnode-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/glassnode-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/metadata/metric\n  method: get\n  operationId: getMetricMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/metrics\n  method: get\n  operationId: listMetricsMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metadata/assets\n  method: get\n  operationId:\
  \ listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/api_usage\n  method: get\n  operationId: getApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/addresses/active_count\n  method: get\n  operationId: getAddressesActiveCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/transactions/transfers_volume_sum\n  method: get\n  operationId: getTransactionsTransfersVolumeSum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/supply/active_1d_1w\n  method: get\n  operationId: getSupplyActive1d1w\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/market/marketcap_usd\n  method: get\n  operationId: getMarketcapUsd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/indicators/net_unrealized_profit_loss\n  method: get\n  operationId: getNupl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/derivatives/futures_open_interest_sum\n  method: get\n  operationId: getFuturesOpenInterestSum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/options/options_gamma_exposure\n  method: get\n  operationId: getOptionsGammaExposure\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/distribution/balance_exchanges\n  method: get\n  operationId: getDistributionBalanceExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/treasuries/balance_companies\n  method: get\n  operationId: getTreasuriesBalanceCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics/macro/us_money_supply_m2\n  method: get\n  operationId: getMacroUsM2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/agentic-access/glassnode-agentic-access.yml
summary_line: 14 operations
tags:
- Web3
- Crypto
- Onchain
- Analytics
- Metrics
- Bitcoin
- Ethereum
- Institutional
---
