---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 21
api_specs:
- filename: openapi.json
  format: json
  label: ADS-B Exchange Aircraft API
  slug: ads-b-exchange-aircraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/openapi/openapi.json
consequence_counts:
  read: 21
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adsbexchange Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'ADS-B Exchange exposes 30 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ADS-B Exchange
provider_slug: adsbexchange
slug: adsbexchange-agentic-access
source_filename: adsbexchange-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 21\n    acting: 9\n  by_consequence:\n    read: 21\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /all\n  method: get\n  operationId: GetApiAircraftV2All\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /total-aircraft\n  method: get\n  operationId: GetApiAircraftV2TotalAircraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /filter\n  method: post\n  operationId:\
  \ PostApiAircraftV2Filter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hex/{hex}\n  method: get\n  operationId: GetApiAircraftV2Hex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hex\n  method: post\n  operationId: PostApiAircraftV2Hex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /icao/{icao}\n  method: get\n  operationId: GetApiAircraftV2Icao\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /icao\n  method: post\n  operationId: PostApiAircraftV2Icao\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mil\n  method: get\n  operationId: GetApiAircraftV2Mil\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /callsign/{callsign}\n  method: get\n  operationId: GetApiAircraftV2Callsign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registration/{registration}\n  method: get\n  operationId: GetApiAircraftV2Registration\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registration\n  method: post\n  operationId: PostApiAircraftV2Registration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sqk/{squawk}\n  method: get\n  operationId: GetApiAircraftV2Sqk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lat/{lat}/lon/{lon}/dist/{dist}\n  method: get\n  operationId: GetApiAircraftV2LatLonDist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proximity/radius\n  method: post\n  operationId: PostApiAircraftV2ProximityRadius\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /minimal/lat/{lat}/lon/{lon}/dist/{dist}\n  method: get\n  operationId: GetApiAircraftV2MinimalLatLonDist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nohex/dist/{dist}/above/{alt}/lat/{lat}/lon/{lon}\n  method: get\n  operationId: GetApiAircraftV2NohexDistAboveLatLon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airport/{airport}\n  method: get\n  operationId: GetApiAircraftV2Airport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /airport\n  method: post\n  operationId: PostApiAircraftV2Airport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geospatial/boundary\n  method: post\n  operationId: PostApiAircraftV2GeospatialBoundary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geospatial/country/{country}\n  method: get\n  operationId: GetApiAircraftV2GeospatialCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /geospatial/country/{country}/subdivisions\n  method: get\n  operationId: GetApiAircraftV2GeospatialCountrySubdivisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geospatial/country/{country}/subdivision/{subdivision}\n  method: get\n  operationId: GetApiAircraftV2GeospatialCountrySubdivision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geospatial/region/{region}\n  method: get\n  operationId: GetApiAircraftV2GeospatialRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geospatial/continent/{continent}\n  method: get\n  operationId: GetApiAircraftV2GeospatialContinent\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/icaos\n  method: post\n  operationId: PostApiAircraftV2OperationsIcaos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operations/icao/{icao}\n  method: get\n  operationId: GetApiAircraftV2OperationsIcao\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/airports\n  method: post\n  operationId: PostApiAircraftV2OperationsAirports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /operations/airport/{airport}\n  method: get\n  operationId: GetApiAircraftV2OperationsAirport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /traces/{folder}/{jsonFile}\n  method: get\n  operationId: GetApiAircraftV2Traces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /traces-hist/{year}/{month}/{day}/traces/{folder}/{jsonFile}\n  method: get\n  operationId: GetApiAircraftV2TracesHistTraces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adsbexchange/refs/heads/main/agentic-access/adsbexchange-agentic-access.yml
summary_line: 30 operations · 9 acting
tags:
- Aviation
- Flight Tracking
- ADS-B
- Aircraft
- Real-Time
- Military
- MLAT
---
