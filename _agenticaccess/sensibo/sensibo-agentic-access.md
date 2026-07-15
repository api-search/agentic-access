---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 10
api_specs:
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Users API
  slug: sensibo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Devices API
  slug: sensibo-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo AC States API
  slug: sensibo-ac-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Measurements API
  slug: sensibo-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Historical Data API
  slug: sensibo-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Climate React API
  slug: sensibo-climate-react-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Schedules API
  slug: sensibo-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
- filename: sensibo-openapi.yml
  format: yaml
  label: Sensibo Timers API
  slug: sensibo-timers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/openapi/sensibo-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 2
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Sensibo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /pods/{device_id}/schedules/{schedule_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /pods/{device_id}/smartmode
operation_count: 19
overview: 'Sensibo exposes 19 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 7 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sensibo
provider_slug: sensibo
slug: sensibo-agentic-access
source_filename: sensibo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sensibo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 10\n    acting: 9\n  by_consequence:\n    read: 10\n    write: 7\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /users/me/pods\n  method: get\n  operationId: listPods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}\n  method: get\n  operationId: getPod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}/acStates\n\
  \  method: get\n  operationId: getAcStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}/acStates\n  method: post\n  operationId: setAcState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pods/{device_id}/acStates/{property}\n  method: patch\n  operationId: patchAcStateProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pods/{device_id}/measurements\n  method: get\n  operationId: getMeasurements\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}/historicalMeasurements\n  method: get\n  operationId: getHistoricalMeasurements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}/events\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}/smartmode\n  method: get\n  operationId: getClimateReact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}/smartmode\n  method: put\n  operationId: toggleClimateReact\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pods/{device_id}/smartmode\n  method: post\n  operationId: setClimateReact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pods/{device_id}/schedules\n  method: get\n  operationId: listSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}/schedules\n  method: post\n  operationId: createSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pods/{device_id}/schedules/{schedule_id}\n  method: get\n  operationId: getSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}/schedules/{schedule_id}\n  method: put\n  operationId: toggleSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pods/{device_id}/schedules/{schedule_id}\n  method: delete\n  operationId: deleteSchedule\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pods/{device_id}/timer\n  method: get\n  operationId: getTimer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pods/{device_id}/timer\n  method: put\n  operationId: setTimer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pods/{device_id}/timer\n  method: delete\n  operationId: deleteTimer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensibo/refs/heads/main/agentic-access/sensibo-agentic-access.yml
summary_line: 19 operations · 9 acting · 2 human-in-the-loop
tags:
- Smart Home
- IoT
- Air Conditioning
- HVAC
- Air Quality
- Climate Control
- Connected Devices
---
