---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 57
api_specs:
- filename: prereason-com-agent-access-api-openapi.yml
  format: yaml
  label: prereason-com Agent access API
  slug: prereason-com-agent-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-agent-access-api-openapi.yml
- filename: prereason-com-company-briefings-api-openapi.yml
  format: yaml
  label: prereason-com Company Briefings API
  slug: prereason-com-company-briefings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-company-briefings-api-openapi.yml
- filename: prereason-com-context-api-openapi.yml
  format: yaml
  label: prereason-com Context API
  slug: prereason-com-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-context-api-openapi.yml
- filename: prereason-com-metrics-api-openapi.yml
  format: yaml
  label: prereason-com Metrics API
  slug: prereason-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-metrics-api-openapi.yml
- filename: prereason-com-short-urls-api-openapi.yml
  format: yaml
  label: prereason-com Short URLs API
  slug: prereason-com-short-urls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-short-urls-api-openapi.yml
- filename: prereason-com-system-api-openapi.yml
  format: yaml
  label: prereason-com System API
  slug: prereason-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-system-api-openapi.yml
- filename: prereason-com-treasury-holdings-api-openapi.yml
  format: yaml
  label: prereason-com Treasury Holdings API
  slug: prereason-com-treasury-holdings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-treasury-holdings-api-openapi.yml
- filename: prereason-com-webhooks-api-openapi.yml
  format: yaml
  label: prereason-com Webhooks API
  slug: prereason-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prereason-com/openapi/prereason-com-webhooks-api-openapi.yml
consequence_counts:
  read: 57
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Prereason Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 59
overview: 'prereason-com exposes 59 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 57 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: prereason-com
provider_slug: prereason-com
slug: prereason-com-agentic-access
source_filename: prereason-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/prereason-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 59\n  by_action_class:\n    connected: 57\n    acting: 2\n  by_consequence:\n    read: 57\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/btc\n  method: get\n  operationId: shortBtc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/context\n  method: get\n  operationId: shortBtcContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/pulse\n  method: get\n  operationId:\
  \ shortBtcPulse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/grid\n  method: get\n  operationId: shortBtcGrid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/momentum\n  method: get\n  operationId: shortBtcMomentum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/onchain\n  method: get\n  operationId: shortBtcOnchain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/miners\n  method: get\n  operationId: shortBtcMiners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /api/btc/etf\n  method: get\n  operationId: shortBtcEtf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/full\n  method: get\n  operationId: shortBtcFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/factors\n  method: get\n  operationId: shortBtcFactors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/energy\n  method: get\n  operationId: shortBtcEnergy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/btc/treasury\n  method: get\n  operationId: shortBtcTreasury\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/macro\n  method: get\n  operationId: shortMacro\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/macro/liquidity\n  method: get\n  operationId: shortMacroLiquidity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/macro/rates\n  method: get\n  operationId: shortMacroRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cross/correlations\n  method: get\n  operationId: shortCrossCorrelations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/cross/breadth\n  method: get\n  operationId: shortCrossBreadth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cross/regime\n  method: get\n  operationId: shortCrossRegime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fx\n  method: get\n  operationId: shortFx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/treasuries\n  method: get\n  operationId: listTreasuryHoldings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cross/ai-compute\n  method: get\n  operationId: shortCrossAiCompute\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commodities/energy-basket\n  method: get\n  operationId: shortCommoditiesEnergyBasket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/macro/auctions\n  method: get\n  operationId: shortMacroAuctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/macro/calendar\n  method: get\n  operationId: shortMacroCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bonds/context\n  method: get\n  operationId: shortBondsContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/bonds/full\n  method: get\n  operationId: shortBondsFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/eth/context\n  method: get\n  operationId: shortEthContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commodities/gold\n  method: get\n  operationId: shortCommoditiesGold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commodities/silver\n  method: get\n  operationId: shortCommoditiesSilver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commodities/copper\n  method: get\n  operationId: shortCommoditiesCopper\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commodities/wheat\n  method: get\n  operationId: shortCommoditiesWheat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commodities/oil-producers\n  method: get\n  operationId: shortCommoditiesOilProducers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commodities/gold-miners\n  method: get\n  operationId: shortCommoditiesGoldMiners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commodities/grains-agribusiness\n  method: get\n  operationId: shortCommoditiesGrainsAgribusiness\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/treasuries/{ticker}\n  method: get\n  operationId: getTreasuryHolding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/metrics/{metric}\n  method: get\n  operationId: getMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/companies/{company}\n  method: get\n  operationId: getCompanyBriefing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/companies/{company}/{block}\n  method: get\n  operationId: getCompanyBriefingBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/events\n  method: get\n  operationId: getChangeEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/news\n  method: get\n  operationId: getNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/context\n  method: get\n  operationId: getContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/companies\n  method: get\n  operationId: listCoveredCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/briefings\n  method: get\n  operationId: listBriefingsAlias\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/briefings/{id}\n  method: get\n  operationId: getBriefingById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/context/briefings\n  method: get\n  operationId: listBriefings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/metrics\n  method: get\n  operationId: listMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/metrics/bitcoin-price/history\n  method: get\n  operationId: getBtcPriceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n \
  \ method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health/ready\n  method: get\n  operationId: getHealthReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/version\n  method: get\n  operationId: getVersionConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/headline\n  method: get\n  operationId: getHeadline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/openapi/spec.json\n  method: get\n  operationId: getOpenApiJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openapi/spec.yaml\n  method: get\n  operationId: getOpenApiYaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openapi/ui\n  method: get\n  operationId: getOpenApiUi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openapi/status\n  method: get\n  operationId: getOpenApiStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: mcpEndpoint\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/claims\n  method: post\n  operationId: createAgentClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/claims/{code}\n  method: get\n  operationId: pollAgentClaim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/prereason-com/agentic-access/prereason-com-agentic-access.yml
summary_line: 59 operations · 2 acting
tags:
- Finance
- Markets
- Artificial Intelligence
- Data
- MCP
---
