---
acting_count: 23
action_class_counts:
  acting: 23
api_specs:
- filename: bear-robotics-carti-api-openapi.yml
  format: yaml
  label: Bear Robotics Carti API
  slug: bear-robotics-carti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-carti-api-openapi.yml
- filename: bear-robotics-fleet-management-api-openapi.yml
  format: yaml
  label: Bear Robotics Fleet Management API
  slug: bear-robotics-fleet-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-fleet-management-api-openapi.yml
- filename: bear-robotics-localization-navigation-api-openapi.yml
  format: yaml
  label: Bear Robotics Localization & Navigation API
  slug: bear-robotics-localization-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-localization-navigation-api-openapi.yml
- filename: bear-robotics-locations-maps-api-openapi.yml
  format: yaml
  label: Bear Robotics Locations & Maps API
  slug: bear-robotics-locations-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-locations-maps-api-openapi.yml
- filename: bear-robotics-mission-api-openapi.yml
  format: yaml
  label: Bear Robotics Mission API
  slug: bear-robotics-mission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-mission-api-openapi.yml
- filename: bear-robotics-robot-status-api-openapi.yml
  format: yaml
  label: Bear Robotics Robot Status API
  slug: bear-robotics-robot-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-robot-status-api-openapi.yml
- filename: bear-robotics-robot-system-api-openapi.yml
  format: yaml
  label: Bear Robotics Robot System API
  slug: bear-robotics-robot-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-robot-system-api-openapi.yml
- filename: bear-robotics-servi-api-openapi.yml
  format: yaml
  label: Bear Robotics Servi API
  slug: bear-robotics-servi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/openapi/bear-robotics-servi-api-openapi.yml
consequence_counts:
  physical: 1
  safety-critical: 1
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Bear Robotics Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/conveyor/control
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/robot/charge
operation_count: 23
overview: 'Bear Robotics exposes 23 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bear Robotics
provider_slug: bear-robotics
slug: bear-robotics-agentic-access
source_filename: bear-robotics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/bear-robotics-cloud-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 23\n  by_consequence:\n    write: 21\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v0/robot-system-info/get\n  method: post\n  operationId: APIService_GetRobotSystemInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/available-locations/get\n  method: post\n  operationId:\
  \ APIService_GetAvailableLocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conveyor-index/get\n  method: post\n  operationId: APIService_GetConveyorIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conveyor/control\n  method: post\n  operationId: APIService_ControlConveyor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/current-map/get\n  method: post\n  operationId: APIService_GetCurrentMap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/location-info/get\n  method: post\n  operationId: APIService_GetLocationInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/map/get\n  method: post\n  operationId: APIService_GetMap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/map/switch\n  method: post\n  operationId: APIService_SwitchMap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mission/append\n  method: post\n  operationId: APIService_AppendMission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mission/append-batch\n  method: post\n  operationId: APIService_AppendMissionBatch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mission/create\n  method: post\n  operationId: APIService_CreateMission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mission/create-batch\n  method: post\n  operationId: APIService_CreateMissionBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mission/update\n\
  \  method: post\n  operationId: APIService_UpdateMission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mission-workflow/create\n  method: post\n  operationId: APIService_CreateMissionWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/goal/skip\n  method: post\n  operationId: APIService_SkipGoal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mission-status/clear\n  method: post\n  operationId: APIService_ClearMissionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pose/set\n  method: post\n  operationId: APIService_SetPose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/robot-ids/list\n  method: post\n  operationId: APIService_ListRobotIDs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/robot-state/get\n  method: post\n  operationId: APIService_GetRobotStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/robot/charge\n  method: post\n  operationId: APIService_ChargeRobot\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/robot/localize\n  method: post\n  operationId: APIService_LocalizeRobot\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/system-command/run\n  method: post\n  operationId: APIService_RunSystemCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trays/calibrate\n  method: post\n  operationId: APIService_CalibrateTrays\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bear-robotics/refs/heads/main/agentic-access/bear-robotics-agentic-access.yml
summary_line: 23 operations · 23 acting · 1 human-in-the-loop
tags:
- Robotics
- Autonomous Mobile Robots
- Fleet Management
- Hospitality
- Food Service
- Logistics
- gRPC
- Protobuf
- Webhooks
- Internet of Things
- Company
---
