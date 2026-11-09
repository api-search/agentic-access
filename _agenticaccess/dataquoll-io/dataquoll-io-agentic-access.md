---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 27
api_specs:
- filename: dataquoll-io-addresses-api-openapi.yml
  format: yaml
  label: DataQuoll Addresses API
  slug: dataquoll-io-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-addresses-api-openapi.yml
- filename: dataquoll-io-calendars-api-openapi.yml
  format: yaml
  label: DataQuoll Calendars API
  slug: dataquoll-io-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-calendars-api-openapi.yml
- filename: dataquoll-io-declarations-api-openapi.yml
  format: yaml
  label: DataQuoll Declarations API
  slug: dataquoll-io-declarations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-declarations-api-openapi.yml
- filename: dataquoll-io-events-api-openapi.yml
  format: yaml
  label: DataQuoll Events API
  slug: dataquoll-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-events-api-openapi.yml
- filename: dataquoll-io-facilities-api-openapi.yml
  format: yaml
  label: DataQuoll Facilities API
  slug: dataquoll-io-facilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-facilities-api-openapi.yml
- filename: dataquoll-io-gauges-api-openapi.yml
  format: yaml
  label: DataQuoll Gauges API
  slug: dataquoll-io-gauges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-gauges-api-openapi.yml
- filename: dataquoll-io-hazard-history-api-openapi.yml
  format: yaml
  label: DataQuoll Hazard history API
  slug: dataquoll-io-hazard-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-hazard-history-api-openapi.yml
- filename: dataquoll-io-incidents-api-openapi.yml
  format: yaml
  label: DataQuoll Incidents API
  slug: dataquoll-io-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-incidents-api-openapi.yml
- filename: dataquoll-io-meta-api-openapi.yml
  format: yaml
  label: DataQuoll Meta API
  slug: dataquoll-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-meta-api-openapi.yml
- filename: dataquoll-io-mobile-sites-api-openapi.yml
  format: yaml
  label: DataQuoll Mobile sites API
  slug: dataquoll-io-mobile-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-mobile-sites-api-openapi.yml
- filename: dataquoll-io-publications-api-openapi.yml
  format: yaml
  label: DataQuoll Publications API
  slug: dataquoll-io-publications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-publications-api-openapi.yml
consequence_counts:
  read: 27
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dataquoll Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'DataQuoll exposes 29 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DataQuoll
provider_slug: dataquoll-io
slug: dataquoll-io-agentic-access
source_filename: dataquoll-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dataquoll-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 27\n    acting: 2\n  by_consequence:\n    read: 27\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/incidents\n  method: get\n  operationId: listIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/incidents/{id}\n  method: get\n  operationId: getIncident\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/incidents/nearby\n\
  \  method: get\n  operationId: nearbyIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/incidents/snapshot\n  method: get\n  operationId: incidentSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/incidents/history\n  method: get\n  operationId: listHistoricalIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/states\n  method: get\n  operationId: listStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/declarations/postcode/{postcode}\n  method: get\n  operationId: declarationsByPostcode\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/declarations/point\n  method: post\n  operationId: declarationsByPoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hazard-history/point\n  method: post\n  operationId: hazardHistoryByPoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/declarations\n  method: get\n  operationId: listDeclarations\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/declarations/agrn/{agrn}\n  method: get\n  operationId: declarationByAgrn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/status\n  method: get\n  operationId: apiStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attribution\n  method: get\n  operationId: getAttribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events/{id}\n  method:\
  \ get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/schema\n  method: get\n  operationId: getSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gauges\n  method: get\n  operationId: listGauges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gauges/{id}\n  method: get\n  operationId: getGauge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gauges/{id}/readings\n  method: get\n  operationId: listGaugeReadings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gauges/summary\n  method: get\n  operationId: getGaugeSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/facilities\n  method: get\n  operationId: listFacilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/address\n  method: post\n  operationId: lookupAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/mobile-sites\n  method: get\n  operationId: listMobileSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calendars\n  method: get\n  operationId: listCalendars\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calendars/{jurisdiction}\n  method: get\n  operationId: getCalendarDays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calendars/{jurisdiction}/{date}\n  method: get\n  operationId: getCalendarDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/publications\n  method: get\n  operationId: listPublications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/publications/{id}\n  method: get\n  operationId: getPublication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/publishers\n  method: get\n  operationId: listPublishers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dataquoll-io/agentic-access/dataquoll-io-agentic-access.yml
summary_line: 29 operations · 2 acting
tags:
- Company
- Data
- Emergency
- Australia
- Public Data
---
