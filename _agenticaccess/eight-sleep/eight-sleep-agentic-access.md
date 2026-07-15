---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 8
api_specs:
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Authentication API
  slug: eight-sleep-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep User API
  slug: eight-sleep-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Device API
  slug: eight-sleep-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Temperature API
  slug: eight-sleep-temperature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Trends API
  slug: eight-sleep-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Base API
  slug: eight-sleep-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
- filename: eight-sleep-openapi.yml
  format: yaml
  label: Eight Sleep Alarms API
  slug: eight-sleep-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/openapi/eight-sleep-openapi.yml
consequence_counts:
  read: 8
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Eight Sleep Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/users/{userId}/base/angle
operation_count: 13
overview: 'Eight Sleep exposes 13 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Eight Sleep
provider_slug: eight-sleep
slug: eight-sleep-agentic-access
source_filename: eight-sleep-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/eight-sleep-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 5\n    connected: 8\n  by_consequence:\n    write: 4\n    read: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/tokens\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{deviceId}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/temperature\n  method: get\n  operationId: getTemperature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/temperature\n  method: put\n  operationId: setTemperature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/away-mode\n  method: put\n  operationId: setAwayMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/trends\n  method: get\n  operationId: getTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/base\n  method: get\n  operationId: getBase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/base/angle\n  method: post\n  operationId:\
  \ setBaseAngle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/users/{userId}/alarms\n  method: get\n  operationId: getAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/alarms/{alarmId}\n  method: put\n  operationId: updateAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/routines\n  method: get\n  operationId: getRoutines\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/agentic-access/eight-sleep-agentic-access.yml
summary_line: 13 operations · 5 acting · 1 human-in-the-loop
tags:
- Sleep
- IoT
- Smart Home
- Wearables
- Health
- Unofficial
---
