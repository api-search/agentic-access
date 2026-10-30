---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 31
api_specs:
- filename: airthings-accounts-api-openapi.yml
  format: yaml
  label: Airthings Accounts API
  slug: airthings-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-accounts-api-openapi.yml
- filename: airthings-device-api-openapi.yml
  format: yaml
  label: Airthings Device API
  slug: airthings-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-device-api-openapi.yml
- filename: airthings-devices-api-openapi.yml
  format: yaml
  label: Airthings Devices API
  slug: airthings-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-devices-api-openapi.yml
- filename: airthings-health-api-openapi.yml
  format: yaml
  label: Airthings Health API
  slug: airthings-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-health-api-openapi.yml
- filename: airthings-locations-api-openapi.yml
  format: yaml
  label: Airthings Locations API
  slug: airthings-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-locations-api-openapi.yml
- filename: airthings-organizations-api-openapi.yml
  format: yaml
  label: Airthings Organizations API
  slug: airthings-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-organizations-api-openapi.yml
- filename: airthings-segments-api-openapi.yml
  format: yaml
  label: Airthings Segments API
  slug: airthings-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-segments-api-openapi.yml
- filename: airthings-sensor-api-openapi.yml
  format: yaml
  label: Airthings Sensor API
  slug: airthings-sensor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-sensor-api-openapi.yml
- filename: airthings-spaces-api-openapi.yml
  format: yaml
  label: Airthings Spaces API
  slug: airthings-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-spaces-api-openapi.yml
- filename: airthings-thresholds-api-openapi.yml
  format: yaml
  label: Airthings Thresholds API
  slug: airthings-thresholds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-thresholds-api-openapi.yml
- filename: airthings-webhooks-api-openapi.yml
  format: yaml
  label: Airthings Webhooks API
  slug: airthings-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airthings/openapi/airthings-webhooks-api-openapi.yml
consequence_counts:
  read: 31
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Airthings Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 39
overview: 'Airthings exposes 39 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Airthings
provider_slug: airthings
slug: airthings-agentic-access
source_filename: airthings-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/airthings-api-openapi.yml, openapi/airthings-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 31\n    acting: 8\n  by_consequence:\n    read: 31\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: //v1/thresholds\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - write:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:device\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devices/labels\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:device\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devices/{serialNumber}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/battery\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/hourly-radon-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/latest-battery\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/latest-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/mold-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/occupancy-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/threshold-breaches\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/ventilation-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{serialNumber}/virus-risk-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    - write:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:device\n    - write:device\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/locations/{locationId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations/{locationId}/devices\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:device\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/locations/{locationId}/latest-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments/{segmentId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments/{segmentId}/hourly-radon-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments/{segmentId}/mold-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments/{segmentId}/occupancy-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments/{segmentId}/samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments/{segmentId}/ventilation-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments/{segmentId}/virus-risk-samples\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - read:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/spaces\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:device\n    - write:device\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:device\n    - write:device\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:device\n    - write:device\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/webhooks/{hookId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:device\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{hookId}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:device\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{accountId}/sensors\n  method: get\n  operationId: getMultipleSensors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/accounts/{accountId}/devices\n  method: get\n  operationId: getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts\n  method: get\n  operationId: getAccountsIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/airthings/agentic-access/airthings-agentic-access.yml
summary_line: 39 operations · 8 acting
tags:
- Company
- AirQuality
- Radon
- Sensors
- IoT
---
