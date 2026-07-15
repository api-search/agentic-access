---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Observations (Data Values) API
  slug: bodytrace-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Data Messages API
  slug: bodytrace-datamessages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Devices API
  slug: bodytrace-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Alerts API
  slug: bodytrace-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Provisioning API
  slug: bodytrace-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Measurement Webhook (Push) API
  slug: bodytrace-measurement-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
consequence_counts:
  physical: 1
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bodytrace Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /device/{imei}/provision
operation_count: 6
overview: 'BodyTrace exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BodyTrace
provider_slug: bodytrace
slug: bodytrace-agentic-access
source_filename: bodytrace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bodytrace-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /device/{imei}/datavalues\n  method: get\n  operationId: getDeviceDataValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/{imei}/datamessages\n  method: get\n  operationId: getDeviceDataMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/{imei}/status\n  method: get\n  operationId: getDeviceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/{imei}/alerts\n  method: get\n  operationId: listDeviceAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/{imei}/provision\n  method: post\n  operationId: provisionDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/agentic-access/bodytrace-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Remote Patient Monitoring
- RPM
- Cellular
- Medical Devices
- Digital Health
- Blood Pressure
- Connected Devices
- IoT
---
