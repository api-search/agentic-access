---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 17
api_specs:
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Patients API
  slug: cliniko-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Appointments API
  slug: cliniko-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Practitioners and Businesses API
  slug: cliniko-practitioners-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Appointment Types API
  slug: cliniko-appointment-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Invoices API
  slug: cliniko-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Treatment Notes API
  slug: cliniko-treatment-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
consequence_counts:
  read: 17
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cliniko Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Cliniko exposes 25 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cliniko
provider_slug: cliniko
slug: cliniko-agentic-access
source_filename: cliniko-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cliniko-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 17\n    acting: 8\n  by_consequence:\n    read: 17\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /patients\n  method: get\n  operationId: listPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients\n  method: post\n  operationId: createPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{id}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{id}\n  method: patch\n  operationId: updatePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{id}/archive\n  method: post\n  operationId: archivePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /patients/{id}/unarchive\n  method: post\n  operationId: unarchivePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /individual_appointments\n  method: get\n  operationId: listIndividualAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /individual_appointments\n  method: post\n  operationId: createIndividualAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /individual_appointments/{id}\n\
  \  method: get\n  operationId: getIndividualAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /individual_appointments/{id}\n  method: patch\n  operationId: updateIndividualAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /individual_appointments/{id}/cancel\n  method: patch\n  operationId: cancelIndividualAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /individual_appointments/{id}/conflicts\n\
  \  method: get\n  operationId: getIndividualAppointmentConflicts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{id}\n  method: get\n  operationId: getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /practitioners\n  method: get\n  operationId: listPractitioners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /practitioners/{id}\n  method: get\n  operationId: getPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses\n  method: get\n  operationId: listBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{id}\n  method: get\n  operationId: getBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointment_types\n  method: get\n  operationId: listAppointmentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointment_types/{id}\n  method: get\n  operationId: getAppointmentType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId:\
  \ listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /treatment_notes\n  method: get\n  operationId: listTreatmentNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /treatment_notes\n  method: post\n  operationId: createTreatmentNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /treatment_notes/{id}\n  method: get\n  operationId:\
  \ getTreatmentNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/agentic-access/cliniko-agentic-access.yml
summary_line: 25 operations · 8 acting
tags:
- Practice Management
- Healthcare
- Allied Health
- Appointments
- Scheduling
- Patients
- EHR
- Clinics
- Bookings
- SaaS
---
