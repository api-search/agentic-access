---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: tier-mobility-gbfs-openapi.yml
  format: yaml
  label: TIER / Dott GBFS API
  slug: tier-mobility-gbfs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-gbfs-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tier Mobility Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'TIER exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TIER
provider_slug: tier-mobility
slug: tier-mobility-agentic-access
source_filename: tier-mobility-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tier-mobility-gbfs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /gbfs_versions.json\n  method: get\n  operationId: listGbfsVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{system_id}/gbfs.json\n  method: get\n  operationId: getGbfsDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{system_id}/system_information.json\n\
  \  method: get\n  operationId: getSystemInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{system_id}/system_pricing_plans.json\n  method: get\n  operationId: getSystemPricingPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{system_id}/vehicle_types.json\n  method: get\n  operationId: getVehicleTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{system_id}/free_bike_status.json\n  method: get\n  operationId: getFreeBikeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{system_id}/station_information.json\n  method: get\n  operationId: getStationInformation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{system_id}/station_status.json\n  method: get\n  operationId: getStationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{system_id}/geofencing_zones.json\n  method: get\n  operationId: getGeofencingZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/agentic-access/tier-mobility-agentic-access.yml
summary_line: 9 operations
tags:
- Mobility
- Micromobility
- Shared Mobility
- E-Scooter
- E-Bike
- Transportation
- Smart Cities
- MaaS
- GBFS
- Open Data
- Europe
- Real-Time
---
