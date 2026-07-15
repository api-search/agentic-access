---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 19
api_specs:
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Clients API
  slug: intakeq-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Appointments API
  slug: intakeq-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Intake Forms API
  slug: intakeq-intake-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Treatment Notes API
  slug: intakeq-treatment-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Invoices API
  slug: intakeq-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Files API
  slug: intakeq-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
consequence_counts:
  physical: 2
  read: 19
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Intakeq Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /intakes/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /intakes/send
operation_count: 30
overview: 'IntakeQ exposes 30 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 9 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IntakeQ
provider_slug: intakeq
slug: intakeq-agentic-access
source_filename: intakeq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/intakeq-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 19\n    acting: 11\n  by_consequence:\n    read: 19\n    write: 9\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /clients\n  method: get\n  operationId: queryClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients\n  method: post\n  operationId: saveClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clientTags\n  method: post\n  operationId: addClientTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clientTags\n  method: delete\n  operationId: removeClientTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/diagnoses\n  method: get\n  operationId: queryClientDiagnoses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /appointments\n  method: get\n  operationId: queryAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments\n  method: post\n  operationId: createAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments\n  method: put\n  operationId: updateAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/{appointmentId}\n  method: get\n  operationId:\
  \ getAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/settings\n  method: get\n  operationId: getBookingSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/cancellation\n  method: post\n  operationId: cancelAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intakes/summary\n  method: get\n  operationId: queryIntakes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intakes/{intakeId}\n\
  \  method: get\n  operationId: getIntake\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intakes/{intakeId}/pdf\n  method: get\n  operationId: downloadIntakePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intakes/{intakeId}/consent/{consentFormId}/pdf\n  method: get\n  operationId: downloadConsentPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intakes/send\n  method: post\n  operationId: sendIntake\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /intakes/resend\n  method: post\n  operationId: resendIntake\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intakes\n  method: post\n  operationId: updateIntakeOfficeAnswers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /questionnaires\n  method: get\n  operationId: listQuestionnaires\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /practitioners\n  method: get\n  operationId: listPractitioners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notes/summary\n  method: get\n  operationId: queryTreatmentNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notes/{noteId}\n  method: get\n  operationId: getTreatmentNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notes/{noteId}/pdf\n  method: get\n  operationId: downloadTreatmentNotePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: queryInvoices\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoiceId}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: get\n  operationId: getClientFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: get\n  operationId: getFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}\n\
  \  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{clientId}\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/agentic-access/intakeq-agentic-access.yml
summary_line: 30 operations · 11 acting
tags:
- Practice Management
- Intake Forms
- Scheduling
- Health and Wellness
- EHR
- Telehealth
- HIPAA
---
