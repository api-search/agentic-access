---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: myshiptracking-account-api-openapi.yml
  format: yaml
  label: MyShipTracking Account API
  slug: myshiptracking-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-account-api-openapi.yml
- filename: myshiptracking-ports-api-openapi.yml
  format: yaml
  label: MyShipTracking Ports API
  slug: myshiptracking-ports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-ports-api-openapi.yml
- filename: myshiptracking-vessels-api-openapi.yml
  format: yaml
  label: MyShipTracking Vessels API
  slug: myshiptracking-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/openapi/myshiptracking-vessels-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Myshiptracking Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'MyShipTracking exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MyShipTracking
provider_slug: myshiptracking
slug: myshiptracking-agentic-access
source_filename: myshiptracking-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/myshiptracking-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /vessel\n  method: get\n  operationId: getVesselStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/bulk\n  method: get\n  operationId: getVesselsBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/zone\n  method: get\n  operationId: getVesselsInZone\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/nearby\n  method: get\n  operationId: getVesselsNearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/track\n  method: get\n  operationId: getVesselTrack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel/search\n  method: get\n  operationId: searchVessels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /port\n  method: get\n  operationId: getPortDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /port/estimate\n  method: get\n  operationId: getPortEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /port/calls\n  method: get\n  operationId: getPortCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/info\n  method: get\n  operationId: getAccountInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myshiptracking/refs/heads/main/agentic-access/myshiptracking-agentic-access.yml
summary_line: 10 operations
tags:
- Vessel Tracking
- AIS
- Maritime
- Ship Tracking
- Real-Time Data
- Ships
- Port Calls
- Maritime Data
- Location
- Fleet Tracking
---
