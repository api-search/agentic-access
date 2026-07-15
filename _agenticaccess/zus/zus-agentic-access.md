---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: zus-openapi.yml
  format: yaml
  label: Zus Patients (FHIR)
  slug: patients-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
- filename: zus-openapi.yml
  format: yaml
  label: Zus Aggregated Profile
  slug: aggregated-profile
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
- filename: zus-openapi.yml
  format: yaml
  label: Zus FHIR Resources
  slug: fhir-resources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
- filename: zus-openapi.yml
  format: yaml
  label: Zus Document Retrieval
  slug: document-retrieval
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
- filename: zus-openapi.yml
  format: yaml
  label: Zus Subscriptions and Webhooks
  slug: subscriptions-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-openapi.yml
consequence_counts:
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zus Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Zus Health exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zus Health
provider_slug: zus
slug: zus-agentic-access
source_filename: zus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zus-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 7\n    connected: 8\n  by_consequence:\n    write: 7\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/Patient\n  method: get\n  operationId: searchPatients\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Patient\n  method: post\n  operationId: createPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Patient/{id}\n  method: put\n  operationId: updatePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /fhir/{resourceType}\n  method: get\n  operationId: searchResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/{resourceType}\n  method: post\n  operationId: createResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/{resourceType}/{id}\n  method: get\n  operationId: readResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/{resourceType}/{id}\n  method: delete\n  operationId: deleteResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir\n  method: post\n  operationId: submitBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient-history/jobs\n  method: post\n  operationId: createPatientHistoryJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient-history/jobs\n  method: get\n  operationId: listPatientHistoryJobs\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient-history/jobs/{jobId}\n  method: get\n  operationId: getPatientHistoryJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/DocumentReference/{id}\n  method: get\n  operationId: readDocumentReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Binary/{id}\n  method: get\n  operationId: readBinary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/agentic-access/zus-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Health
- FHIR
- Interoperability
- Patient Data
- Healthcare
---
