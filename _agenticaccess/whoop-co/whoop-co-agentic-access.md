---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 14
api_specs:
- filename: openapi.json
  format: json
  label: WHOOP API
  slug: whoop-api
  spec_type: OpenAPI
  url: https://api.prod.whoop.com/developer/doc/openapi.json
- filename: whoop-api-openapi.yml
  format: yaml
  label: WHOOP Trusted Partner API
  slug: whoop-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/openapi/whoop-api-openapi.yml
consequence_counts:
  read: 14
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Whoop Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/user/access
operation_count: 20
overview: 'WHOOP exposes 20 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 5 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WHOOP
provider_slug: whoop-co
slug: whoop-co-agentic-access
source_filename: whoop-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/whoop-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 14\n    acting: 6\n  by_consequence:\n    read: 14\n    write: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/activity-mapping/{activityV1Id}\n  method: get\n  operationId: getActivityMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cycle/{cycleId}\n  method: get\n  operationId: getCycleById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:cycles\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/cycle\n  method: get\n  operationId: getCycleCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:cycles\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cycle/{cycleId}/sleep\n  method: get\n  operationId: getSleepForCycle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partner/development/add-test-data\n  method: post\n  operationId: addTestData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partner/requisition/{id}\n  method: get\n  operationId: getLabRequisitionById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partner/service-request/{id}\n  method: get\n  operationId: getServiceRequestById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partner/token\n  method: post\n  operationId: requestToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partner/requisition/{id}/status\n  method: patch\n  operationId: updateLabRequisitionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partner/service-request/{id}/status\n  method: patch\n  operationId: updateServiceRequestStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partner/service-request/{id}/results\n  method: post\n  operationId: uploadDiagnosticReportResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/recovery\n  method: get\n  operationId: getRecoveryCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - read:recovery\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cycle/{cycleId}/recovery\n  method: get\n  operationId: getRecoveryForCycle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:recovery\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/activity/sleep/{sleepId}\n  method: get\n  operationId: getSleepById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:sleep\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/activity/sleep\n  method: get\n  operationId: getSleepCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:sleep\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/user/measurement/body\n  method: get\n  operationId: getBodyMeasurement\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:body_measurement\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/user/profile/basic\n  method: get\n  operationId: getProfileBasic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/user/access\n  method: delete\n  operationId: revokeUserOAuthAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/activity/workout/{workoutId}\n  method: get\n  operationId: getWorkoutById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n \
  \   - read:workout\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/activity/workout\n  method: get\n  operationId: getWorkoutCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:workout\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whoop-co/refs/heads/main/agentic-access/whoop-co-agentic-access.yml
summary_line: 20 operations · 6 acting · 1 human-in-the-loop
tags:
- Fitness
- Wearables
- Health
- Recovery
- Sleep
- Strain
- Heart Rate
- Workout
- Biometrics
---
