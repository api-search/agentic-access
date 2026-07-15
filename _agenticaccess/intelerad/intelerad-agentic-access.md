---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 1
api_specs:
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Studies API
  slug: intelerad-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Storage API
  slug: intelerad-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Patients API
  slug: intelerad-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Orders and Worklist API
  slug: intelerad-worklist-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Reports API
  slug: intelerad-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare HL7 Integration API
  slug: intelerad-hl7-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Webhooks and Routing API
  slug: intelerad-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Namespaces and Accounts API
  slug: intelerad-namespaces-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
consequence_counts:
  physical: 2
  read: 1
  write: 12
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
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/list
operation_count: 15
overview: 'Intelerad exposes 15 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 12 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Intelerad
provider_slug: intelerad
slug: intelerad-agentic-access
source_filename: intelerad-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/intelerad-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 14\n    connected: 1\n  by_consequence:\n    write: 12\n    read: 1\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /session/login\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session/logout\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/list\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/get\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/share\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/delete\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/study/{namespace}/{studyUid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient/list\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient/get\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/list\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/add\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /report/list\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hl7/transform/list\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/add\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespace/list\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/agentic-access/intelerad-agentic-access.yml
summary_line: 15 operations · 14 acting
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
