---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 13
api_specs:
- filename: cloudstudioiot-access-tokens-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Access tokens API
  slug: cloudstudioiot-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-access-tokens-api-openapi.yml
- filename: cloudstudioiot-alarms-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Alarms API
  slug: cloudstudioiot-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-alarms-api-openapi.yml
- filename: cloudstudioiot-alerts-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Alerts API
  slug: cloudstudioiot-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-alerts-api-openapi.yml
- filename: cloudstudioiot-endpoint-data-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Endpoint data API
  slug: cloudstudioiot-endpoint-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-endpoint-data-api-openapi.yml
- filename: cloudstudioiot-geozones-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Geozones API
  slug: cloudstudioiot-geozones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-geozones-api-openapi.yml
- filename: cloudstudioiot-instance-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Instance API
  slug: cloudstudioiot-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-instance-api-openapi.yml
consequence_counts:
  read: 13
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudstudioiot Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Cloud Studio IoT exposes 15 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloud Studio IoT
provider_slug: cloudstudioiot
slug: cloudstudioiot-agentic-access
source_filename: cloudstudioiot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: generated\nsource: openapi/cloudstudioiot-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 2\n    connected: 13\n  by_consequence:\n    write: 2\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /services/gear/AuthorizationService.svc/CreateClientAccessTokenAllIntegrations\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/gear/AuthorizationService.svc/DeleteClientAccessToken\n\
  \  method: post\n  operationId: deleteAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/alerts\n  method: get\n  operationId: listAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/alerts/incremental/{sequenceNumber}\n  method: get\n  operationId: listAlertsIncremental\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/alerts/{alertID}\n  method: get\n  operationId: getAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v2/alarms\n  method: get\n  operationId: listAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/alarms/incremental/{sequenceNumber}\n  method: get\n  operationId: listAlarmsIncremental\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/alarms/{alarmID}\n  method: get\n  operationId: getAlarm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/endpointData\n  method: get\n  operationId: listEndpointData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/endpointData/incremental/{sequenceNumber}\n  method: get\n  operationId:\
  \ listEndpointDataIncremental\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/endpointData/multiple\n  method: get\n  operationId: getLatestEndpointData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/geozones\n  method: get\n  operationId: listGeozones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/geozones/incremental/{sequenceNumber}\n  method: get\n  operationId: listGeozonesIncremental\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/geozones/{geozoneID}\n  method: get\n  operationId: getGeozone\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/instance/mapping/{sequenceNumber}\n  method: get\n  operationId: getInstanceMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/agentic-access/cloudstudioiot-agentic-access.yml
summary_line: 15 operations · 2 acting
tags:
- Company
- IoT
- AI
- Industrial
- Platform
---
