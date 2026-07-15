---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: marinetraffic-ais-openapi.yml
  format: yaml
  label: MarineTraffic AIS Vessel Tracking API
  slug: marinetraffic-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/openapi/marinetraffic-ais-openapi.yml
- filename: marinetraffic-ais-openapi.yml
  format: yaml
  label: MarineTraffic AIS Vessel Tracking API
  slug: marinetraffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/openapi/marinetraffic-ais-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Marinetraffic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'MarineTraffic exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MarineTraffic
provider_slug: marinetraffic
slug: marinetraffic-agentic-access
source_filename: marinetraffic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/marinetraffic-ais-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /exportvessel/{apikey}\n  method: get\n  operationId: getVesselDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exportvesseltrack/{apikey}\n  method: get\n  operationId: getVesselTrack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getexpectedarrivals/{apikey}\n\
  \  method: get\n  operationId: getExpectedArrivals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getportcalls/{apikey}\n  method: get\n  operationId: getPortCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getvesselpositions/{apikey}\n  method: get\n  operationId: getVesselPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/agentic-access/marinetraffic-agentic-access.yml
summary_line: 5 operations
tags:
- AIS
- Maritime
- Shipping
- Vessel Tracking
---
