---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 15
api_specs:
- filename: span-rest-api-openapi.json
  format: json
  label: SPAN REST API
  slug: span-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/openapi/span-rest-api-openapi.json
- filename: span-ebus-asyncapi.yml
  format: yaml
  label: SPAN eBus MQTT API
  slug: span-ebus-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/asyncapi/span-ebus-asyncapi.yml
consequence_counts:
  read: 15
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Span Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/panel/emergency-reconnect
operation_count: 24
overview: 'SPAN exposes 24 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 8 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SPAN
provider_slug: span-io
slug: span-io-agentic-access
source_filename: span-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/span-rest-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 9\n    connected: 15\n  by_consequence:\n    write: 8\n    read: 15\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/auth/register\n  method: post\n  operationId: generate_jwt_api_v1_auth_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/auth/clients\n  method: get\n  operationId: get_all_clients_api_v1_auth_clients_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/clients/{name}\n  method: get\n  operationId: get_client_api_v1_auth_clients__name__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/clients/{name}\n  method: delete\n  operationId: delete_client_api_v1_auth_clients__name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/status\n  method: get\n  operationId: system_status_api_v1_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v1/wifi/scan\n  method: get\n  operationId: get_wifi_scan_api_v1_wifi_scan_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/wifi/connect\n  method: post\n  operationId: run_wifi_connect_api_v1_wifi_connect_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/panel\n  method: get\n  operationId: get_panel_state_api_v1_panel_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/islanding-state\n  method: get\n  operationId: get_islanding_state_api_v1_islanding_state_get\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/panel/grid\n  method: get\n  operationId: get_main_relay_state_api_v1_panel_grid_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/panel/grid\n  method: post\n  operationId: set_main_relay_state_api_v1_panel_grid_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/panel/power\n  method: get\n  operationId: get_panel_power_api_v1_panel_power_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/panel/meter\n  method: get\n  operationId: get_panel_meter_api_v1_panel_meter_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/circuits\n  method: get\n  operationId: get_circuits_api_v1_circuits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/circuits/{circuitId}\n  method: get\n  operationId: get_circuit_state_api_v1_circuits__circuitId__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/circuits/{circuitId}\n  method: post\n  operationId: set_circuit_state_api_v1_circuits__circuitId__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/spaces/{spaces_id}\n  method: get\n  operationId: deprecated_spaces_endpoint_stub_api_v1_spaces__spaces_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spaces/{spaces_id}\n  method: post\n  operationId: deprecated_spaces_endpoint_stub_api_v1_spaces__spaces_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/spaces\n  method: get\n  operationId: deprecated_spaces_endpoint_stub_api_v1_spaces_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/panel/emergency-reconnect\n  method: post\n  operationId: run_panel_emergency_reconnect_api_v1_panel_emergency_reconnect_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/storage/soe\n  method: get\n  operationId: get_storage_soe_api_v1_storage_soe_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/storage/soe\n  method: post\n  operationId: set_storage_soe_api_v1_storage_soe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/storage/nice-to-have-thresh\n  method: get\n  operationId: get_storage_nice_to_have_threshold_api_v1_storage_nice_to_have_thresh_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/storage/nice-to-have-thresh\n  method: post\n  operationId: set_storage_nice_to_have_threshold_api_v1_storage_nice_to_have_thresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/span-io/refs/heads/main/agentic-access/span-io-agentic-access.yml
summary_line: 24 operations · 9 acting · 1 human-in-the-loop
tags:
- Energy
- Home Energy
- Electrification
- Smart Panel
- Electrical Panel
- Home Automation
- Solar
- Energy Storage
- EV Charging
- Grid
- Islanding
- Backup Power
- Demand Response
- IoT
- MQTT
- Homie
- Electrification Bus
- On-Premise
---
