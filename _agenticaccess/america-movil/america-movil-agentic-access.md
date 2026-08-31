---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 1
api_specs:
- filename: america-movil-check-sim-swap-api-openapi.yml
  format: yaml
  label: América Móvil Check SIM swap API
  slug: america-movil-check-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-check-sim-swap-api-openapi.yml
- filename: america-movil-device-locations-api-openapi.yml
  format: yaml
  label: América Móvil Device Locations API
  slug: america-movil-device-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-device-locations-api-openapi.yml
- filename: america-movil-location-verification-api-openapi.yml
  format: yaml
  label: América Móvil Location verification API
  slug: america-movil-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-location-verification-api-openapi.yml
- filename: america-movil-retrieve-sim-swap-date-api-openapi.yml
  format: yaml
  label: América Móvil Retrieve SIM swap date API
  slug: america-movil-retrieve-sim-swap-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-retrieve-sim-swap-date-api-openapi.yml
consequence_counts:
  read: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: America Movil Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'América Móvil exposes 4 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: América Móvil
provider_slug: america-movil
slug: america-movil-agentic-access
source_filename: america-movil-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/america-movil-claro-device-location-openapi.json, openapi/america-movil-claro-device-location-verify-camara-openapi.yaml,\n  openapi/america-movil-claro-sim-swap-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 1\n    acting: 3\n  by_consequence:\n    read: 1\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /lbs/devices/locations\n  method: get\n  operationId: device-locations-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify\n  method: post\n  operationId: verifyLocation\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - device-location-read\n- path: /retrieve-date\n  method: post\n  operationId: retrieveSimSwapDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - retrieve-sim-swap-date\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check\n  method: post\n  operationId: checkSimSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - check-sim-swap\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/agentic-access/america-movil-agentic-access.yml
summary_line: 4 operations · 3 acting
tags:
- Telecommunications
- Mexico
- Latin America
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- Device Location
- Broadband
- 5G
- Carrier
---
