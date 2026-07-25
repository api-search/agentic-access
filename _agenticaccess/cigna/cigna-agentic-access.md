---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: cigna-bulk-data-api-openapi.yml
  format: yaml
  label: Cigna Bulk Data API
  slug: cigna-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-bulk-data-api-openapi.yml
- filename: cigna-condition-api-openapi.yml
  format: yaml
  label: Cigna Condition API
  slug: cigna-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-condition-api-openapi.yml
- filename: cigna-coverage-api-openapi.yml
  format: yaml
  label: Cigna Coverage API
  slug: cigna-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-coverage-api-openapi.yml
- filename: cigna-encounter-api-openapi.yml
  format: yaml
  label: Cigna Encounter API
  slug: cigna-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-encounter-api-openapi.yml
- filename: cigna-explanationofbenefit-api-openapi.yml
  format: yaml
  label: Cigna ExplanationOfBenefit API
  slug: cigna-explanationofbenefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-explanationofbenefit-api-openapi.yml
- filename: cigna-healthcareservice-api-openapi.yml
  format: yaml
  label: Cigna HealthcareService API
  slug: cigna-healthcareservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-healthcareservice-api-openapi.yml
- filename: cigna-insuranceplan-api-openapi.yml
  format: yaml
  label: Cigna InsurancePlan API
  slug: cigna-insuranceplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-insuranceplan-api-openapi.yml
- filename: cigna-location-api-openapi.yml
  format: yaml
  label: Cigna Location API
  slug: cigna-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-location-api-openapi.yml
- filename: cigna-medicationknowledge-api-openapi.yml
  format: yaml
  label: Cigna MedicationKnowledge API
  slug: cigna-medicationknowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-medicationknowledge-api-openapi.yml
- filename: cigna-medicationrequest-api-openapi.yml
  format: yaml
  label: Cigna MedicationRequest API
  slug: cigna-medicationrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-medicationrequest-api-openapi.yml
- filename: cigna-observation-api-openapi.yml
  format: yaml
  label: Cigna Observation API
  slug: cigna-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-observation-api-openapi.yml
- filename: cigna-organization-api-openapi.yml
  format: yaml
  label: Cigna Organization API
  slug: cigna-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-organization-api-openapi.yml
- filename: cigna-patient-api-openapi.yml
  format: yaml
  label: Cigna Patient API
  slug: cigna-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-patient-api-openapi.yml
- filename: cigna-practitioner-api-openapi.yml
  format: yaml
  label: Cigna Practitioner API
  slug: cigna-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-practitioner-api-openapi.yml
- filename: cigna-practitionerrole-api-openapi.yml
  format: yaml
  label: Cigna PractitionerRole API
  slug: cigna-practitionerrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-practitionerrole-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cigna Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Cigna exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cigna
provider_slug: cigna
slug: cigna-agentic-access
source_filename: cigna-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cigna-drug-formulary-api-openapi.yml, openapi/cigna-patient-access-api-openapi.yml,\n  openapi/cigna-provider-access-api-openapi.yml, openapi/cigna-provider-directory-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /InsurancePlan\n  method: get\n  operationId: searchFormularyPlan\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MedicationKnowledge\n  method: get\n  operationId: searchMedicationKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /$userinfo\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Coverage\n  method: get\n\
  \  operationId: searchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExplanationOfBenefit\n  method: get\n  operationId: searchExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Encounter\n  method: get\n  operationId: searchEncounter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Observation\n  method: get\n  operationId: searchObservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Condition\n  method: get\n  operationId: searchCondition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /MedicationRequest\n  method: get\n  operationId: searchMedicationRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Group/{groupId}/$export\n  method: get\n  operationId: bulkExportGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{patientId}/$everything\n  method: get\n  operationId: getPatientEverything\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n\
  \  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner\n  method: get\n  operationId: searchPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization\n  method: get\n  operationId: searchOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Location\n  method: get\n  operationId: searchLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /HealthcareService\n  method: get\n  operationId: searchHealthcareService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PractitionerRole\n  method: get\n  operationId: searchPractitionerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /InsurancePlan\n  method: get\n  operationId: searchInsurancePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/agentic-access/cigna-agentic-access.yml
summary_line: 22 operations
tags:
- CMS Interoperability
- Da Vinci
- Drug Formulary
- FHIR
- Health Insurance
- Healthcare
- Patient Access
- Provider Directory
- SMART on FHIR
- Fortune 100
---
