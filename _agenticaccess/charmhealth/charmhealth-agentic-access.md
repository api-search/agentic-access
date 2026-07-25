---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: charmhealth-allergyintolerance-api-openapi.yml
  format: yaml
  label: CharmHealth AllergyIntolerance API
  slug: charmhealth-allergyintolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-allergyintolerance-api-openapi.yml
- filename: charmhealth-appointment-api-openapi.yml
  format: yaml
  label: CharmHealth Appointment API
  slug: charmhealth-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-appointment-api-openapi.yml
- filename: charmhealth-capability-api-openapi.yml
  format: yaml
  label: CharmHealth Capability API
  slug: charmhealth-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-capability-api-openapi.yml
- filename: charmhealth-careplan-api-openapi.yml
  format: yaml
  label: CharmHealth CarePlan API
  slug: charmhealth-careplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-careplan-api-openapi.yml
- filename: charmhealth-careteam-api-openapi.yml
  format: yaml
  label: CharmHealth CareTeam API
  slug: charmhealth-careteam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-careteam-api-openapi.yml
- filename: charmhealth-condition-api-openapi.yml
  format: yaml
  label: CharmHealth Condition API
  slug: charmhealth-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-condition-api-openapi.yml
- filename: charmhealth-documentreference-api-openapi.yml
  format: yaml
  label: CharmHealth DocumentReference API
  slug: charmhealth-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-documentreference-api-openapi.yml
- filename: charmhealth-encounter-api-openapi.yml
  format: yaml
  label: CharmHealth Encounter API
  slug: charmhealth-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-encounter-api-openapi.yml
- filename: charmhealth-immunization-api-openapi.yml
  format: yaml
  label: CharmHealth Immunization API
  slug: charmhealth-immunization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-immunization-api-openapi.yml
- filename: charmhealth-medicationrequest-api-openapi.yml
  format: yaml
  label: CharmHealth MedicationRequest API
  slug: charmhealth-medicationrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-medicationrequest-api-openapi.yml
- filename: charmhealth-observation-api-openapi.yml
  format: yaml
  label: CharmHealth Observation API
  slug: charmhealth-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-observation-api-openapi.yml
- filename: charmhealth-organization-api-openapi.yml
  format: yaml
  label: CharmHealth Organization API
  slug: charmhealth-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-organization-api-openapi.yml
- filename: charmhealth-patient-api-openapi.yml
  format: yaml
  label: CharmHealth Patient API
  slug: charmhealth-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-patient-api-openapi.yml
- filename: charmhealth-practitioner-api-openapi.yml
  format: yaml
  label: CharmHealth Practitioner API
  slug: charmhealth-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-practitioner-api-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Charmhealth Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'CharmHealth exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CharmHealth
provider_slug: charmhealth
slug: charmhealth-agentic-access
source_filename: charmhealth-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/charmhealth-fhir-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient\n  method: get\n  operationId: searchPatient\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AllergyIntolerance\n  method: get\n  operationId: searchAllergyIntolerance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Condition\n  method: get\n  operationId: searchCondition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Encounter\n  method: get\n  operationId: searchEncounter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Observation\n  method: get\n  operationId: searchObservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /MedicationRequest\n  method: get\n  operationId: searchMedicationRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Immunization\n  method: get\n  operationId: searchImmunization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CarePlan\n  method: get\n  operationId: searchCarePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CareTeam\n  method: get\n  operationId: searchCareTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DocumentReference\n  method: get\n  operationId: searchDocumentReference\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner\n  method: get\n  operationId: searchPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization\n  method: get\n  operationId: searchOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Appointment\n  method: get\n  operationId: searchAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/agentic-access/charmhealth-agentic-access.yml
summary_line: 15 operations
tags:
- EHR
- EMR
- FHIR
- Healthcare
- HL7
- Patient Engagement
- Patients
- SMART on FHIR
- US Core
---
