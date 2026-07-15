---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 9
api_specs:
- filename: gp-connect-access-record-structured-fhir.yaml
  format: yaml
  label: GP Connect Access Record - Structured FHIR API
  slug: access-record-structured-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-access-record-structured-fhir/master/specification/gp-connect-access-record-structured-fhir.yaml
- filename: gp-connect-appointments-management-fhir.yaml
  format: yaml
  label: GP Connect Appointment Management FHIR API
  slug: appointment-management-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-appointments-management-fhir/master/specification/gp-connect-appointments-management-fhir.yaml
- filename: gp-connect-update-record-fhir.yaml
  format: yaml
  label: GP Connect Update Record FHIR API
  slug: update-record-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-update-record-fhir/master/specification/gp-connect-update-record-fhir.yaml
- filename: gp-connect-access-record-fhir.yaml
  format: yaml
  label: GP Connect Patient Facing Access Record FHIR API
  slug: patient-facing-access-record-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-access-record-fhir/master/specification/gp-connect-access-record-fhir.yaml
- filename: gp-connect-appointments-management-fhir.yaml
  format: yaml
  label: GP Connect Patient Facing Appointment Management FHIR API
  slug: patient-facing-appointments-management-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-appointments-management-fhir/master/specification/gp-connect-appointments-management-fhir.yaml
- filename: gp-connect-prescriptions-management-fhir.yaml
  format: yaml
  label: GP Connect Patient Facing Prescriptions Management FHIR API
  slug: patient-facing-prescriptions-management-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/NHSDigital/gp-connect-prescriptions-management-fhir/master/specification/gp-connect-prescriptions-management-fhir.yaml
consequence_counts:
  read: 9
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gp Connect Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'GP Connect exposes 14 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GP Connect
provider_slug: gp-connect
slug: gp-connect-agentic-access
source_filename: gp-connect-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gp-connect-appointments-management-fhir.yaml, openapi/gp-connect-patient-facing-access-record-fhir.yaml,\n  openapi/gp-connect-patient-facing-prescriptions-management-fhir.yaml, openapi/gp-connect-update-record-fhir.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 9\n    acting: 5\n  by_consequence:\n    read: 9\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /Slot\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Appointment\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Patient/{id}/Appointment\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Appointment/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Appointment/{id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Patient/$gpc.getstructuredrecord\n  method: post\n  operationId: get-structured-record\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/Patient/{id}\n  method: get\n  operationId: get-document-patient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/Binary/{id}\n  method: get\n  operationId: get-document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}/DocumentReference\n  method: get\n  operationId: search-document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}/MedicationRequest\n\
  \  method: get\n  operationId: get-ordered-medicationrequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Task\n  method: post\n  operationId: post-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Task\n  method: get\n  operationId: get-task\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FHIR/STU3/Bundle\n  method: post\n  operationId: post-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meta\n  method: get\n  operationId: get-capabilitystatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gp-connect/refs/heads/main/agentic-access/gp-connect-agentic-access.yml
summary_line: 14 operations · 5 acting
tags:
- NHS
- FHIR
- Healthcare
- GP Records
- Appointments
- Prescriptions
- Interoperability
- UK
- Patient Records
- Electronic Health Records
- FHIR STU3
- FHIR R4
---
