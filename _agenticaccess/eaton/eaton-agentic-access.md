---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 11
api_specs:
- filename: eaton-authorization-api-openapi.yml
  format: yaml
  label: Eaton Authorization API
  slug: eaton-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-authorization-api-openapi.yml
- filename: eaton-device-commands-api-openapi.yml
  format: yaml
  label: Eaton Device Commands API
  slug: eaton-device-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-device-commands-api-openapi.yml
- filename: eaton-devices-api-openapi.yml
  format: yaml
  label: Eaton Devices API
  slug: eaton-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-devices-api-openapi.yml
- filename: eaton-energy-data-api-openapi.yml
  format: yaml
  label: Eaton Energy Data API
  slug: eaton-energy-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-energy-data-api-openapi.yml
- filename: eaton-ev-only-api-openapi.yml
  format: yaml
  label: Eaton EV Only API
  slug: eaton-ev-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-ev-only-api-openapi.yml
- filename: eaton-events-api-openapi.yml
  format: yaml
  label: Eaton Events API
  slug: eaton-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-events-api-openapi.yml
- filename: eaton-locations-api-openapi.yml
  format: yaml
  label: Eaton Locations API
  slug: eaton-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-locations-api-openapi.yml
- filename: eaton-organizations-api-openapi.yml
  format: yaml
  label: Eaton Organizations API
  slug: eaton-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/openapi/eaton-organizations-api-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Eaton Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/deviceBatchCommands
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/devices/{deviceId}/commands
operation_count: 15
overview: 'Eaton exposes 15 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Eaton
provider_slug: eaton
slug: eaton-agentic-access
source_filename: eaton-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smart-breaker-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 4\n    connected: 11\n  by_consequence:\n    write: 2\n    read: 11\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth2/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/{organizationId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/locations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/locations/{locationId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/devices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/devices/{deviceId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v1/devices/{deviceId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/devices/{deviceId}/state\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/devices/{deviceId}/commands\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/deviceBatchCommands\n \
  \ method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/devices/{deviceId}/energy\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/devices/{deviceId}/events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ev/{deviceId}/sessions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ev/{deviceId}/sessions/{sessionId}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eaton/refs/heads/main/agentic-access/eaton-agentic-access.yml
summary_line: 15 operations · 4 acting
tags:
- Power Management
- Electrical
- Smart Breaker
- EV Charging
- Demand Response
- Data Center
- DCIM
- PDU
- UPS
- Utility
- Industrial
- Building
- Mobility
- AI Factory
- Energy
- IoT
- Sustainability
---
