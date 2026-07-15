---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 21
api_specs:
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Patients API
  slug: nookal-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Appointments API
  slug: nookal-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Clinic API
  slug: nookal-clinic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Invoices API
  slug: nookal-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Verification API
  slug: nookal-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
consequence_counts:
  physical: 5
  read: 21
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nookal Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /addInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /addPaymentToInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getInvoicePayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getInvoices
operation_count: 36
overview: 'Nookal exposes 36 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 10 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nookal
provider_slug: nookal
slug: nookal-agentic-access
source_filename: nookal-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nookal-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 21\n    acting: 15\n  by_consequence:\n    read: 21\n    write: 10\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /verify\n  method: get\n  operationId: verify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getLocations\n  method: get\n  operationId: getLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getLocationLogo\n  method: get\n\
  \  operationId: getLocationLogo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getPractitioners\n  method: get\n  operationId: getPractitioners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getPractitionerPhoto\n  method: get\n  operationId: getPractitionerPhoto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getAppointmentTypes\n  method: get\n  operationId: getAppointmentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getClassTypes\n  method: get\n  operationId: getClassTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getStockList\n  method: get\n  operationId: getStockList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getPatients\n  method: get\n  operationId: getPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searchPatients\n  method: get\n  operationId: searchPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getCases\n  method: get\n  operationId: getCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getAllCases\n  method: get\n  operationId: getAllCases\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addPatient\n  method: post\n  operationId: addPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /editPatient\n  method: post\n  operationId: editPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getTreatmentNotes\n  method: get\n  operationId: getTreatmentNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /getAllTreatmentNotes\n  method: get\n  operationId: getAllTreatmentNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addTreatmentNote\n  method: post\n  operationId: addTreatmentNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getPatientFiles\n  method: get\n  operationId: getPatientFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getFileUrl\n  method: get\n  operationId: getFileUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /addCase\n  method: post\n  operationId: addCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /updatePatientMedicareDetails\n  method: post\n  operationId: updatePatientMedicareDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getAppointments\n  method: get\n  operationId: getAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getAppointmentAvailabilities\n\
  \  method: get\n  operationId: getAppointmentAvailabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getClassAvailabilities\n  method: get\n  operationId: getClassAvailabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addAppointmentBooking\n  method: post\n  operationId: addAppointmentBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /updateAppointmentBooking\n  method: post\n  operationId: updateAppointmentBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addClassBooking\n  method: post\n  operationId: addClassBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancelAppointment\n  method: post\n  operationId: cancelAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rebookAppointment\n  method: post\n  operationId: rebookAppointment\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getClassParticipants\n  method: get\n  operationId: getClassParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getWaitingList\n  method: get\n  operationId: getWaitingList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getInvoices\n  method: post\n  operationId: getInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getInvoice\n  method: post\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addInvoice\n  method: post\n  operationId: addInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addPaymentToInvoice\n  method: post\n  operationId: addPaymentToInvoice\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getInvoicePayments\n  method: post\n  operationId: getInvoicePayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/agentic-access/nookal-agentic-access.yml
summary_line: 36 operations · 15 acting
tags:
- Practice Management
- Healthcare
- Allied Health
- Appointments
- Scheduling
- Patients
- Clinics
- Bookings
- Physiotherapy
- SaaS
---
