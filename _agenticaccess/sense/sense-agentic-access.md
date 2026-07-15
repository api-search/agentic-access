---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 12
api_specs:
- filename: sense-sense-client-api-openapi.yml
  format: yaml
  label: Sense Client API
  slug: sense-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sense/refs/heads/main/openapi/sense-sense-client-api-openapi.yml
consequence_counts:
  read: 12
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sense Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Sense exposes 15 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sense
provider_slug: sense
slug: sense-agentic-access
source_filename: sense-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sense-sense-client-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 3\n    connected: 12\n  by_consequence:\n    write: 3\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /authenticate\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authenticate/mfa\n  method: post\n  operationId: validateMfa\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /renew\n  method: post\n  operationId: renewAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logout\n  method: get\n  operationId: logout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/monitors/{monitor_id}/overview\n  method: get\n  operationId: getMonitorOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /app/monitors/{monitor_id}/status\n  method: get\n  operationId: getMonitorStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/monitors/{monitor_id}/devices\n  method: get\n  operationId: getDiscoveredDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/monitors/{monitor_id}/devices/overview\n  method: get\n  operationId: getDevicesOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/monitors/{monitor_id}/devices/always_on\n  method: get\n  operationId: getAlwaysOnInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/monitors/{monitor_id}/devices/{device_id}\n\
  \  method: get\n  operationId: getDeviceInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{monitor_id}/devices\n  method: get\n  operationId: getRawDeviceData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/monitors/{monitor_id}/history/usage\n  method: get\n  operationId: getUsageHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/monitors/{monitor_id}/history/usage/solar\n  method: get\n  operationId: getSolarHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/{monitor_id}/realtime_update\n  method: get\n  operationId: getRealtimeUpdate\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}/timeline\n  method: get\n  operationId: getUserTimeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sense/refs/heads/main/agentic-access/sense-agentic-access.yml
summary_line: 15 operations · 3 acting
tags:
- Energy
- Home Energy Monitoring
- IoT
- Smart Home
- Electricity
- Solar
- Device Detection
- Real-Time Data
- ClimateTech
---
