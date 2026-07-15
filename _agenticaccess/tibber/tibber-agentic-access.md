---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: tibber-graphql-api-openapi.yml
  format: yaml
  label: Tibber GraphQL API
  slug: tibber-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/openapi/tibber-graphql-api-openapi.yml
- filename: tibber-data-api-openapi.yml
  format: yaml
  label: Tibber Data API
  slug: tibber-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/openapi/tibber-data-api-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tibber Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Tibber exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tibber
provider_slug: tibber
slug: tibber-agentic-access
source_filename: tibber-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tibber-data-api-openapi.yml, openapi/tibber-graphql-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/homes\n  method: get\n  operationId: listHomes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/homes/{homeId}/devices\n  method: get\n  operationId: listDevicesForHome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/homes/{homeId}/devices/{deviceId}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/homes/{homeId}/devices/{deviceId}/history\n  method: get\n  operationId: getDeviceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gql\n  method: post\n  operationId: executeGraphQL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/agentic-access/tibber-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Energy
- SmartHome
- SmartMeter
- ElectricityPricing
- ElectricVehicleCharging
- HeatPump
- SolarInverter
- HomeBattery
- GraphQL
- OAuth2
- Nordic
---
