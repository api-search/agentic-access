---
acting_count: 0
action_class_counts:
  connected: 26
api_specs:
- filename: clever-care-coverage-openapi.json
  format: json
  label: Clever Care FHIR Coverage
  slug: clever-care-fhir-coverage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-coverage-openapi.json
- filename: clever-care-endpoint-openapi.json
  format: json
  label: Clever Care FHIR Endpoint
  slug: clever-care-fhir-endpoint
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-endpoint-openapi.json
- filename: clever-care-explanation-of-benefit-openapi.json
  format: json
  label: Clever Care FHIR ExplanationOfBenefit
  slug: clever-care-fhir-explanationofbenefit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-explanation-of-benefit-openapi.json
- filename: clever-care-healthcare-service-openapi.json
  format: json
  label: Clever Care FHIR HealthcareService
  slug: clever-care-fhir-healthcareservice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-healthcare-service-openapi.json
- filename: clever-care-insurance-plan-openapi.json
  format: json
  label: Clever Care FHIR InsurancePlan
  slug: clever-care-fhir-insuranceplan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-insurance-plan-openapi.json
- filename: clever-care-list-openapi.json
  format: json
  label: Clever Care FHIR List
  slug: clever-care-fhir-list
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-list-openapi.json
- filename: clever-care-location-openapi.json
  format: json
  label: Clever Care FHIR Location
  slug: clever-care-fhir-location
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-location-openapi.json
- filename: clever-care-medication-knowledge-openapi.json
  format: json
  label: Clever Care FHIR MedicationKnowledge
  slug: clever-care-fhir-medicationknowledge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-medication-knowledge-openapi.json
- filename: clever-care-organization-openapi.json
  format: json
  label: Clever Care FHIR Organization
  slug: clever-care-fhir-organization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-organization-openapi.json
- filename: clever-care-organization-affiliation-openapi.json
  format: json
  label: Clever Care FHIR OrganizationAffiliation
  slug: clever-care-fhir-organizationaffiliation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-organization-affiliation-openapi.json
- filename: clever-care-patient-openapi.json
  format: json
  label: Clever Care FHIR Patient
  slug: clever-care-fhir-patient
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-patient-openapi.json
- filename: clever-care-practitioner-openapi.json
  format: json
  label: Clever Care FHIR Practitioner
  slug: clever-care-fhir-practitioner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-practitioner-openapi.json
- filename: clever-care-practitioner-role-openapi.json
  format: json
  label: Clever Care FHIR PractitionerRole
  slug: clever-care-fhir-practitionerrole
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-practitioner-role-openapi.json
consequence_counts:
  read: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clever Care Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Clever Care exposes 26 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clever Care
provider_slug: clever-care
slug: clever-care-agentic-access
source_filename: clever-care-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/clever-care-coverage-openapi.json, openapi/clever-care-endpoint-openapi.json,\n  openapi/clever-care-explanation-of-benefit-openapi.json, openapi/clever-care-healthcare-service-openapi.json,\n  openapi/clever-care-insurance-plan-openapi.json, openapi/clever-care-list-openapi.json, openapi/clever-care-location-openapi.json,\n  openapi/clever-care-medication-knowledge-openapi.json, openapi/clever-care-organization-affiliation-openapi.json,\n  openapi/clever-care-organization-openapi.json, openapi/clever-care-patient-openapi.json, openapi/clever-care-practitioner-openapi.json,\n  openapi/clever-care-practitioner-role-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n\
  \    connected: 26\n  by_consequence:\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: searchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchExplanationOfBenefit\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchHealthcareService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readHealthcareService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchInsurancePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method:\
  \ get\n  operationId: readInsurancePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /\n  method: get\n  operationId: searchMedicationKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readMedicationKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchOrganizationAffiliation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readOrganizationAffiliation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readPractitioner\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: searchPractitionerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{id}\n  method: get\n  operationId: readPractitionerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/agentic-access/clever-care-agentic-access.yml
summary_line: 26 operations
tags:
- Company
- Life Sciences
- Health Insurance
- Medicare Advantage
- Healthcare
- FHIR
- Healthcare Interoperability
- Patient Access
- Provider Directory
- CMS-9115-F
---
