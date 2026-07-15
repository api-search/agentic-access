---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: redfin-stingray-api-openapi.yml
  format: yaml
  label: Redfin Stingray API
  slug: redfin-stingray-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-stingray-api-openapi.yml
- filename: redfin-gis-csv-api-openapi.yml
  format: yaml
  label: Redfin GIS CSV Export API
  slug: redfin-gis-csv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-gis-csv-api-openapi.yml
- filename: redfin-data-center-openapi.yml
  format: yaml
  label: Redfin Data Center
  slug: redfin-data-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/openapi/redfin-data-center-openapi.yml
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Redfin Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Redfin exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Redfin
provider_slug: redfin
slug: redfin-agentic-access
source_filename: redfin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/redfin-data-center-openapi.yml, openapi/redfin-gis-csv-api-openapi.yml, openapi/redfin-stingray-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /redfin_market_tracker/us_national_market_tracker.tsv000.gz\n  method: get\n  operationId: downloadNationalMarketTracker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redfin_market_tracker/redfin_metro_market_tracker.tsv000.gz\n  method: get\n  operationId: downloadMetroMarketTracker\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redfin_market_tracker/state_market_tracker.tsv000.gz\n  method: get\n  operationId: downloadStateMarketTracker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redfin_market_tracker/county_market_tracker.tsv000.gz\n  method: get\n  operationId: downloadCountyMarketTracker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redfin_market_tracker/city_market_tracker.tsv000.gz\n  method: get\n  operationId: downloadCityMarketTracker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redfin_market_tracker/zip_code_market_tracker.tsv000.gz\n  method:\
  \ get\n  operationId: downloadZipCodeMarketTracker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redfin_market_tracker/neighborhood_market_tracker.tsv000.gz\n  method: get\n  operationId: downloadNeighborhoodMarketTracker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gis-csv\n  method: get\n  operationId: exportGisCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /do/gis-search\n  method: get\n  operationId: gisSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gis\n  method: get\n  operationId: gisApiSearch\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/home/details/initialInfo\n  method: get\n  operationId: getInitialInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/home/details/aboveTheFold\n  method: get\n  operationId: getAboveTheFold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/home/details/belowTheFold\n  method: get\n  operationId: getBelowTheFold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/home/details/mainHouseInfoPanelInfo\n  method: get\n  operationId: getMainHouseInfoPanelInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/home/details/avmHistoricalData\n  method: get\n  operationId: getAvmHistoricalData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/home/details/neighborhoodStats/statsInfo\n  method: get\n  operationId: getNeighborhoodStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/home/details/commute/commuteInfo\n  method: get\n  operationId: getCommuteInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/region/{regionType}/{regionId}/{code}/trends\n  method: get\n  operationId: getRegionTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/region/{regionType}/{regionId}/{code}/aggregate-trends\n  method: get\n  operationId: getRegionAggregateTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redfin/refs/heads/main/agentic-access/redfin-agentic-access.yml
summary_line: 19 operations
tags:
- CSV Export
- GIS
- Home Values
- Housing Market
- Listings
- Property Data
- Real Estate
---
