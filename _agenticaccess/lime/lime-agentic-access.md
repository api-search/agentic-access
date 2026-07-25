---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: lime-free-bike-status-api-openapi.yml
  format: yaml
  label: Lime Free Bike Status API
  slug: lime-free-bike-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-free-bike-status-api-openapi.yml
- filename: lime-gbfs-json-api-openapi.yml
  format: yaml
  label: Lime Gbfs.json API
  slug: lime-gbfs-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-gbfs-json-api-openapi.yml
- filename: lime-station-information-api-openapi.yml
  format: yaml
  label: Lime Station Information API
  slug: lime-station-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-station-information-api-openapi.yml
- filename: lime-station-status-api-openapi.yml
  format: yaml
  label: Lime Station Status API
  slug: lime-station-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-station-status-api-openapi.yml
- filename: lime-system-information-api-openapi.yml
  format: yaml
  label: Lime System Information API
  slug: lime-system-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-system-information-api-openapi.yml
- filename: lime-vehicle-types-api-openapi.yml
  format: yaml
  label: Lime Vehicle Types API
  slug: lime-vehicle-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-vehicle-types-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lime Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Lime exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lime
provider_slug: lime
slug: lime-agentic-access
source_filename: lime-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lime-gbfs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /gbfs.json\n  method: get\n  operationId: getGbfsDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system_information\n  method: get\n  operationId: getSystemInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicle_types\n  method: get\n  operationId: getVehicleTypes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /station_information\n  method: get\n  operationId: getStationInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /station_status\n  method: get\n  operationId: getStationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free_bike_status\n  method: get\n  operationId: getFreeBikeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/agentic-access/lime-agentic-access.yml
summary_line: 6 operations
tags:
- Shared Mobility
- Micromobility
- Electric Scooters
- Electric Bikes
- E-Bikes
- E-Scooters
- Transportation
- Urban Mobility
- GBFS
- MDS
- Smart Cities
- Transit
---
