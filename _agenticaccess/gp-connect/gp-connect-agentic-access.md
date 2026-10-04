---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: gp-connect-appointment-api-openapi.yml
  format: yaml
  label: GP Connect Appointment API
  slug: gp-connect-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-appointment-api-openapi.yml
- filename: gp-connect-documents-api-openapi.yml
  format: yaml
  label: GP Connect Documents API
  slug: gp-connect-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-documents-api-openapi.yml
- filename: gp-connect-fhir-api-openapi.yml
  format: yaml
  label: GP Connect FHIR API
  slug: gp-connect-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-fhir-api-openapi.yml
- filename: gp-connect-meta-api-openapi.yml
  format: yaml
  label: GP Connect Meta API
  slug: gp-connect-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-meta-api-openapi.yml
- filename: gp-connect-patient-api-openapi.yml
  format: yaml
  label: GP Connect Patient API
  slug: gp-connect-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-patient-api-openapi.yml
- filename: gp-connect-slot-api-openapi.yml
  format: yaml
  label: GP Connect Slot API
  slug: gp-connect-slot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-slot-api-openapi.yml
- filename: gp-connect-task-api-openapi.yml
  format: yaml
  label: GP Connect Task API
  slug: gp-connect-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/openapi/gp-connect-task-api-openapi.yml
consequence_counts:
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gp Connect Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'GP Connect exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GP Connect
provider_slug: gp-connect
slug: gp-connect-agentic-access
source_filename: gp-connect-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/gp-connect-appointment-api-openapi.yml, openapi/gp-connect-documents-api-openapi.yml,\n  openapi/gp-connect-fhir-api-openapi.yml, openapi/gp-connect-meta-api-openapi.yml, openapi/gp-connect-patient-api-openapi.yml,\n  openapi/gp-connect-slot-api-openapi.yml, openapi/gp-connect-task-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 4\n    connected: 10\n  by_consequence:\n    write: 4\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /Appointment\n  method: post\n  operationId: postAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Appointment/{id}\n  method: get\n  operationId: getAppointmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Appointment/{id}\n  method: put\n  operationId: putAppointmentById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/Patient/{id}\n  method: get\n  operationId: get-document-patient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/Binary/{id}\n  method:\
  \ get\n  operationId: get-document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FHIR/STU3/Bundle\n  method: post\n  operationId: post-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meta\n  method: get\n  operationId: get-capabilitystatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}/Appointment\n  method: get\n  operationId: getPatientByIdAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/$gpc.getstructuredrecord\n\
  \  method: post\n  operationId: get-structured-record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}/DocumentReference\n  method: get\n  operationId: search-document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}/MedicationRequest\n  method: get\n  operationId: get-ordered-medicationrequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Slot\n  method: get\n  operationId: getSlot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Task\n  method: post\n  operationId: post-task\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Task\n  method: get\n  operationId: get-task\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/agentic-access/gp-connect-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- NHS
- FHIR
- Healthcare
- GP Records
- Appointments
- Prescriptions
- Interoperability
- United Kingdom
- Patient Records
- Electronic Health Records
- FHIR STU3
---
