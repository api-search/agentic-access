---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: datavant-healthjump-ehr-openapi.yml
  format: yaml
  label: Datavant Healthjump EHR Integration API
  slug: datavant-healthjump-ehr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/datavant-healthjump-ehr-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Roivant Sciences Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Roivant Sciences exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Roivant Sciences
provider_slug: roivant-sciences
slug: roivant-sciences-agentic-access
source_filename: roivant-sciences-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/datavant-healthjump-ehr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /patients\n  method: get\n  operationId: listPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /patients/{patient_id}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n \
  \   scope:\n    - read:clinical\n    - read:patients\n- path: /encounters\n  method: get\n  operationId: listEncounters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /encounters/{encounter_id}\n  method: get\n  operationId: getEncounter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /vitals\n  method: get\n  operationId: listVitals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /allergies\n  method: get\n  operationId: listAllergies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /immunizations\n  method: get\n  operationId: listImmunizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /medications\n  method: get\n  operationId: listMedications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /diagnoses\n  method: get\n  operationId: listDiagnoses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /procedures\n  method: get\n  operationId: listProcedures\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /labs\n  method: get\n  operationId: listLabs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /appointments\n  method: get\n  operationId: listAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path:\
  \ /providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n- path: /practices\n  method: get\n  operationId: listPractices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read:clinical\n    - read:patients\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/agentic-access/roivant-sciences-agentic-access.yml
summary_line: 15 operations
tags:
- Biotech
- Pharmaceutical
- Drug Development
- Clinical Trials
- Health Data
- Tokenization
- Electronic Health Records
- Real World Evidence
- Holding Company
- Healthcare
---
