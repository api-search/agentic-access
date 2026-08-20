---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: temple-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Temple Health Allergy Intolerance API
  slug: temple-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-allergy-intolerance-api-openapi.yml
- filename: temple-health-bulk-data-api-openapi.yml
  format: yaml
  label: Temple Health Bulk Data API
  slug: temple-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-bulk-data-api-openapi.yml
- filename: temple-health-condition-api-openapi.yml
  format: yaml
  label: Temple Health Condition API
  slug: temple-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-condition-api-openapi.yml
- filename: temple-health-document-reference-api-openapi.yml
  format: yaml
  label: Temple Health Document Reference API
  slug: temple-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-document-reference-api-openapi.yml
- filename: temple-health-encounter-api-openapi.yml
  format: yaml
  label: Temple Health Encounter API
  slug: temple-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-encounter-api-openapi.yml
- filename: temple-health-medication-request-api-openapi.yml
  format: yaml
  label: Temple Health Medication Request API
  slug: temple-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-medication-request-api-openapi.yml
- filename: temple-health-metadata-api-openapi.yml
  format: yaml
  label: Temple Health Metadata API
  slug: temple-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-metadata-api-openapi.yml
- filename: temple-health-observation-api-openapi.yml
  format: yaml
  label: Temple Health Observation API
  slug: temple-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-observation-api-openapi.yml
- filename: temple-health-patient-api-openapi.yml
  format: yaml
  label: Temple Health Patient API
  slug: temple-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-patient-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Temple Health Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Temple Health exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Temple Health
provider_slug: temple-health
slug: temple-health-agentic-access
source_filename: temple-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/temple-health-temple-health-fhir-r4-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n\
  \    - patient/Patient.read\n- path: /.well-known/smart-configuration\n  method: get\n  operationId: getSmartConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n\
  \    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Patient\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Observation\n  method: get\n  operationId: searchObservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n\
  \    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Condition\n  method: get\n  operationId: searchCondition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Encounter\n  method: get\n  operationId: searchEncounter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n\
  \    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /MedicationRequest\n  method: get\n  operationId: searchMedicationRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /AllergyIntolerance\n  method: get\n  operationId: searchAllergyIntolerance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n\
  \    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /DocumentReference\n  method: get\n  operationId: searchDocumentReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Group/{id}/$export\n  method: get\n  operationId: bulkExportGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/agentic-access/temple-health-agentic-access.yml
summary_line: 11 operations
tags:
- Academic Medical Center
- CMS Interoperability
- Cures Act
- DSTU2
- Epic
- FHIR
- Fox Chase Cancer Center
- HL7
- Healthcare
- Hospital System
- MyChart
- Authentication
- Patient Access
- Price Transparency
- R4
- SMART on FHIR
- Temple University
- US Core
- USCDI
---
