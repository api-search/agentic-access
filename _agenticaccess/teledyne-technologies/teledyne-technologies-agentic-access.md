---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: teledyne-flir-camera-rest-openapi.yml
  format: yaml
  label: Teledyne FLIR Camera REST API
  slug: flir-camera-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teledyne-technologies/refs/heads/main/openapi/teledyne-flir-camera-rest-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Teledyne Technologies Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Teledyne Technologies exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Teledyne Technologies
provider_slug: teledyne-technologies
slug: teledyne-technologies-agentic-access
source_filename: teledyne-technologies-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/teledyne-flir-camera-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /image/current\n  method: get\n  operationId: getCurrentImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/{instance}.json\n  method: get\n  operationId: getSpotMeasurement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /box/{instance}.json\n  method: get\n\
  \  operationId: getBoxMeasurement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /line/{instance}.json\n  method: get\n  operationId: getLineMeasurement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alarms\n  method: get\n  operationId: getAllAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alarm/{instance}.json\n  method: get\n  operationId: getAlarm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tempsensor/{instance}.json\n  method: get\n  operationId: getTemperatureSensor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teledyne-technologies/refs/heads/main/agentic-access/teledyne-technologies-agentic-access.yml
summary_line: 7 operations
tags:
- Aerospace
- Defense
- Digital Imaging
- Instrumentation
- Thermal Imaging
- Test and Measurement
- Fortune 500
---
