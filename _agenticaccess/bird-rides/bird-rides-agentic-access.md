---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: bird-gbfs-openapi.yml
  format: yaml
  label: Bird GBFS Feed
  slug: bird-gbfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-rides/refs/heads/main/openapi/bird-gbfs-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bird Rides Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Bird exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bird
provider_slug: bird-rides
slug: bird-rides-agentic-access
source_filename: bird-rides-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bird-gbfs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /gbfs.json\n  method: get\n  operationId: getGbfsDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gbfs_versions.json\n  method: get\n  operationId: getGbfsVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system_information.json\n  method: get\n  operationId:\
  \ getSystemInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicle_types.json\n  method: get\n  operationId: getVehicleTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free_bike_status.json\n  method: get\n  operationId: getFreeBikeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /station_information.json\n  method: get\n  operationId: getStationInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /station_status.json\n  method: get\n  operationId: getStationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geofencing_zones.json\n  method: get\n  operationId: getGeofencingZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system_pricing_plans.json\n  method: get\n  operationId: getSystemPricingPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system_regions.json\n  method: get\n  operationId: getSystemRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bird-rides/refs/heads/main/agentic-access/bird-rides-agentic-access.yml
summary_line: 10 operations
tags:
- Micromobility
- Shared Mobility
- Electric Scooters
- E-Scooters
- E-Bikes
- Bikeshare
- Transportation
- Urban Mobility
- GBFS
- General Bikeshare Feed Specification
- Mobility Data Specification
- MDS
- Geofencing
- Cities
- Smart Cities
- Fleet Management
- Third Lane Mobility
---
