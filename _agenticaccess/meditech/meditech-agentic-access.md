---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: meditech-fhir-openapi.yml
  format: yaml
  label: Meditech Expanse FHIR API
  slug: meditech-expanse-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-fhir-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Meditech Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'meditech exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: meditech
provider_slug: meditech
slug: meditech-agentic-access
source_filename: meditech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/meditech-fhir-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n- path: /Patient\n  method: get\n  operationId: searchPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n- path: /Patient/{id}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n- path: /Patient/{id}/Observation\n  method: get\n  operationId: getPatientObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n- path: /Patient/{id}/Condition\n  method: get\n  operationId: getPatientConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n- path: /Patient/{id}/MedicationRequest\n  method: get\n\
  \  operationId: getPatientMedications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n- path: /Patient/{id}/AllergyIntolerance\n  method: get\n  operationId: getPatientAllergies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n- path: /Patient/{id}/Encounter\n  method: get\n  operationId: getPatientEncounters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n- path: /Patient/{id}/DiagnosticReport\n  method: get\n  operationId: getPatientDiagnosticReports\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n- path: /Patient/{id}/$everything\n  method: get\n  operationId: getPatientEverything\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch\n    - patient/*.read\n    - user/*.read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/agentic-access/meditech-agentic-access.yml
summary_line: 10 operations
tags: []
---
