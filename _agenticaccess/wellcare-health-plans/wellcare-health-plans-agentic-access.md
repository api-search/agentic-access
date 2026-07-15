---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: wellcare-fhir-patient-access-api-openapi.yml
  format: yaml
  label: WellCare FHIR Patient Access API
  slug: fhir-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-fhir-patient-access-api-openapi.yml
- filename: wellcare-fhir-provider-directory-api-openapi.yml
  format: yaml
  label: WellCare FHIR Provider Directory API
  slug: fhir-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-fhir-provider-directory-api-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wellcare Health Plans Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'wellcare-health-plans exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: wellcare-health-plans
provider_slug: wellcare-health-plans
slug: wellcare-health-plans-agentic-access
source_filename: wellcare-health-plans-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wellcare-fhir-patient-access-api-openapi.yml, openapi/wellcare-fhir-provider-directory-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /fhir/r4/Patient/{id}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/Patient.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Coverage\n  method: get\n  operationId: listCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - patient/Coverage.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/ExplanationOfBenefit\n  method: get\n  operationId: listExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/ExplanationOfBenefit.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Condition\n  method: get\n  operationId: listConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/Condition.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Observation\n  method: get\n  operationId: listObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/Observation.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/MedicationRequest\n  method: get\n  operationId: listMedicationRequests\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/MedicationRequest.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Immunization\n  method: get\n  operationId: listImmunizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/Immunization.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Encounter\n  method: get\n  operationId: listEncounters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/Encounter.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Practitioner\n  method: get\n  operationId: searchPractitioners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Practitioner/{id}\n  method:\
  \ get\n  operationId: getPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Organization\n  method: get\n  operationId: searchOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Organization/{id}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/Location\n  method: get\n  operationId: searchLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/PractitionerRole\n  method: get\n  operationId: searchPractitionerRoles\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/r4/InsurancePlan\n  method: get\n  operationId: searchInsurancePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/agentic-access/wellcare-health-plans-agentic-access.yml
summary_line: 15 operations
tags:
- Fortune 500
---
