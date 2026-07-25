---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: tesla-energy-backup-api-openapi.yml
  format: yaml
  label: Tesla Energy Backup API
  slug: tesla-energy-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-backup-api-openapi.yml
- filename: tesla-energy-history-api-openapi.yml
  format: yaml
  label: Tesla Energy History API
  slug: tesla-energy-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-history-api-openapi.yml
- filename: tesla-energy-live-status-api-openapi.yml
  format: yaml
  label: Tesla Energy Live Status API
  slug: tesla-energy-live-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-live-status-api-openapi.yml
- filename: tesla-energy-off-grid-charging-api-openapi.yml
  format: yaml
  label: Tesla Energy Off Grid Charging API
  slug: tesla-energy-off-grid-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-off-grid-charging-api-openapi.yml
- filename: tesla-energy-operation-api-openapi.yml
  format: yaml
  label: Tesla Energy Operation API
  slug: tesla-energy-operation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-operation-api-openapi.yml
- filename: tesla-energy-products-api-openapi.yml
  format: yaml
  label: Tesla Energy Products API
  slug: tesla-energy-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-products-api-openapi.yml
- filename: tesla-energy-programs-api-openapi.yml
  format: yaml
  label: Tesla Energy Programs API
  slug: tesla-energy-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-programs-api-openapi.yml
- filename: tesla-energy-site-info-api-openapi.yml
  format: yaml
  label: Tesla Energy Site Info API
  slug: tesla-energy-site-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-site-info-api-openapi.yml
- filename: tesla-energy-storm-mode-api-openapi.yml
  format: yaml
  label: Tesla Energy Storm Mode API
  slug: tesla-energy-storm-mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-storm-mode-api-openapi.yml
- filename: tesla-energy-time-of-use-api-openapi.yml
  format: yaml
  label: Tesla Energy Time Of Use API
  slug: tesla-energy-time-of-use-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-time-of-use-api-openapi.yml
consequence_counts:
  read: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tesla Energy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Tesla Energy exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tesla Energy
provider_slug: tesla-energy
slug: tesla-energy-agentic-access
source_filename: tesla-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tesla-energy-fleet-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 5\n    acting: 5\n  by_consequence:\n    read: 5\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - energy_cmds\n    - energy_device_data\n- path: /energy_sites/{site_id}/site_info\n  method: get\n  operationId: getEnergySiteInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - energy_cmds\n    - energy_device_data\n- path: /energy_sites/{site_id}/live_status\n  method: get\n  operationId: getEnergySiteLiveStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - energy_cmds\n    - energy_device_data\n- path: /energy_sites/{site_id}/calendar_history\n  method: get\n  operationId: getEnergySiteCalendarHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - energy_cmds\n    - energy_device_data\n- path: /energy_sites/{site_id}/backup\n  method: post\n  operationId: setBackupReservePercent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - energy_cmds\n    - energy_device_data\n- path: /energy_sites/{site_id}/operation\n  method: post\n  operationId: setSiteOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - energy_cmds\n    - energy_device_data\n- path: /energy_sites/{site_id}/storm_mode\n  method: post\n  operationId: setStormMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - energy_cmds\n    - energy_device_data\n- path: /energy_sites/{site_id}/time_of_use_settings\n\
  \  method: post\n  operationId: setTimeOfUseSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - energy_cmds\n    - energy_device_data\n- path: /energy_sites/{site_id}/off_grid_vehicle_charging_reserve\n  method: post\n  operationId: setOffGridVehicleChargingReserve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - energy_cmds\n    - energy_device_data\n- path: /energy_sites/{site_id}/programs\n  method: get\n  operationId: getEnergySitePrograms\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - energy_cmds\n    - energy_device_data\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/agentic-access/tesla-energy-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- Energy
- Clean Energy
- Solar
- Battery Storage
- Powerwall
- Megapack
- Solar Roof
- Virtual Power Plant
- IoT
- Grid Services
- Home Energy
- Utility Scale
---
