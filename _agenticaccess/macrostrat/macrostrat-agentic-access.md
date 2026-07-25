---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: macrostrat-age-model-api-openapi.yml
  format: yaml
  label: Macrostrat Age Model API
  slug: macrostrat-age-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-age-model-api-openapi.yml
- filename: macrostrat-cartography-api-openapi.yml
  format: yaml
  label: Macrostrat Cartography API
  slug: macrostrat-cartography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-cartography-api-openapi.yml
- filename: macrostrat-columns-api-openapi.yml
  format: yaml
  label: Macrostrat Columns API
  slug: macrostrat-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-columns-api-openapi.yml
- filename: macrostrat-definitions-api-openapi.yml
  format: yaml
  label: Macrostrat Definitions API
  slug: macrostrat-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-definitions-api-openapi.yml
- filename: macrostrat-fossils-api-openapi.yml
  format: yaml
  label: Macrostrat Fossils API
  slug: macrostrat-fossils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-fossils-api-openapi.yml
- filename: macrostrat-geologic-maps-api-openapi.yml
  format: yaml
  label: Macrostrat Geologic Maps API
  slug: macrostrat-geologic-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-geologic-maps-api-openapi.yml
- filename: macrostrat-grids-api-openapi.yml
  format: yaml
  label: Macrostrat Grids API
  slug: macrostrat-grids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-grids-api-openapi.yml
- filename: macrostrat-measurements-api-openapi.yml
  format: yaml
  label: Macrostrat Measurements API
  slug: macrostrat-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-measurements-api-openapi.yml
- filename: macrostrat-meta-api-openapi.yml
  format: yaml
  label: Macrostrat Meta API
  slug: macrostrat-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-meta-api-openapi.yml
- filename: macrostrat-mobile-api-openapi.yml
  format: yaml
  label: Macrostrat Mobile API
  slug: macrostrat-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-mobile-api-openapi.yml
- filename: macrostrat-paleogeography-api-openapi.yml
  format: yaml
  label: Macrostrat Paleogeography API
  slug: macrostrat-paleogeography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-paleogeography-api-openapi.yml
- filename: macrostrat-sections-api-openapi.yml
  format: yaml
  label: Macrostrat Sections API
  slug: macrostrat-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-sections-api-openapi.yml
- filename: macrostrat-stats-api-openapi.yml
  format: yaml
  label: Macrostrat Stats API
  slug: macrostrat-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-stats-api-openapi.yml
- filename: macrostrat-units-api-openapi.yml
  format: yaml
  label: Macrostrat Units API
  slug: macrostrat-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-units-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Macrostrat Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Macrostrat exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Macrostrat
provider_slug: macrostrat
slug: macrostrat-agentic-access
source_filename: macrostrat-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/macrostrat-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /columns\n  method: get\n  operationId: getColumns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections\n  method: get\n  operationId: getSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /units\n  method: get\n  operationId: getUnits\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fossils\n  method: get\n  operationId: getFossils\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paleogeography\n  method: get\n  operationId: getPaleogeography\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geologic_units/map\n  method: get\n  operationId: getGeologicMapUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geologic_units/map/points\n\
  \  method: get\n  operationId: getGeologicMapPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geologic_units/map/legend\n  method: get\n  operationId: getGeologicMapLegend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /measurements\n  method: get\n  operationId: getMeasurements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /age_model\n  method: get\n  operationId: getAgeModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /defs\n  method: get\n  operationId: getDefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /carto\n  method: get\n  operationId: getCarto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grids\n  method: get\n  operationId: getGrids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobile\n  method: get\n  operationId: getMobile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta\n  method: get\n  operationId: getMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/agentic-access/macrostrat-agentic-access.yml
summary_line: 16 operations
tags:
- Geological Data
- Geology
- Rocks
- Paleontology
- Earth Science
---
