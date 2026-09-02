---
acting_count: 12
action_class_counts:
  acting: 12
api_specs:
- filename: beehero-audio-api-openapi.yml
  format: yaml
  label: BeeHero Audio API
  slug: beehero-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-audio-api-openapi.yml
- filename: beehero-auth-api-openapi.yml
  format: yaml
  label: BeeHero Auth API
  slug: beehero-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-auth-api-openapi.yml
- filename: beehero-gateways-api-openapi.yml
  format: yaml
  label: BeeHero Gateways API
  slug: beehero-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-gateways-api-openapi.yml
- filename: beehero-sensors-api-openapi.yml
  format: yaml
  label: BeeHero Sensors API
  slug: beehero-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/openapi/beehero-sensors-api-openapi.yml
consequence_counts:
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Beehero Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'BeeHero exposes 12 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BeeHero
provider_slug: beehero
slug: beehero-agentic-access
source_filename: beehero-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/beehero-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 12\n  by_consequence:\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_audio_samples\n  method: post\n  operationId: get_audio_sample_by_mac_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sensors/samples\n  method: post\n  operationId: get_sensors_sample_by_mac_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sensors/samples_connected\n  method: post\n  operationId: get_sensors_connected_by_gateway_mac\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sensors/update_sensor_name\n  method:\
  \ put\n  operationId: update_sensor_name\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateways/samples\n  method: post\n  operationId: get_gateways_sample_by_mac_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateways/samples/get_mac_address\n  method: post\n  operationId: get_gateway_mac_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /gateways/add_skip_remote\n  method: put\n  operationId: add_skip_remote_to_gateway_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateways/remove_skip_remote\n  method: put\n  operationId: remove_skip_remote_from_gateway_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateways/gateway_config_status\n  method: post\n  operationId: get_gateway_config_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateways/movement_interrupt\n  method: put\n  operationId: movement_interrupt_gateway_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateways/rssi_configuration\n  method: put\n  operationId: rssi_configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beehero/refs/heads/main/agentic-access/beehero-agentic-access.yml
summary_line: 12 operations · 12 acting
tags:
- Company
- Agriculture
- AgTech
- Pollination
- beekeeping
- Precision Agriculture
- IoT
- Sensors
- Environmental Data
- MCP
- agent-native
---
