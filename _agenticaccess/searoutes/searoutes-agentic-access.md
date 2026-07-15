---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 30
api_specs:
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Ocean Routing API
  slug: searoutes-ocean-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Geocoding API
  slug: searoutes-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes CO2 Emissions API
  slug: searoutes-co2-emissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Vessel Tracking API
  slug: searoutes-vessel-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Search & Carriers API
  slug: searoutes-search-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Weather API
  slug: searoutes-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
consequence_counts:
  read: 30
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Searoutes Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Searoutes exposes 32 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Searoutes
provider_slug: searoutes
slug: searoutes-agentic-access
source_filename: searoutes-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/searoutes-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 30\n    acting: 2\n  by_consequence:\n    read: 30\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /route/v2/sea/{locations}\n  method: get\n  operationId: getSeaRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /route/v2/sea/{locations}/plan\n  method: get\n  operationId: getSeaRoutePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocoding/v2/all\n\
  \  method: get\n  operationId: geocodeAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocoding/v2/port\n  method: get\n  operationId: geocodePort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocoding/v2/airport\n  method: get\n  operationId: geocodeAirport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocoding/v2/area\n  method: get\n  operationId: geocodeArea\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocoding/v2/zip\n  method: get\n  operationId: geocodeZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocoding/v2/closest\n  method: get\n  operationId: geocodeClosest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocoding/v2/place\n  method: get\n  operationId: geocodePlace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/v2/shipment\n  method: get\n  operationId: getShipmentCo2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/v2/vessel\n  method: get\n  operationId: getVesselCo2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/v2/road\n  method: get\n  operationId: getRoadCo2\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/v2/rail\n  method: get\n  operationId: getRailCo2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/v2/aircraft\n  method: get\n  operationId: getAircraftCo2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/v2/inland-water\n  method: get\n  operationId: getInlandWaterCo2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/v2/run\n  method: post\n  operationId: getMilkRunCo2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co2/v2/plan\n  method: get\n  operationId: getPlanCo2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/v2/proformas/{hash}\n  method: get\n  operationId: getProformaCo2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/v2/execution/{hash}\n  method: get\n  operationId: getExecutionCo2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/v2/position\n  method: get\n  operationId: getVesselPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /vessel/v2/eta\n  method: get\n  operationId: getVesselEta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/v2/arrivals\n  method: get\n  operationId: getVesselArrivals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/v2/name\n  method: get\n  operationId: searchVesselByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/v2/timeseries\n  method: get\n  operationId: getVesselTimeseries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/v2/trace\n  method: get\n  operationId: getVesselTrace\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/v2/carriers\n  method: get\n  operationId: searchCarriers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/v2/carrier/{id}\n  method: get\n  operationId: getCarrier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/v2/service\n  method: get\n  operationId: searchServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/v2/service/{id}\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /weather/v2/forecast\n  method: get\n  operationId: getWeatherForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /weather/v2/historical\n  method: get\n  operationId: getWeatherHistorical\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /weather/v2/track\n  method: post\n  operationId: getWeatherAlongTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/agentic-access/searoutes-agentic-access.yml
summary_line: 32 operations · 2 acting
tags:
- Maritime
- Sea Routing
- Ocean Freight
- CO2 Emissions
- Carbon Accounting
- Vessel Tracking
- AIS
- Geocoding
- Logistics
- Supply Chain
---
