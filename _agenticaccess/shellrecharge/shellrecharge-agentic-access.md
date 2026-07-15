---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge EV Public Locations API
  slug: shellrecharge-public-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge EV Public Charge Sessions API
  slug: shellrecharge-public-charge-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge OCPI API
  slug: shellrecharge-ocpi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge Tariffs API
  slug: shellrecharge-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge Tokens API
  slug: shellrecharge-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  safety-critical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Shellrecharge Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /mobility-ev-api/v1/api/charge-sessions/stop/{sessionId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mobility-ev-api/v1/api/charge-sessions/start
operation_count: 8
overview: 'ShellRecharge exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ShellRecharge
provider_slug: shellrecharge
slug: shellrecharge-agentic-access
source_filename: shellrecharge-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/shellrecharge-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 6\n    acting: 2\n  by_consequence:\n    read: 6\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /ev/v2/locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ev/v2/locations/{uid}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /ev/v2/locations/nearby\n  method: get\n  operationId: getNearbyLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ev/v2/locations/markers\n  method: get\n  operationId: getLocationMarkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobility-ev-api/v1/api/charge-sessions/start\n  method: post\n  operationId: startChargeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobility-ev-api/v1/api/charge-sessions/retrieve/{sessionId}\n  method: get\n  operationId: retrieveChargeSession\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mobility-ev-api/v1/api/charge-sessions/stop/{sessionId}\n  method: post\n  operationId: stopChargeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mobility-ev-api/v1/api/charge-sessions/active\n  method: get\n  operationId: listActiveChargeSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/agentic-access/shellrecharge-agentic-access.yml
summary_line: 8 operations · 2 acting · 1 human-in-the-loop
tags:
- EV Charging
- Electric Vehicles
- Mobility
- Charge Points
- OCPI
- Energy
---
