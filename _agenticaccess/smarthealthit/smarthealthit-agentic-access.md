---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 14
api_specs:
- filename: smarthealthit-openapi.yml
  format: yaml
  label: SMART Sandbox FHIR R4 API
  slug: smarthealthit-sandbox-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/openapi/smarthealthit-openapi.yml
- filename: smarthealthit-openapi.yml
  format: yaml
  label: SMART App Launch Authorization API
  slug: smarthealthit-smart-app-launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/openapi/smarthealthit-openapi.yml
- filename: smarthealthit-openapi.yml
  format: yaml
  label: SMART Bulk Data Export API
  slug: smarthealthit-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/openapi/smarthealthit-openapi.yml
consequence_counts:
  read: 14
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smarthealthit Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'SMART Health IT exposes 15 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SMART Health IT
provider_slug: smarthealthit
slug: smarthealthit-agentic-access
source_filename: smarthealthit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smarthealthit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 14\n    acting: 1\n  by_consequence:\n    read: 14\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient\n  method: get\n  operationId: searchPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}\n  method: get\n\
  \  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Observation\n  method: get\n  operationId: searchObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Condition\n  method: get\n  operationId: searchConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MedicationRequest\n  method: get\n  operationId: searchMedicationRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Encounter\n  method: get\n  operationId: searchEncounters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /AllergyIntolerance\n  method: get\n  operationId: searchAllergyIntolerances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Immunization\n  method: get\n  operationId: searchImmunizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DocumentReference\n  method: get\n  operationId: searchDocumentReferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/authorize\n  method: get\n  operationId: smartAuthorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/token\n  method: post\n  operationId:\
  \ smartToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /$export\n  method: get\n  operationId: bulkSystemExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/$export\n  method: get\n  operationId: bulkPatientExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Group/{id}/$export\n  method: get\n  operationId: bulkGroupExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/agentic-access/smarthealthit-agentic-access.yml
summary_line: 15 operations · 1 acting
tags:
- SMART on FHIR
- FHIR
- Health IT
- EHR Integration
- Clinical Data
- Clinical Records
- Patient Facing
- Open Standards
- Interoperability
---
