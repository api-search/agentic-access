---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 29
api_specs:
- filename: shipfinder-ais-data-api-ais-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API AIS Dataset API
  slug: shipfinder-ais-data-api-ais-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-ais-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-china-coastline-warning-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API China Coastline Warning Dataset API
  slug: shipfinder-ais-data-api-china-coastline-warning-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-china-coastline-warning-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-event-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Event Dataset API
  slug: shipfinder-ais-data-api-event-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-event-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-history-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API History Dataset API
  slug: shipfinder-ais-data-api-history-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-history-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-meteorology-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Meteorology Dataset API
  slug: shipfinder-ais-data-api-meteorology-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-meteorology-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-prediction-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Prediction Dataset API
  slug: shipfinder-ais-data-api-prediction-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-prediction-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-voyage-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Voyage Dataset API
  slug: shipfinder-ais-data-api-voyage-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-voyage-dataset-api-openapi.yml
consequence_counts:
  read: 29
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shipfinder Ais Data Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'ShipFinder AIS Data API exposes 40 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ShipFinder AIS Data API
provider_slug: shipfinder-ais-data-api
slug: shipfinder-ais-data-api-agentic-access
source_filename: shipfinder-ais-data-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/shipfinder-ais-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 29\n    acting: 11\n  by_consequence:\n    read: 29\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/AIS/FleetPosition\n  method: get\n  operationId: getFleetPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/AIS/VesselFlagInfo\n  method: get\n  operationId: getVesselFlagInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v1/AIS/VesselPositionMulti\n  method: get\n  operationId: getVesselPositionMulti\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/AIS/VesselPositionSingle\n  method: get\n  operationId: getVesselPositionSingle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/AIS/VesselSearch\n  method: get\n  operationId: getVesselSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/AIS/VesselsInZone\n  method: get\n  operationId: getVesselsInZone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/AIS/VesselsNearby\n  method: get\n  operationId: getVesselsNearby\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Event/AddFleet\n  method: post\n  operationId: postAddFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/AddGeofence\n  method: post\n  operationId: postAddGeofence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/AddVesselSpeedAlert\n  method: post\n  operationId: postAddVesselSpeedAlert\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/AddVesselToFleet\n  method: post\n  operationId: postAddVesselToFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/DeleteFleet\n  method: post\n  operationId: postDeleteFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/DeleteFleetVessel\n  method: post\n  operationId:\
  \ postDeleteFleetVessel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/DeleteGeofence\n  method: delete\n  operationId: deleteGeofence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/DeleteVesselSpeedAlert\n  method: post\n  operationId: postDeleteVesselSpeedAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/Event/GetFleet\n  method: get\n  operationId: getFleet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Event/GetGeofence\n  method: get\n  operationId: getGeofence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Event/UpdateFleetInfo\n  method: post\n  operationId: postUpdateFleetInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/UpdateFleetVessel\n  method: post\n  operationId: postUpdateFleetVessel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/UpdateGeofence\n  method: post\n  operationId: postUpdateGeofence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Event/VesselSpeedAlertList\n  method: get\n  operationId: getVesselSpeedAlertList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/History/PortCallRecordsByPort\n  method: get\n  operationId: getPortCallRecordsByPort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/History/PortCallRecordsByVessel\n  method: get\n  operationId: getPortCallRecordsByVessel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/History/PortCallRecordsByVesselAtPort\n  method: get\n  operationId: getPortCallRecordsByVesselAtPort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/History/VesselCurrentPortCall\n  method: get\n  operationId: getVesselCurrentPortCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/History/VesselHistoryTrack\n  method: get\n  operationId: getVesselHistoryTrack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/History/VesselStsEvents\n  method: get\n  operationId: getVesselStsEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Meteorology/CycloneInfo\n  method: get\n  operationId: getCycloneInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Meteorology/CyclonesList\n  method: get\n  operationId: getCyclonesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Meteorology/MarineWeather\n  method: get\n  operationId: getMarineWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Meteorology/TideStationInfo\n\
  \  method: get\n  operationId: getTideStationInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Meteorology/TideStationList\n  method: get\n  operationId: getTideStationList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Prediction/ETA\n  method: get\n  operationId: getETA\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Prediction/RoutePlanPointToPoint\n  method: get\n  operationId: getRoutePlanPointToPoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Prediction/RoutePlanPortToPort\n  method: get\n  operationId: getRoutePlanPortToPort\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Voyage/PortAnchoredVessels\n  method: get\n  operationId: getPortAnchoredVessels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Voyage/PortBerthedVessels\n  method: get\n  operationId: getPortBerthedVessels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Voyage/PortExpectedArrivals\n  method: get\n  operationId: getPortExpectedArrivals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Voyage/PortInfo\n  method: get\n  operationId: getPortInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Warning/NavigationalWarnings\n  method: get\n  operationId: getNavigationalWarnings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/agentic-access/shipfinder-ais-data-api-agentic-access.yml
summary_line: 40 operations · 11 acting
tags:
- AIS
- Maritime Data
- Vessel Tracking
- Ship Tracking
- Vessel Data
- Historical AIS
- Geospatial
- GIS
- Logistics
- Supply Chain
- Weather
- Meteorology
- Trade
- Commodities
- Compliance
- Risk
- Event Streaming
- Webhook
---
