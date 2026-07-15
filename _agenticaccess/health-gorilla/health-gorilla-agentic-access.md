---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 18
api_specs:
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Patients (FHIR)
  slug: patients-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Record Query/Retrieval
  slug: record-query
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Lab Ordering
  slug: lab-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Diagnostic Reports
  slug: diagnostic-reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Documents
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
- filename: health-gorilla-openapi.yml
  format: yaml
  label: Eligibility
  slug: eligibility
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-openapi.yml
consequence_counts:
  physical: 1
  read: 18
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Health Gorilla Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /RequestGroup
operation_count: 22
overview: 'Health Gorilla exposes 22 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Health Gorilla
provider_slug: health-gorilla
slug: health-gorilla-agentic-access
source_filename: health-gorilla-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/health-gorilla-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 18\n    acting: 4\n  by_consequence:\n    read: 18\n    write: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient\n  method: get\n  operationId: searchPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient\n\
  \  method: post\n  operationId: createPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}\n  method: put\n  operationId: updatePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Patient/{id}/$everything\n  method: get\n  operationId: patientEverything\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /RequestGroup\n  method: post\n  operationId: createRequestGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /RequestGroup\n  method: get\n  operationId: searchRequestGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /RequestGroup/{id}\n  method: get\n  operationId: readRequestGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ServiceRequest\n  method: get\n  operationId:\
  \ searchServiceRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ServiceRequest\n  method: post\n  operationId: createServiceRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ServiceRequest/{id}\n  method: get\n  operationId: readServiceRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DiagnosticReport\n  method: get\n  operationId: searchDiagnosticReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DiagnosticReport/{id}\n\
  \  method: get\n  operationId: readDiagnosticReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Observation\n  method: get\n  operationId: searchObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DocumentReference\n  method: get\n  operationId: searchDocumentReferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DocumentReference/{id}\n  method: get\n  operationId: readDocumentReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Binary/{id}\n  method: get\n  operationId: readBinary\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Coverage\n  method: get\n  operationId: searchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Coverage/{id}\n  method: get\n  operationId: readCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner\n  method: get\n  operationId: searchPractitioners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner/{id}\n  method: get\n  operationId: readPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/agentic-access/health-gorilla-agentic-access.yml
summary_line: 22 operations · 4 acting
tags:
- Health
- Interoperability
- FHIR
- Clinical Data
- Lab Ordering
---
