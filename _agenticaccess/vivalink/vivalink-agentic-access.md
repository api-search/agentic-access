---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Subjects API
  slug: vivalink-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Devices API
  slug: vivalink-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Vital Signs Data API
  slug: vivalink-vital-signs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Webhooks API
  slug: vivalink-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK FHIR API
  slug: vivalink-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
consequence_counts:
  read: 8
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vivalink Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'VivaLNK exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VivaLNK
provider_slug: vivalink
slug: vivalink-agentic-access
source_filename: vivalink-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vivalink-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 8\n    acting: 8\n  by_consequence:\n    read: 8\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/subjects\n  method: get\n  operationId: listSubjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subjects\n  method: post\n  operationId: createSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subjects/{subjectId}\n  method: get\n  operationId: getSubject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subjects/{subjectId}\n  method: patch\n  operationId: updateSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subjects/{subjectId}\n  method: delete\n  operationId: deactivateSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{deviceId}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devices/{deviceId}/assignment\n  method: put\n  operationId: assignDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devices/{deviceId}/assignment\n  method: delete\n  operationId: unassignDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subjects/{subjectId}/measurements\n  method: get\n  operationId: listMeasurements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subjects/{subjectId}/exports\n  method: post\n  operationId: createExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhookId}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/Observation\n  method: get\n  operationId: searchFhirObservations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/agentic-access/vivalink-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Connected Health
- Remote Patient Monitoring
- RPM
- Wearables
- Biosensors
- Biometrics
- ECG
- Vital Signs
- Digital Health
- IoT
- Clinical Trials
---
