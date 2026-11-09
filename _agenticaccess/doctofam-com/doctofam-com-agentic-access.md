---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 13
api_specs:
- filename: doctofam-com-appointments-api-openapi.yml
  format: yaml
  label: Doctofam Appointments API
  slug: doctofam-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-appointments-api-openapi.yml
- filename: doctofam-com-clinics-api-openapi.yml
  format: yaml
  label: Doctofam Clinics API
  slug: doctofam-com-clinics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-clinics-api-openapi.yml
- filename: doctofam-com-invoices-api-openapi.yml
  format: yaml
  label: Doctofam Invoices API
  slug: doctofam-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-invoices-api-openapi.yml
- filename: doctofam-com-patients-api-openapi.yml
  format: yaml
  label: Doctofam Patients API
  slug: doctofam-com-patients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-patients-api-openapi.yml
- filename: doctofam-com-payments-api-openapi.yml
  format: yaml
  label: Doctofam Payments API
  slug: doctofam-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-payments-api-openapi.yml
- filename: doctofam-com-procedures-api-openapi.yml
  format: yaml
  label: Doctofam Procedures API
  slug: doctofam-com-procedures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-procedures-api-openapi.yml
- filename: doctofam-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Doctofam Webhook subscriptions API
  slug: doctofam-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doctofam-com/openapi/doctofam-com-webhook-subscriptions-api-openapi.yml
consequence_counts:
  physical: 2
  read: 13
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Doctofam Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments
operation_count: 21
overview: 'Doctofam exposes 21 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Doctofam
provider_slug: doctofam-com
slug: doctofam-com-agentic-access
source_filename: doctofam-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/doctofam-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 13\n    acting: 8\n  by_consequence:\n    read: 13\n    write: 6\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/appointments\n  method: get\n  operationId: getApiAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/appointments\n  method: post\n  operationId: postApiAppointments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appointments/{appointmentId}\n  method: get\n  operationId: getApiAppointmentsAppointmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/clinics\n  method: get\n  operationId: getApiClinics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/clinics/{clinicId}\n  method: get\n  operationId: getApiClinicsClinicId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices\n  method: get\n  operationId: getApiInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/invoices\n  method: post\n  operationId: postApiInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoices/{invoiceId}\n  method: get\n  operationId: getApiInvoicesInvoiceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/patients\n  method: get\n  operationId: getApiPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/patients\n  method: post\n  operationId: postApiPatients\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/patients/{patientId}\n  method: get\n  operationId: getApiPatientsPatientId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments\n  method: get\n  operationId: getApiPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments\n  method: post\n  operationId: postApiPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{paymentId}\n  method: get\n  operationId: getApiPaymentsPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/procedures\n  method: get\n  operationId: getApiProcedures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/procedures\n  method: post\n  operationId: postApiProcedures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/procedures/{procedureId}\n  method: get\n  operationId: getApiProceduresProcedureId\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooksubscriptions\n  method: get\n  operationId: getApiWebhooksubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooksubscriptions\n  method: post\n  operationId: postApiWebhooksubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooksubscriptions/{webhookSubscriptionId}\n  method: put\n  operationId: putApiWebhooksubscriptionsWebhookSubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooksubscriptions/{webhookSubscriptionId}\n  method: delete\n  operationId: deleteApiWebhooksubscriptionsWebhookSubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/doctofam-com/agentic-access/doctofam-com-agentic-access.yml
summary_line: 21 operations · 8 acting
tags:
- Medical Practice Management
- Appointment Scheduling
- Billing and Insurance
---
