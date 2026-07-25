---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: varian-medical-systems-allergyintolerance-api-openapi.yml
  format: yaml
  label: Varian Medical Systems AllergyIntolerance API
  slug: varian-medical-systems-allergyintolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-allergyintolerance-api-openapi.yml
- filename: varian-medical-systems-careplan-api-openapi.yml
  format: yaml
  label: Varian Medical Systems CarePlan API
  slug: varian-medical-systems-careplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-careplan-api-openapi.yml
- filename: varian-medical-systems-condition-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Condition API
  slug: varian-medical-systems-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-condition-api-openapi.yml
- filename: varian-medical-systems-diagnosticreport-api-openapi.yml
  format: yaml
  label: Varian Medical Systems DiagnosticReport API
  slug: varian-medical-systems-diagnosticreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-diagnosticreport-api-openapi.yml
- filename: varian-medical-systems-documentreference-api-openapi.yml
  format: yaml
  label: Varian Medical Systems DocumentReference API
  slug: varian-medical-systems-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-documentreference-api-openapi.yml
- filename: varian-medical-systems-goal-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Goal API
  slug: varian-medical-systems-goal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-goal-api-openapi.yml
- filename: varian-medical-systems-medicationrequest-api-openapi.yml
  format: yaml
  label: Varian Medical Systems MedicationRequest API
  slug: varian-medical-systems-medicationrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-medicationrequest-api-openapi.yml
- filename: varian-medical-systems-metadata-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Metadata API
  slug: varian-medical-systems-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-metadata-api-openapi.yml
- filename: varian-medical-systems-observation-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Observation API
  slug: varian-medical-systems-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-observation-api-openapi.yml
- filename: varian-medical-systems-patient-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Patient API
  slug: varian-medical-systems-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-patient-api-openapi.yml
- filename: varian-medical-systems-procedure-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Procedure API
  slug: varian-medical-systems-procedure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-procedure-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Varian Medical Systems Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Varian Medical Systems exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Varian Medical Systems
provider_slug: varian-medical-systems
slug: varian-medical-systems-agentic-access
source_filename: varian-medical-systems-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/varian-aria-fhir-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /Patient\n  method: get\n  operationId: searchPatients\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /Patient/{id}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /Condition\n  method: get\n  operationId: searchConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /Condition/{id}\n  method:\
  \ get\n  operationId: getCondition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /Procedure\n  method: get\n  operationId: searchProcedures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /Procedure/{id}\n  method: get\n  operationId: getProcedure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n\
  \    - patient/Patient.read\n    - patient/Procedure.read\n- path: /Observation\n  method: get\n  operationId: searchObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /Observation/{id}\n  method: get\n  operationId: getObservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /DiagnosticReport\n  method: get\n  operationId: searchDiagnosticReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /DiagnosticReport/{id}\n  method: get\n  operationId: getDiagnosticReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /CarePlan\n  method: get\n  operationId: searchCarePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /MedicationRequest\n  method: get\n  operationId: searchMedicationRequests\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /AllergyIntolerance\n  method: get\n  operationId: searchAllergyIntolerances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n- path: /DocumentReference\n  method: get\n  operationId: searchDocumentReferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n\
  \    - patient/Patient.read\n    - patient/Procedure.read\n- path: /Goal\n  method: get\n  operationId: searchGoals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - launch/patient\n    - patient/Condition.read\n    - patient/Observation.read\n    - patient/Patient.read\n    - patient/Procedure.read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/agentic-access/varian-medical-systems-agentic-access.yml
summary_line: 16 operations
tags:
- Healthcare
- Oncology
- Medical Devices
- FHIR
- Radiation Therapy
- Health IT
- Fortune 1000
---
