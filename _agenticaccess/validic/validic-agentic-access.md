---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 12
api_specs:
- filename: validic-openapi.yml
  format: yaml
  label: Validic Users API
  slug: validic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Marketplace & Connections API
  slug: validic-marketplace-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Observations & Data API
  slug: validic-observations-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Devices API
  slug: validic-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Streaming API
  slug: validic-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
- filename: validic-openapi.yml
  format: yaml
  label: Validic Push Service API
  slug: validic-push-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Validic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organizations/{org_id}/users
operation_count: 21
overview: 'Validic exposes 21 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Validic
provider_slug: validic
slug: validic-agentic-access
source_filename: validic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/validic-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 12\n    acting: 9\n  by_consequence:\n    read: 12\n    physical: 1\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /organizations/{org_id}/users\n  method: get\n  operationId: getAllUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}/users\n  method: post\n  operationId: provisionUser\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{org_id}/users/{uid}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}/users/{uid}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{org_id}/users/{uid}/cgm\n  method: get\n  operationId: getCgm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /organizations/{org_id}/users/{uid}/intraday\n  method: get\n  operationId: getIntraday\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}/users/{uid}/measurements\n  method: get\n  operationId: getMeasurements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}/users/{uid}/nutrition\n  method: get\n  operationId: getNutrition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}/users/{uid}/sleep\n  method: get\n  operationId: getSleep\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /organizations/{org_id}/users/{uid}/summaries\n  method: get\n  operationId: getSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}/users/{uid}/workouts\n  method: get\n  operationId: getWorkouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}/connection_events\n  method: get\n  operationId: getConnectionEventsByOrgId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{org_id}/users/{uid}/devices/{device_id}/activate\n  method: put\n  operationId: activateCellularDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{org_id}/users/{uid}/devices/{device_id}/suspend\n  method: put\n  operationId: suspendCellularDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams\n  method: post\n  operationId: createStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{id}\n  method: get\n  operationId: getStream\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streams/{id}\n  method: put\n  operationId: updateStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{id}\n  method: delete\n  operationId: deleteStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{id}/connect\n  method: get\n  operationId: connectToStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /streams/{id}/replay\n  method: post\n  operationId: replayStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{org_id}/push\n  method: post\n  operationId: createPushSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/agentic-access/validic-agentic-access.yml
summary_line: 21 operations · 9 acting
tags:
- Health Data
- Digital Health
- Wearables
- Remote Patient Monitoring
- Health IoT
- Interoperability
- HIPAA
---
