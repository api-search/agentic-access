---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: aqara-automation-api-openapi.yml
  format: yaml
  label: Aqara Automation API
  slug: aqara-automation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-automation-api-openapi.yml
- filename: aqara-device-api-openapi.yml
  format: yaml
  label: Aqara Device API
  slug: aqara-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-device-api-openapi.yml
- filename: aqara-gateway-api-openapi.yml
  format: yaml
  label: Aqara Gateway API
  slug: aqara-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-gateway-api-openapi.yml
- filename: aqara-space-api-openapi.yml
  format: yaml
  label: Aqara Space API
  slug: aqara-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-space-api-openapi.yml
- filename: aqara-studio-api-openapi.yml
  format: yaml
  label: Aqara Studio API
  slug: aqara-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-studio-api-openapi.yml
consequence_counts:
  read: 5
  safety-critical: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Aqara Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /devices/command/execute
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /devices/trait/execute
operation_count: 9
overview: 'Aqara exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 2 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Aqara
provider_slug: aqara
slug: aqara-agentic-access
source_filename: aqara-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/aiot-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 2\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /spaces\n  method: get\n  operationId: getSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces\n  method: post\n  operationId: createSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/name\n  method: post\n  operationId: updateSpaceName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/types\n  method: get\n  operationId: getDeviceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: get\n  operationId: getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/definitions\n  method: get\n  operationId: getDeviceDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/trait/execute\n  method: post\n  operationId: executeDeviceTrait\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /devices/trait/read\n  method: post\n  operationId: getTraitValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/command/execute\n  method: post\n  operationId: executeDeviceCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/aqara/agentic-access/aqara-agentic-access.yml
summary_line: 9 operations · 4 acting · 2 human-in-the-loop
tags:
- IoT
- Smart Home
- Home Automation
- Consumer Electronics
- Security
---
