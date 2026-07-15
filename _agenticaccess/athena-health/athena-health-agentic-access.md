---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 31
api_specs:
- filename: athenahealth-athenaone-rest-api-openapi.yml
  format: yaml
  label: athenahealth athenaOne REST API
  slug: athenahealth-athenaone-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-athenaone-rest-api-openapi.yml
- filename: athenahealth-fhir-r4-api-openapi.yml
  format: yaml
  label: athenahealth FHIR R4 API
  slug: athenahealth-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-r4-api-openapi.yml
- filename: athenahealth-fhir-subscriptions-api-openapi.yml
  format: yaml
  label: athenahealth FHIR Subscriptions API
  slug: athenahealth-fhir-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-subscriptions-api-openapi.yml
- filename: athenahealth-fhir-bulk-data-api-openapi.yml
  format: yaml
  label: athenahealth FHIR Bulk Data Access API
  slug: athenahealth-fhir-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-bulk-data-api-openapi.yml
- filename: athenahealth-cds-hooks-api-openapi.yml
  format: yaml
  label: athenahealth CDS Hooks API
  slug: athenahealth-cds-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-cds-hooks-api-openapi.yml
consequence_counts:
  read: 31
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Athena Health Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'athenahealth exposes 40 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: athenahealth
provider_slug: athena-health
slug: athena-health-agentic-access
source_filename: athena-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/athenahealth-athenaone-rest-api-openapi.yml, openapi/athenahealth-cds-hooks-api-openapi.yml,\n  openapi/athenahealth-fhir-bulk-data-api-openapi.yml, openapi/athenahealth-fhir-r4-api-openapi.yml,\n  openapi/athenahealth-fhir-subscriptions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 31\n    acting: 9\n  by_consequence:\n    read: 31\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /patients\n  method: get\n  operationId: searchPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients\n  method:\
  \ post\n  operationId: createPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{patientid}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientid}\n  method: put\n  operationId: updatePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments\n  method: get\n  operationId: searchAppointments\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/open\n  method: get\n  operationId: getOpenAppointmentSlots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/{appointmentid}\n  method: get\n  operationId: getAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/{appointmentid}/cancel\n  method: put\n  operationId: cancelAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/{appointmentid}/checkin\n  method: post\n  operationId:\
  \ checkInAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/{appointmentid}/reschedule\n  method: put\n  operationId: rescheduleAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chart/{patientid}/encounters\n  method: get\n  operationId: listPatientEncounters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/encounter/{encounterid}\n  method: get\n  operationId: getEncounter\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims\n  method: get\n  operationId: searchClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientid}/documents\n  method: get\n  operationId: listPatientDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /departments\n  method: get\n  operationId: listDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /practiceinfo\n  method: get\n  operationId: getPracticeInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cds-services\n  method: get\n  operationId: discoverCdsServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cds-services/{id}\n  method: post\n  operationId: invokeCdsService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Group/{id}/$export\n  method: get\n  operationId: groupBulkExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /bulk/status/{jobid}\n  method: get\n  operationId: getBulkExportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk/status/{jobid}\n  method: delete\n  operationId: cancelBulkExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient\n  method: get\n  operationId: searchFhirPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}\n  method: get\n  operationId: readFhirPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Encounter\n  method: get\n  operationId: searchFhirEncounters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Encounter/{id}\n  method: get\n  operationId: readFhirEncounter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Observation\n  method: get\n  operationId: searchFhirObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Condition\n  method: get\n  operationId: searchFhirConditions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MedicationRequest\n  method: get\n  operationId: searchFhirMedicationRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AllergyIntolerance\n  method: get\n  operationId: searchFhirAllergies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DocumentReference\n  method: get\n  operationId: searchFhirDocumentReferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DiagnosticReport\n  method: get\n  operationId: searchFhirDiagnosticReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /Immunization\n  method: get\n  operationId: searchFhirImmunizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Appointment\n  method: get\n  operationId: searchFhirAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Subscription\n  method: get\n  operationId: searchSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Subscription\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /Subscription/{id}\n  method: get\n  operationId: readSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Subscription/{id}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Subscription/{id}/$status\n  method: get\n  operationId: getSubscriptionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/agentic-access/athena-health-agentic-access.yml
summary_line: 40 operations · 9 acting
tags:
- EHR
- Electronic Health Records
- Healthcare
- HL7
- FHIR
- Interoperability
- Practice Management
- Revenue Cycle Management
- USCDI
- Cures Act
- SMART on FHIR
- CDS Hooks
- Cloud EHR
---
