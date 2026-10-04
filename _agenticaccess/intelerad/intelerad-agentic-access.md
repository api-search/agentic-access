---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 5
api_specs:
- filename: intelerad-hl7-api-openapi.yml
  format: yaml
  label: Intelerad HL7 API
  slug: intelerad-hl7-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-hl7-api-openapi.yml
- filename: intelerad-namespace-api-openapi.yml
  format: yaml
  label: Intelerad Namespace API
  slug: intelerad-namespace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-namespace-api-openapi.yml
- filename: intelerad-order-api-openapi.yml
  format: yaml
  label: Intelerad Order API
  slug: intelerad-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-order-api-openapi.yml
- filename: intelerad-patient-api-openapi.yml
  format: yaml
  label: Intelerad Patient API
  slug: intelerad-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-patient-api-openapi.yml
- filename: intelerad-report-api-openapi.yml
  format: yaml
  label: Intelerad Report API
  slug: intelerad-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-report-api-openapi.yml
- filename: intelerad-session-api-openapi.yml
  format: yaml
  label: Intelerad Session API
  slug: intelerad-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-session-api-openapi.yml
- filename: intelerad-storage-api-openapi.yml
  format: yaml
  label: Intelerad Storage API
  slug: intelerad-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-storage-api-openapi.yml
- filename: intelerad-study-api-openapi.yml
  format: yaml
  label: Intelerad Study API
  slug: intelerad-study-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-study-api-openapi.yml
- filename: intelerad-webhook-api-openapi.yml
  format: yaml
  label: Intelerad Webhook API
  slug: intelerad-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-webhook-api-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Intelerad Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/add
operation_count: 15
overview: 'Intelerad exposes 15 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 9 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Intelerad
provider_slug: intelerad
slug: intelerad-agentic-access
source_filename: intelerad-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/intelerad-hl7-api-openapi.yml, openapi/intelerad-namespace-api-openapi.yml,\n  openapi/intelerad-order-api-openapi.yml, openapi/intelerad-patient-api-openapi.yml, openapi/intelerad-report-api-openapi.yml,\n  openapi/intelerad-session-api-openapi.yml, openapi/intelerad-storage-api-openapi.yml, openapi/intelerad-study-api-openapi.yml,\n  openapi/intelerad-webhook-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 10\n    connected: 5\n  by_consequence:\n    write: 9\n    read: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /hl7/transform/list\n  method: post\n  operationId: postHl7TransformList\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/list\n  method: post\n  operationId: postNamespaceList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/list\n  method: post\n  operationId: postOrderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/add\n  method: post\n  operationId: postOrderAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient/list\n  method: post\n  operationId: postPatientList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient/get\n  method: post\n  operationId: postPatientGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /report/list\n  method: post\n  operationId: postReportList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /session/login\n  method: post\n  operationId: postSessionLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session/logout\n  method: post\n  operationId: postSessionLogout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/study/{namespace}/{studyUid}\n  method: get\n  operationId: getStorageStudyByNamespaceByStudyUid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/list\n  method: post\n  operationId:\
  \ postStudyList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/get\n  method: post\n  operationId: postStudyGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/share\n  method: post\n  operationId: postStudyShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/delete\n  method: post\n  operationId: postStudyDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/add\n  method: post\n  operationId: postWebhookAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/agentic-access/intelerad-agentic-access.yml
summary_line: 15 operations · 10 acting
tags:
- Medical Imaging
- PACS
- Enterprise Imaging
- Radiology
- DICOM
- DICOMweb
- HL7
- FHIR
- Healthcare
- Interoperability
- Image Exchange
---
