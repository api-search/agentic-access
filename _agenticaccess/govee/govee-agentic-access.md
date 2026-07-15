---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: govee-openapi.yml
  format: yaml
  label: Govee Devices API
  slug: govee-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Device State API
  slug: govee-device-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Device Control API
  slug: govee-device-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Dynamic Scenes API
  slug: govee-dynamic-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee DIY Scenes API
  slug: govee-diy-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
- filename: govee-openapi.yml
  format: yaml
  label: Govee Segment Color and Brightness API
  slug: govee-segment-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/openapi/govee-openapi.yml
consequence_counts:
  read: 1
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Govee Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /device/control
operation_count: 5
overview: 'Govee exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 3 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Govee
provider_slug: govee
slug: govee-agentic-access
source_filename: govee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/govee-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 1\n    acting: 4\n  by_consequence:\n    read: 1\n    write: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /user/devices\n  method: get\n  operationId: getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/state\n  method: post\n  operationId: getDeviceState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device/control\n  method: post\n  operationId: controlDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /device/scenes\n  method: post\n  operationId: getDeviceScenes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device/diy-scenes\n  method: post\n  operationId: getDeviceDiyScenes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govee/refs/heads/main/agentic-access/govee-agentic-access.yml
summary_line: 5 operations · 4 acting · 1 human-in-the-loop
tags:
- Smart Home
- Smart Lighting
- IoT
- LED
- Home Automation
- Device Control
---
