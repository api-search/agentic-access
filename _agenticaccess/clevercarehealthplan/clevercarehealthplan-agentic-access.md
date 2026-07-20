---
acting_count: 0
action_class_counts:
  connected: 27
api_specs:
- filename: clevercarehealthplan-fhir-openapi.yml
  format: yaml
  label: Clever Care Health Plan FHIR R4 API
  slug: clever-care-health-plan-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/openapi/clevercarehealthplan-fhir-openapi.yml
consequence_counts:
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clevercarehealthplan Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Clever Care Health Plan exposes 27 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clever Care Health Plan
provider_slug: clevercarehealthplan
slug: clevercarehealthplan-agentic-access
source_filename: clevercarehealthplan-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/clevercarehealthplan-fhir-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 27\n  by_consequence:\n    read: 27\n  human_in_the_loop_required: 0\noperations:\n- path: /Patient\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/*.cruds\n    - user/*.cruds\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/*.cruds\n    - user/*.cruds\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /ExplanationOfBenefit\n  method: get\n  operationId: searchExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/*.cruds\n    - user/*.cruds\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExplanationOfBenefit/{id}\n  method: get\n  operationId: readExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/*.cruds\n    - user/*.cruds\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Coverage\n  method: get\n  operationId: searchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/*.cruds\n    - user/*.cruds\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Coverage/{id}\n  method: get\n  operationId: readCoverage\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - patient/*.cruds\n    - user/*.cruds\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization\n  method: get\n  operationId: searchOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization/{id}\n  method: get\n  operationId: readOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OrganizationAffiliation\n  method: get\n  operationId: searchOrganizationAffiliation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OrganizationAffiliation/{id}\n  method: get\n  operationId: readOrganizationAffiliation\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner\n  method: get\n  operationId: searchPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner/{id}\n  method: get\n  operationId: readPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PractitionerRole\n  method: get\n  operationId: searchPractitionerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PractitionerRole/{id}\n  method: get\n  operationId: readPractitionerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /HealthcareService\n\
  \  method: get\n  operationId: searchHealthcareService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /HealthcareService/{id}\n  method: get\n  operationId: readHealthcareService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Location\n  method: get\n  operationId: searchLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Location/{id}\n  method: get\n  operationId: readLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Endpoint\n  method: get\n  operationId: searchEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Endpoint/{id}\n  method: get\n  operationId: readEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /InsurancePlan\n  method: get\n  operationId: searchInsurancePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /InsurancePlan/{id}\n  method: get\n  operationId: readInsurancePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MedicationKnowledge\n  method: get\n  operationId: searchMedicationKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MedicationKnowledge/{id}\n\
  \  method: get\n  operationId: readMedicationKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /List\n  method: get\n  operationId: searchList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /List/{id}\n  method: get\n  operationId: readList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/agentic-access/clevercarehealthplan-agentic-access.yml
summary_line: 27 operations
tags:
- Company
- Healthcare
- Health Insurance
- Medicare Advantage
- FHIR
- Interoperability
- Patient Access
- Provider Directory
- Drug Formulary
---
