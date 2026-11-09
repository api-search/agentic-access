---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 9
api_specs:
- filename: dododentist-com-appointments-api-openapi.yml
  format: yaml
  label: DodoDentist Appointments API
  slug: dododentist-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-appointments-api-openapi.yml
- filename: dododentist-com-clinics-api-openapi.yml
  format: yaml
  label: DodoDentist Clinics API
  slug: dododentist-com-clinics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-clinics-api-openapi.yml
- filename: dododentist-com-invoices-api-openapi.yml
  format: yaml
  label: DodoDentist Invoices API
  slug: dododentist-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-invoices-api-openapi.yml
- filename: dododentist-com-patients-api-openapi.yml
  format: yaml
  label: DodoDentist Patients API
  slug: dododentist-com-patients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-patients-api-openapi.yml
- filename: dododentist-com-payments-api-openapi.yml
  format: yaml
  label: DodoDentist Payments API
  slug: dododentist-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-payments-api-openapi.yml
- filename: dododentist-com-treatments-api-openapi.yml
  format: yaml
  label: DodoDentist Treatments API
  slug: dododentist-com-treatments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-treatments-api-openapi.yml
- filename: dododentist-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: DodoDentist Webhook subscriptions API
  slug: dododentist-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dododentist-com/openapi/dododentist-com-webhook-subscriptions-api-openapi.yml
consequence_counts:
  read: 9
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dododentist Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'DodoDentist exposes 18 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DodoDentist
provider_slug: dododentist-com
slug: dododentist-com-agentic-access
source_filename: dododentist-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dododentist-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 9\n    acting: 9\n  by_consequence:\n    read: 9\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/appointments\n  method: get\n  operationId: getApiAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/appointments\n  method: post\n  operationId: postApiAppointments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appointments/{appointmentId}\n  method: get\n  operationId: getApiAppointmentsAppointmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/appointments/{appointmentId}\n  method: put\n  operationId: putApiAppointmentsAppointmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appointments/{appointmentId}\n  method: delete\n  operationId: deleteApiAppointmentsAppointmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/clinics\n  method: get\n  operationId: getApiClinics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices\n  method: get\n  operationId: getApiInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/patients\n  method: get\n  operationId: getApiPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/patients\n  method: post\n  operationId: postApiPatients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/patients/{patientId}\n  method: get\n  operationId: getApiPatientsPatientId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/patients/{patientId}\n  method: put\n  operationId: putApiPatientsPatientId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/patients/{patientId}\n  method: delete\n  operationId: deleteApiPatientsPatientId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments\n  method: get\n  operationId: getApiPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/treatments\n  method: get\n  operationId: getApiTreatments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooksubscriptions\n  method: get\n  operationId: getApiWebhooksubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooksubscriptions\n  method: post\n  operationId: postApiWebhooksubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooksubscriptions/{webhookSubscriptionId}\n  method: put\n  operationId: putApiWebhooksubscriptionsWebhookSubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooksubscriptions/{webhookSubscriptionId}\n  method: delete\n  operationId: deleteApiWebhooksubscriptionsWebhookSubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/dododentist-com/agentic-access/dododentist-com-agentic-access.yml
summary_line: 18 operations · 9 acting
tags:
- Dental
- Software
- Software-as-a-Service
- Practice Management
- Healthcare
---
