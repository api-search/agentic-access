---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: roivant-sciences-allergies-api-openapi.yml
  format: yaml
  label: Roivant Sciences Allergies API
  slug: roivant-sciences-allergies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-allergies-api-openapi.yml
- filename: roivant-sciences-appointments-api-openapi.yml
  format: yaml
  label: Roivant Sciences Appointments API
  slug: roivant-sciences-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-appointments-api-openapi.yml
- filename: roivant-sciences-diagnoses-api-openapi.yml
  format: yaml
  label: Roivant Sciences Diagnoses API
  slug: roivant-sciences-diagnoses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-diagnoses-api-openapi.yml
- filename: roivant-sciences-documents-api-openapi.yml
  format: yaml
  label: Roivant Sciences Documents API
  slug: roivant-sciences-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-documents-api-openapi.yml
- filename: roivant-sciences-encounters-api-openapi.yml
  format: yaml
  label: Roivant Sciences Encounters API
  slug: roivant-sciences-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-encounters-api-openapi.yml
- filename: roivant-sciences-immunizations-api-openapi.yml
  format: yaml
  label: Roivant Sciences Immunizations API
  slug: roivant-sciences-immunizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-immunizations-api-openapi.yml
- filename: roivant-sciences-labs-api-openapi.yml
  format: yaml
  label: Roivant Sciences Labs API
  slug: roivant-sciences-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-labs-api-openapi.yml
- filename: roivant-sciences-medications-api-openapi.yml
  format: yaml
  label: Roivant Sciences Medications API
  slug: roivant-sciences-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-medications-api-openapi.yml
- filename: roivant-sciences-patients-api-openapi.yml
  format: yaml
  label: Roivant Sciences Patients API
  slug: roivant-sciences-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-patients-api-openapi.yml
- filename: roivant-sciences-practices-api-openapi.yml
  format: yaml
  label: Roivant Sciences Practices API
  slug: roivant-sciences-practices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-practices-api-openapi.yml
- filename: roivant-sciences-procedures-api-openapi.yml
  format: yaml
  label: Roivant Sciences Procedures API
  slug: roivant-sciences-procedures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-procedures-api-openapi.yml
- filename: roivant-sciences-providers-api-openapi.yml
  format: yaml
  label: Roivant Sciences Providers API
  slug: roivant-sciences-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-providers-api-openapi.yml
- filename: roivant-sciences-vitals-api-openapi.yml
  format: yaml
  label: Roivant Sciences Vitals API
  slug: roivant-sciences-vitals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-vitals-api-openapi.yml
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
- Pharmaceuticals
- Drug Development
- Clinical Trials
- Health Data
- Tokenization
- Electronic Health Records
- Real-World Evidence
- Holding Company
- Healthcare
---
