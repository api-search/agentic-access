---
acting_count: 0
action_class_counts:
  connected: 25
api_specs:
- filename: fluvigil-de-flood-situation-api-openapi.yml
  format: yaml
  label: Fluvigil Flood Situation API
  slug: fluvigil-de-flood-situation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-flood-situation-api-openapi.yml
- filename: fluvigil-de-health-api-openapi.yml
  format: yaml
  label: Fluvigil Health API
  slug: fluvigil-de-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-health-api-openapi.yml
- filename: fluvigil-de-me-api-openapi.yml
  format: yaml
  label: Fluvigil Me API
  slug: fluvigil-de-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-me-api-openapi.yml
- filename: fluvigil-de-rivers-api-openapi.yml
  format: yaml
  label: Fluvigil Rivers API
  slug: fluvigil-de-rivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-rivers-api-openapi.yml
- filename: fluvigil-de-sources-api-openapi.yml
  format: yaml
  label: Fluvigil Sources API
  slug: fluvigil-de-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-sources-api-openapi.yml
- filename: fluvigil-de-stations-api-openapi.yml
  format: yaml
  label: Fluvigil Stations API
  slug: fluvigil-de-stations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-stations-api-openapi.yml
- filename: fluvigil-de-stats-api-openapi.yml
  format: yaml
  label: Fluvigil Stats API
  slug: fluvigil-de-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluvigil-de/openapi/fluvigil-de-stats-api-openapi.yml
consequence_counts:
  read: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fluvigil De Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Fluvigil exposes 25 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fluvigil
provider_slug: fluvigil-de
slug: fluvigil-de-agentic-access
source_filename: fluvigil-de-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/fluvigil-de-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 25\n  by_consequence:\n    read: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /stations\n  method: get\n  operationId: listStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/map\n  method: get\n  operationId: listMapStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/stream\n  method: get\n  operationId: streamStationChanges\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources/visible\n  method: get\n  operationId: getVisibleStationSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources/stream\n  method: get\n  operationId: streamVisibleStationSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/state-timeline\n  method: get\n  operationId: getStationStateTimeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}\n  method: get\n  operationId: getStation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/by-slug/{slug}\n  method: get\n  operationId: getStationBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/readings\n  method: get\n  operationId: listStationReadings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/state\n  method: get\n  operationId: getStationState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/neighbors\n  method: get\n  operationId: listStationNeighbors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/history-context\n\
  \  method: get\n  operationId: getStationHistoryContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/analogue\n  method: get\n  operationId: getStationAnalogue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rivers/{slug}\n  method: get\n  operationId: getRiver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/routing\n  method: get\n  operationId: simulateStationRouting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/forecast\n  method: get\n  operationId: getStationForecast\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/report-text\n  method: get\n  operationId: getStationReportText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flood-situation/latest\n  method: get\n  operationId: getLatestFloodSituation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flood-situation/{date}\n  method: get\n  operationId: getFloodSituationByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/statistics\n  method: get\n  operationId: getStationStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /stations/{id}/year-over-year\n  method: get\n  operationId: getStationYearOverYear\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{id}/weather\n  method: get\n  operationId: getStationWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/fluvigil-de/agentic-access/fluvigil-de-agentic-access.yml
summary_line: 25 operations
tags:
- Water
- Environment
- Data
- API
- Germany
---
