---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: airlabs-airlines-api-openapi.yml
  format: yaml
  label: Airlabs Airlines API
  slug: airlabs-airlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-airlines-api-openapi.yml
- filename: airlabs-airports-api-openapi.yml
  format: yaml
  label: Airlabs Airports API
  slug: airlabs-airports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-airports-api-openapi.yml
- filename: airlabs-alert-api-openapi.yml
  format: yaml
  label: Airlabs Alert API
  slug: airlabs-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-alert-api-openapi.yml
- filename: airlabs-cities-api-openapi.yml
  format: yaml
  label: Airlabs Cities API
  slug: airlabs-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-cities-api-openapi.yml
- filename: airlabs-delays-api-openapi.yml
  format: yaml
  label: Airlabs Delays API
  slug: airlabs-delays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-delays-api-openapi.yml
- filename: airlabs-fleets-api-openapi.yml
  format: yaml
  label: Airlabs Fleets API
  slug: airlabs-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-fleets-api-openapi.yml
- filename: airlabs-flight-api-openapi.yml
  format: yaml
  label: Airlabs Flight API
  slug: airlabs-flight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-flight-api-openapi.yml
- filename: airlabs-flights-api-openapi.yml
  format: yaml
  label: Airlabs Flights API
  slug: airlabs-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-flights-api-openapi.yml
- filename: airlabs-nearby-api-openapi.yml
  format: yaml
  label: Airlabs Nearby API
  slug: airlabs-nearby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-nearby-api-openapi.yml
- filename: airlabs-routes-api-openapi.yml
  format: yaml
  label: Airlabs Routes API
  slug: airlabs-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-routes-api-openapi.yml
- filename: airlabs-schedules-api-openapi.yml
  format: yaml
  label: Airlabs Schedules API
  slug: airlabs-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-schedules-api-openapi.yml
- filename: airlabs-suggest-api-openapi.yml
  format: yaml
  label: Airlabs Suggest API
  slug: airlabs-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/openapi/airlabs-suggest-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Airlabs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Airlabs exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Airlabs
provider_slug: airlabs
slug: airlabs-agentic-access
source_filename: airlabs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /flights\n  method: get\n  operationId: flights_flights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedules\n  method: get\n  operationId: schedules_schedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delays\n  method: get\n  operationId: delays_delays\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flight\n  method: get\n  operationId: flight_flight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert\n  method: get\n  operationId: alert_flight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nearby\n  method: get\n  operationId: nearby_nearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suggest\n  method: get\n  operationId: suggest_suggestenvelope\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airlines\n  method: get\n\
  \  operationId: airlines_airlines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports\n  method: get\n  operationId: airports_airports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cities\n  method: get\n  operationId: cities_cities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fleets\n  method: get\n  operationId: fleets_fleets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes\n  method: get\n  operationId: routes_routes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airlabs/refs/heads/main/agentic-access/airlabs-agentic-access.yml
summary_line: 12 operations
tags:
- Aviation
- Flights
- Airlines
- Airports
- Flight Tracking
- Flight Status
- Real-time Data
---
