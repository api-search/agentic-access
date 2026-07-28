---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: aeso-poolprice-api-v1-1-openapi.json
  format: json
  label: AESO Pool Price Report API
  slug: aeso-pool-price-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-poolprice-api-v1-1-openapi.json
- filename: aeso-systemmarginalprice-api-v1-1-openapi.json
  format: json
  label: AESO System Marginal Price Report API
  slug: aeso-system-marginal-price-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-systemmarginalprice-api-v1-1-openapi.json
- filename: aeso-currentsupplydemand-api-v2-openapi.json
  format: json
  label: AESO Current Supply Demand API (v2)
  slug: aeso-current-supply-demand-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-currentsupplydemand-api-v2-openapi.json
- filename: aeso-currentsupplydemand-api-v1-openapi.json
  format: json
  label: AESO Current Supply Demand API (v1)
  slug: aeso-current-supply-demand-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-currentsupplydemand-api-v1-openapi.json
- filename: aeso-actualforecast-api-v1-openapi.json
  format: json
  label: AESO Actual Forecast Report API
  slug: aeso-actual-forecast-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-actualforecast-api-v1-openapi.json
- filename: aeso-aiesgencapacity-api-v1-openapi.json
  format: json
  label: AESO AIES Gen Capacity API
  slug: aeso-aies-gen-capacity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-aiesgencapacity-api-v1-openapi.json
- filename: aeso-loadoutageforecast-api-v1-openapi.json
  format: json
  label: AESO Load Outage Forecast API
  slug: aeso-load-outage-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-loadoutageforecast-api-v1-openapi.json
- filename: aeso-itc-api-v1-openapi.json
  format: json
  label: AESO Intertie Public Reports API
  slug: aeso-intertie-public-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-itc-api-v1-openapi.json
- filename: aeso-energymeritorder-api-v1-openapi.json
  format: json
  label: AESO Energy Merit Order Report API
  slug: aeso-energy-merit-order-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-energymeritorder-api-v1-openapi.json
- filename: aeso-meteredvolume-api-v1-openapi.json
  format: json
  label: AESO Metered Volume Report API
  slug: aeso-metered-volume-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-meteredvolume-api-v1-openapi.json
- filename: aeso-operatingreserveoffercontrol-api-v1-openapi.json
  format: json
  label: AESO Operating Reserve Offer Control Report API
  slug: aeso-operating-reserve-offer-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-operatingreserveoffercontrol-api-v1-openapi.json
- filename: aeso-assetlist-api-v1-openapi.json
  format: json
  label: AESO Asset List API
  slug: aeso-asset-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-assetlist-api-v1-openapi.json
- filename: aeso-poolparticipant-api-v1-openapi.json
  format: json
  label: AESO Pool Participant API
  slug: aeso-pool-participant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-poolparticipant-api-v1-openapi.json
- filename: aeso-unitcommitmentdata-api-v2-openapi.json
  format: json
  label: AESO Unit Commitment Data API
  slug: aeso-unit-commitment-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/openapi/aeso-unitcommitmentdata-api-v2-openapi.json
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aeso Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'AESO exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AESO
provider_slug: aeso
slug: aeso-agentic-access
source_filename: aeso-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/aeso-actualforecast-api-v1-openapi.json, openapi/aeso-aiesgencapacity-api-v1-openapi.json,\n  openapi/aeso-assetlist-api-v1-openapi.json, openapi/aeso-currentsupplydemand-api-v1-openapi.json,\n  openapi/aeso-currentsupplydemand-api-v2-openapi.json, openapi/aeso-energymeritorder-api-v1-openapi.json,\n  openapi/aeso-itc-api-v1-openapi.json, openapi/aeso-loadoutageforecast-api-v1-openapi.json,\n  openapi/aeso-meteredvolume-api-v1-openapi.json, openapi/aeso-operatingreserveoffercontrol-api-v1-openapi.json,\n  openapi/aeso-poolparticipant-api-v1-openapi.json, openapi/aeso-poolprice-api-v1-1-openapi.json,\n  openapi/aeso-systemmarginalprice-api-v1-1-openapi.json, openapi/aeso-unitcommitmentdata-api-v2-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment.\
  \ See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /load/albertaInternalLoad\n  method: get\n  operationId: getActualForecastReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AIESGenCapacity\n  method: get\n  operationId: getAIESControlReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assetlist\n  method: get\n  operationId: getAssetListData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /csd/generation/assets/current\n  method: get\n  operationId: getCSDReportByAsset\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /csd/summary/current\n  method: get\n  operationId: getCSDSummaryDataReportv2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meritOrder/energy\n  method: get\n  operationId: getMeritOrderReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outage\n  method: get\n  operationId: getOutages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interchange\n  method: get\n  operationId: getReportByRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loadOutageReport\n\
  \  method: get\n  operationId: getLoadOutageRangeReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meteredvolume/details\n  method: get\n  operationId: getMeteredVolumeReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operatingReserveOfferControl\n  method: get\n  operationId: getOperatingReserveOfferControlReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /poolparticipantlist\n  method: get\n  operationId: getPoolParticipantListData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price/poolPrice\n  method: get\n  operationId: getPoolPriceDateRangeReport\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price/systemMarginalPrice\n  method: get\n  operationId: getSystemMarginalPriceReportForDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price/systemMarginalPrice/current\n  method: get\n  operationId: getCurrentSystemMarginalPriceReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unitCommitment\n  method: get\n  operationId: getUnitCommitmentDataReportV11ForDateRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeso/refs/heads/main/agentic-access/aeso-agentic-access.yml
summary_line: 16 operations
tags:
- Energy
- Canada
- Alberta
- Electricity
- Energy Markets
- Grid
- System Operator
- Market Operator
- Open Energy Data
- Wholesale Power
- Demand Response
- Renewables
- Utilities
---
