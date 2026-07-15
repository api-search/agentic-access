---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: data-retrieval-api.json
  format: json
  label: CO-OPS Data Retrieval API
  slug: co-ops-data-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/data-retrieval-api.json
- filename: metadata-api.json
  format: json
  label: CO-OPS Metadata API
  slug: co-ops-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/metadata-api.json
- filename: derived-product-api.json
  format: json
  label: CO-OPS Derived Product API
  slug: co-ops-derived-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/derived-product-api.json
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Noaa Co Ops Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'NOAA CO-OPS exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NOAA CO-OPS
provider_slug: noaa-co-ops
slug: noaa-co-ops-agentic-access
source_filename: noaa-co-ops-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/data-retrieval-api.json, openapi/derived-product-api.json, openapi/metadata-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /datagetter\n  method: get\n  operationId: getData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /toptenwaterlevels\n  method: get\n  operationId: getTopTenWaterLevels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /peakwaterlevels\n  method: get\n  operationId: getPeakWaterLevels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extremewaterlevels\n  method: get\n  operationId: getExtremeWaterLevels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sealvltrends\n  method: get\n  operationId: getSeaLevelTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /slr_projections\n  method: get\n  operationId: getSeaLevelRiseProjections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /htf_annual\n  method: get\n  operationId: getHighTideFloodingAnnual\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /htf_monthly\n  method: get\n  operationId: getHighTideFloodingMonthly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /htf_projection_decadal\n  method: get\n  operationId: getHighTideFloodingProjectionDecadal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /benchmarks\n  method: get\n  operationId: getBenchmarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations.json\n  method: get\n  operationId: listStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /stations/{stationId}.json\n  method: get\n  operationId: getStation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{stationId}/{resource}.json\n  method: get\n  operationId: getStationResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ports.json\n  method: get\n  operationId: listPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/agentic-access/noaa-co-ops-agentic-access.yml
summary_line: 14 operations
tags:
- NOAA
- Tides
- Currents
- Oceanographic
- Water Level
- Weather
- Predictions
- Government
---
