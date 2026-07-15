---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 12
api_specs:
- filename: wahoo-cloud-api-openapi.yml
  format: yaml
  label: Wahoo Cloud API
  slug: wahoo-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/openapi/wahoo-cloud-api-openapi.yml
consequence_counts:
  read: 12
  safety-critical: 1
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Wahoo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/permissions
operation_count: 28
overview: 'Wahoo Fitness exposes 28 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 15 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wahoo Fitness
provider_slug: wahoo
slug: wahoo-agentic-access
source_filename: wahoo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wahoo-cloud-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 12\n    acting: 16\n  by_consequence:\n    read: 12\n    write: 15\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user_write\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workouts\n  method: get\n  operationId: listWorkouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workouts_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workouts\n  method: post\n  operationId: createWorkout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workouts_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workouts/{id}\n  method: get\n  operationId: getWorkout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workouts_read\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /v1/workouts/{id}\n  method: put\n  operationId: updateWorkout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workouts_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workouts/{id}\n  method: delete\n  operationId: deleteWorkout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workouts_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workouts/{id}/workout_summary\n  method: get\n  operationId: getWorkoutSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - workouts_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workouts/{id}/workout_summary\n  method: post\n  operationId: createWorkoutSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workouts_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workout_file_uploads\n  method: post\n  operationId: createWorkoutFileUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workouts_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workout_file_uploads/{token}\n  method: get\n  operationId: getWorkoutFileUpload\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - workouts_write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - plans_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - plans_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/plans/{id}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - plans_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans/{id}\n\
  \  method: put\n  operationId: updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - plans_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/plans/{id}\n  method: delete\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - plans_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workouts/{workout_id}/plans\n  method: get\n  operationId: listPlansForWorkout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - plans_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/routes\n  method: get\n  operationId: listRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - routes_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/routes\n  method: post\n  operationId: createRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - routes_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/routes/{id}\n  method: get\n  operationId: getRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - routes_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/routes/{id}\n  method: put\n  operationId: updateRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - routes_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/routes/{id}\n  method: delete\n  operationId: deleteRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - routes_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/power_zones\n  method: get\n  operationId: listPowerZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - power_zones_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/power_zones\n  method: post\n  operationId: createPowerZones\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - power_zones_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/power_zones/{id}\n  method: get\n  operationId: getPowerZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - power_zones_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/power_zones/{id}\n  method: put\n  operationId: updatePowerZones\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - power_zones_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/power_zones/{id}\n  method: delete\n  operationId: deletePowerZones\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - power_zones_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/permissions\n  method: delete\n  operationId: revokeAppAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/agentic-access/wahoo-agentic-access.yml
summary_line: 28 operations · 16 acting · 1 human-in-the-loop
tags:
- Fitness
- Cycling
- Endurance Training
- Bike Computers
- Smart Trainers
- Indoor Cycling
- Heart Rate
- Power Meters
- GPS
- Wearables
- Hardware
- FIT Files
- Webhooks
- OAuth
---
