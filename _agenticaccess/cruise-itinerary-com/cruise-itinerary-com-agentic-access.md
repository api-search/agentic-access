---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 23
api_specs:
- filename: cruise-itinerary-com-bulk-exports-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Bulk exports API
  slug: cruise-itinerary-com-bulk-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-bulk-exports-api-openapi.yml
- filename: cruise-itinerary-com-changes-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Changes API
  slug: cruise-itinerary-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-changes-api-openapi.yml
- filename: cruise-itinerary-com-cruise-itinerary-data-api-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Cruise Itinerary Data API
  slug: cruise-itinerary-com-cruise-itinerary-data-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-cruise-itinerary-data-api-api-openapi.yml
- filename: cruise-itinerary-com-price-index-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Price index API
  slug: cruise-itinerary-com-price-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-price-index-api-openapi.yml
- filename: cruise-itinerary-com-reference-data-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Reference data API
  slug: cruise-itinerary-com-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-reference-data-api-openapi.yml
- filename: cruise-itinerary-com-resolver-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Resolver API
  slug: cruise-itinerary-com-resolver-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-resolver-api-openapi.yml
- filename: cruise-itinerary-com-sailings-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Sailings API
  slug: cruise-itinerary-com-sailings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-sailings-api-openapi.yml
- filename: cruise-itinerary-com-service-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Service API
  slug: cruise-itinerary-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-service-api-openapi.yml
- filename: cruise-itinerary-com-ships-and-ports-api-openapi.yml
  format: yaml
  label: cruise-itinerary-com Ships and ports API
  slug: cruise-itinerary-com-ships-and-ports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cruise-itinerary-com/openapi/cruise-itinerary-com-ships-and-ports-api-openapi.yml
consequence_counts:
  read: 23
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cruise Itinerary Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'cruise-itinerary-com exposes 24 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: cruise-itinerary-com
provider_slug: cruise-itinerary-com
slug: cruise-itinerary-com-agentic-access
source_filename: cruise-itinerary-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/cruise-itinerary-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 23\n    acting: 1\n  by_consequence:\n    read: 23\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lines\n  method: get\n  operationId: listLines\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lines/{id}\n  method: get\n  operationId: getLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ships\n  method: get\n  operationId: listShips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ships/{id}\n  method: get\n  operationId: getShip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ports\n  method: get\n  operationId: listPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ports/{id}\n\
  \  method: get\n  operationId: getPort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/destinations\n  method: get\n  operationId: listDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/regions\n  method: get\n  operationId: listRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resolve\n  method: get\n  operationId: resolve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resolve\n  method: post\n  operationId: resolveBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/price-index/latest\n  method: get\n  operationId: getPriceIndexLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sailings\n  method: get\n  operationId: listSailings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sailings/{id}\n  method: get\n  operationId: getSailing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sailings/{id}/prices\n  method: get\n  operationId: getSailingPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cruises/{id}\n  method: get\n  operationId: getCruise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ships/{id}/schedule\n  method: get\n  operationId: getShipSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ports/{id}/calendar\n  method: get\n  operationId: getPortCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ports/{id}/days/{date}\n  method: get\n  operationId: getPortDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/changes\n  method: get\n  operationId: listChanges\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price-index\n  method: get\n  operationId: getPriceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exports\n  method: get\n  operationId: listExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exports/{date}/{file}\n  method: get\n  operationId: downloadExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cruise-itinerary-com/agentic-access/cruise-itinerary-com-agentic-access.yml
summary_line: 24 operations · 1 acting
tags:
- Company
- Travel
- Data
- Cruise
---
