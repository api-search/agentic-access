---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 27
api_specs:
- filename: predoc-authentication-api-openapi.yml
  format: yaml
  label: Predoc Authentication API
  slug: predoc-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/openapi/predoc-authentication-api-openapi.yml
- filename: predoc-documents-api-openapi.yml
  format: yaml
  label: Predoc Documents API
  slug: predoc-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/openapi/predoc-documents-api-openapi.yml
- filename: predoc-events-api-openapi.yml
  format: yaml
  label: Predoc Events API
  slug: predoc-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/openapi/predoc-events-api-openapi.yml
- filename: predoc-patient-api-openapi.yml
  format: yaml
  label: Predoc Patient API
  slug: predoc-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/openapi/predoc-patient-api-openapi.yml
- filename: predoc-record-request-api-openapi.yml
  format: yaml
  label: Predoc Record Request API
  slug: predoc-record-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/openapi/predoc-record-request-api-openapi.yml
- filename: predoc-record-upload-api-openapi.yml
  format: yaml
  label: Predoc Record Upload API
  slug: predoc-record-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/openapi/predoc-record-upload-api-openapi.yml
- filename: predoc-retrieval-api-openapi.yml
  format: yaml
  label: Predoc Retrieval API
  slug: predoc-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/openapi/predoc-retrieval-api-openapi.yml
consequence_counts:
  read: 27
  safety-critical: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 13
kind: agentic-access
layout: agentic-access
method: generated
name: Predoc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/events
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/events/{configurationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/events/{configurationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/patients/{patientId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/patients/{patientId}/requests
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/patients/{patientId}/summary
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/records/upload/anonymous
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/requests/{requestId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/retrievals/previous-providers/{retrievalId}/close
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/patients
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/records/upload
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/requests
operation_count: 40
overview: 'Predoc exposes 40 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 13 safety-critical.


  13 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Predoc
provider_slug: predoc
slug: predoc-agentic-access
source_filename: predoc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/predoc-partner-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    acting: 13\n    connected: 27\n  by_consequence:\n    safety-critical: 13\n    read: 27\n  human_in_the_loop_required: 13\noperations:\n- path: /v1/auth/token\n  method: post\n  operationId: AuthController_signIn_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/documents/{documentId}\n  method: get\n \
  \ operationId: DocumentController_getPatientClinicalSummary_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: post\n  operationId: WebhookConfigurationController_createWebhookConfiguration_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/events\n  method: get\n  operationId: WebhookConfigurationController_listWebhookConfigurations_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{configurationId}\n  method: patch\n  operationId: WebhookConfigurationController_updateWebhookConfiguration_v1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/events/{configurationId}\n  method: delete\n  operationId: WebhookConfigurationController_deleteWebhookConfiguration_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/patients\n  method: get\n  operationId: PatientController_searchPatientsByInformation_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/patients/{patientId}\n  method: get\n  operationId: PatientController_getPatientInformation_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}\n  method: patch\n  operationId: PatientController_updatePatientInformation_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/patients/{patientId}/additional-records\n  method: get\n  operationId: PatientDocumentsController_getPatientAdditionalRecords_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/curated-patient-data/{classificationGroupType}\n\
  \  method: get\n  operationId: CuratedPatientDataController_getCuratedPatientData_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/documents\n  method: get\n  operationId: PatientDocumentsController_getPatientDocuments_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/drug-allergies\n  method: get\n  operationId: PatientDocumentsController_getPatientDrugAllergies_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/facesheets\n  method: get\n  operationId: PatientDocumentsController_getPatientFacesheets_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/facesheets/requests/{facesheetRequestId}/output\n  method: get\n  operationId: PatientDocumentsController_getPatientFacesheetOutput_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/hie-docs\n  method: get\n  operationId: PatientDocumentsController_getPatientHieDocs_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/imaging-results\n  method: get\n  operationId: PatientDocumentsController_getPatientImagingResults_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/lab-results\n  method: get\n  operationId: PatientController_getPatientLabResultsBySearch_v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/lab-results/available\n  method: get\n  operationId: PatientController_getAvailablePatientChemistries_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/lab-tests\n  method: get\n  operationId: PatientDocumentsController_getPatientLabTests_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/medications\n  method: get\n  operationId: PatientDocumentsController_getPatientMedications_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/other-records\n\
  \  method: get\n  operationId: PatientDocumentsController_getPatientOtherRecords_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/procedure-notes\n  method: get\n  operationId: PatientDocumentsController_getPatientProcedureNotes_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/provider-notes\n  method: get\n  operationId: PatientDocumentsController_getPatientProviderFacilityNotes_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/requests\n  method: get\n  operationId: PatientController_getPatientRequests_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/requests\n  method: post\n  operationId: PatientController_addRequestToExistingPatient_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/patients/{patientId}/summary\n  method: post\n  operationId: PatientController_requestPatientClinicalSummary_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/patients/{patientId}/vaccine-documents\n  method:\
  \ get\n  operationId: PatientDocumentsController_getPatientVaccineDocuments_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patientId}/vaccine-records\n  method: get\n  operationId: PatientDocumentsController_getPatientVaccineRecords_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/records/upload/anonymous\n  method: post\n  operationId: RecordUploadController_uploadAnonymousRecord_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/records/uploads/{recordUploadId}/status\n  method:\
  \ get\n  operationId: RecordUploadController_getAnonymousRecordUploadStatus_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/requests/facesheet-configs\n  method: get\n  operationId: RequestController_facesheetConfigs_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/requests/{requestId}\n  method: patch\n  operationId: RequestController_updateExistingRecordRequest_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/retrievals/previous-providers/{retrievalId}\n  method: get\n  operationId: RetrievalController_getRetrieval_v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/retrievals/previous-providers/{retrievalId}/close\n  method: post\n  operationId: RetrievalController_closeRetrieval_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/patients\n  method: post\n  operationId: PatientController_createPatient_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /v2/patients/{patientId}/documents/search\n  method: post\n  operationId: PatientController_searchPatientDocuments_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/records/upload\n  method: post\n  operationId: RecordUploadController_uploadRecordV2_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/requests\n  method: post\n  operationId: RequestController_createRecordRequestV2_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/requests\n  method: get\n  operationId: RequestController_getListOfRecordRequests_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predoc/refs/heads/main/agentic-access/predoc-agentic-access.yml
summary_line: 40 operations · 13 acting · 13 human-in-the-loop
tags:
- Company
- Healthcare
- Medical Records
- Health Information Exchange
- FHIR
- Clinical Data
- Artificial Intelligence
- Interoperability
- EHR Integration
- Webhook
- Clinical Research
---
