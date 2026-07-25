---
acting_count: 0
action_class_counts:
  connected: 21
api_specs:
- filename: jefferson-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Jefferson Health Allergy Intolerance API
  slug: jefferson-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-allergy-intolerance-api-openapi.yml
- filename: jefferson-health-bulk-data-api-openapi.yml
  format: yaml
  label: Jefferson Health Bulk Data API
  slug: jefferson-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-bulk-data-api-openapi.yml
- filename: jefferson-health-condition-api-openapi.yml
  format: yaml
  label: Jefferson Health Condition API
  slug: jefferson-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-condition-api-openapi.yml
- filename: jefferson-health-document-reference-api-openapi.yml
  format: yaml
  label: Jefferson Health Document Reference API
  slug: jefferson-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-document-reference-api-openapi.yml
- filename: jefferson-health-encounter-api-openapi.yml
  format: yaml
  label: Jefferson Health Encounter API
  slug: jefferson-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-encounter-api-openapi.yml
- filename: jefferson-health-endpoint-api-openapi.yml
  format: yaml
  label: Jefferson Health Endpoint API
  slug: jefferson-health-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-endpoint-api-openapi.yml
- filename: jefferson-health-healthcare-service-api-openapi.yml
  format: yaml
  label: Jefferson Health Healthcare Service API
  slug: jefferson-health-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-healthcare-service-api-openapi.yml
- filename: jefferson-health-insurance-plan-api-openapi.yml
  format: yaml
  label: Jefferson Health Insurance Plan API
  slug: jefferson-health-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-insurance-plan-api-openapi.yml
- filename: jefferson-health-location-api-openapi.yml
  format: yaml
  label: Jefferson Health Location API
  slug: jefferson-health-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-location-api-openapi.yml
- filename: jefferson-health-medication-request-api-openapi.yml
  format: yaml
  label: Jefferson Health Medication Request API
  slug: jefferson-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-medication-request-api-openapi.yml
- filename: jefferson-health-metadata-api-openapi.yml
  format: yaml
  label: Jefferson Health Metadata API
  slug: jefferson-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-metadata-api-openapi.yml
- filename: jefferson-health-observation-api-openapi.yml
  format: yaml
  label: Jefferson Health Observation API
  slug: jefferson-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-observation-api-openapi.yml
- filename: jefferson-health-organization-api-openapi.yml
  format: yaml
  label: Jefferson Health Organization API
  slug: jefferson-health-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-organization-api-openapi.yml
- filename: jefferson-health-patient-api-openapi.yml
  format: yaml
  label: Jefferson Health Patient API
  slug: jefferson-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-patient-api-openapi.yml
- filename: jefferson-health-practitioner-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner API
  slug: jefferson-health-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-api-openapi.yml
- filename: jefferson-health-practitioner-role-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner Role API
  slug: jefferson-health-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-role-api-openapi.yml
consequence_counts:
  read: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jefferson Health Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Jefferson Health exposes 21 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jefferson Health
provider_slug: jefferson-health
slug: jefferson-health-agentic-access
source_filename: jefferson-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/jefferson-health-jhp-provider-directory-fhir-api-openapi.yml, openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 21\n  by_consequence:\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner/{id}\n  method: get\n  operationId: readPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /Practitioner\n  method: get\n  operationId: searchPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PractitionerRole\n  method: get\n  operationId: searchPractitionerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization/{id}\n  method: get\n  operationId: readOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization\n  method: get\n  operationId: searchOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Location\n  method: get\n  operationId: searchLocation\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /HealthcareService\n  method: get\n  operationId: searchHealthcareService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /InsurancePlan\n  method: get\n  operationId: searchInsurancePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Endpoint\n  method: get\n  operationId: searchEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /.well-known/smart-configuration\n  method: get\n  operationId: getSmartConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Patient\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Observation\n  method: get\n  operationId: searchObservation\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Condition\n  method: get\n  operationId: searchCondition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /Encounter\n  method: get\n  operationId: searchEncounter\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /MedicationRequest\n  method: get\n  operationId: searchMedicationRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n\
  - path: /AllergyIntolerance\n  method: get\n  operationId: searchAllergyIntolerance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n- path: /DocumentReference\n  method: get\n  operationId: searchDocumentReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n\
  \    - patient/Observation.read\n    - patient/Patient.read\n- path: /Group/{id}/$export\n  method: get\n  operationId: bulkExportGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fhirUser\n    - launch\n    - offline_access\n    - openid\n    - patient/AllergyIntolerance.read\n    - patient/Condition.read\n    - patient/DocumentReference.read\n    - patient/Encounter.read\n    - patient/MedicationRequest.read\n    - patient/Observation.read\n    - patient/Patient.read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/agentic-access/jefferson-health-agentic-access.yml
summary_line: 21 operations
tags:
- Academic Medical Center
- CARIN Blue Button
- CMS Interoperability
- Cures Act
- Da Vinci Plan-Net
- Epic
- FHIR
- HL7
- Healthcare
- Hospital System
- MyChart
- OAuth 2.0
- Patient Access
- Provider Directory
- SMART on FHIR
- US Core
- USCDI
---
