---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 26
api_specs:
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Clients API
  slug: provet-cloud-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Patients API
  slug: provet-cloud-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Appointments API
  slug: provet-cloud-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Consultations API
  slug: provet-cloud-consultations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Billing & Invoicing API
  slug: provet-cloud-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Items & Reference Data API
  slug: provet-cloud-items-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Webhooks API
  slug: provet-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
consequence_counts:
  physical: 7
  read: 26
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Provet Cloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /appointment/{id}/send_appointment_confirmation/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /consultation/{id}/consultationdischargeinstruction/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice/{id}/full_refund/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice/{id}/partial_refund/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoicepayment/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoicepayment/{id}/cancel_payment/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /unallocatedpayment/
operation_count: 55
overview: 'Provet Cloud exposes 55 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 22 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Provet Cloud
provider_slug: provet-cloud
slug: provet-cloud-agentic-access
source_filename: provet-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/provet-cloud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    connected: 26\n    acting: 29\n  by_consequence:\n    read: 26\n    write: 22\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /client/\n  method: get\n  operationId: listClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/\n  method: post\n  operationId: createClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{id}/\n  method: patch\n  operationId: updateClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{id}/custom_field_values/\n  method: get\n  operationId: getClientCustomFieldValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{id}/custom_field_values/\n  method: post\n  operationId: setClientCustomFieldValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /phonenumber/\n  method: get\n  operationId: listPhoneNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonenumber/\n  method: post\n  operationId: createPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient/\n  method: get\n  operationId: listPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient/\n  method: post\n  operationId: createPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient/bulk/\n  method: post\n  operationId: bulkCreatePatients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient/{id}/\n  method: patch\n  operationId: updatePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient/{id}/custom_field_values/\n  method: get\n  operationId: getPatientCustomFieldValues\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient/{id}/custom_field_values/\n  method: post\n  operationId: setPatientCustomFieldValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointment/\n  method: post\n  operationId: createAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointment/{id}/send_appointment_confirmation/\n  method: post\n  operationId: sendAppointmentConfirmation\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointment_reminder/\n  method: post\n  operationId: createAppointmentReminder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onlinebookingclient/\n  method: post\n  operationId: createOnlineBookingClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /onlinebookingpatient/\n  method: post\n  operationId: createOnlineBookingPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/\n  method: get\n  operationId: listConsultations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consultation/\n  method: post\n  operationId: createConsultation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/{id}/\n  method: get\n\
  \  operationId: getConsultation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consultation/{id}/update_status/\n  method: post\n  operationId: updateConsultationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/{id}/mark_sent/\n  method: post\n  operationId: markConsultationSent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/{id}/medicines/\n  method: get\n  operationId: listConsultationMedicines\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consultation/{id}/medicines/\n  method: post\n  operationId: addConsultationMedicine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/{id}/procedures/\n  method: get\n  operationId: listConsultationProcedures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consultation/{id}/procedures/\n  method: post\n  operationId: addConsultationProcedure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/{id}/supplies/\n  method: get\n  operationId: listConsultationSupplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consultation/{id}/supplies/\n  method: post\n  operationId: addConsultationSupply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/{id}/foods/\n  method: get\n  operationId: listConsultationFoods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consultation/{id}/foods/\n\
  \  method: post\n  operationId: addConsultationFood\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/{id}/consultationdiagnosis/\n  method: post\n  operationId: addConsultationDiagnosis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/{id}/consultationnote/\n  method: post\n  operationId: addConsultationNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultation/{id}/consultationdischargeinstruction/\n  method: post\n  operationId: addConsultationDischargeInstruction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consultationitem/\n  method: get\n  operationId: listConsultationItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice/\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice/{id}/full_refund/\n\
  \  method: post\n  operationId: fullRefundInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice/{id}/partial_refund/\n  method: post\n  operationId: partialRefundInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoicerow/\n  method: get\n  operationId: listInvoiceRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /invoicerow/{id}/\n  method: get\n  operationId: getInvoiceRow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoicepayment/\n  method: get\n  operationId: listInvoicePayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoicepayment/\n  method: post\n  operationId: createInvoicePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoicepayment/{id}/cancel_payment/\n  method: post\n  operationId: cancelInvoicePayment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unallocatedpayment/\n  method: get\n  operationId: listUnallocatedPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unallocatedpayment/\n  method: post\n  operationId: createUnallocatedPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /item/\n  method: get\n  operationId: listItems\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /department/{id}/\n  method: get\n  operationId: getDepartment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reason/{id}/\n  method: get\n  operationId: getReason\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{id}/\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_fields/\n  method: get\n  operationId: listCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /codelist/species/\n  method: get\n  operationId: listSpeciesCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codelist/breeds/\n  method: get\n  operationId: listBreedCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codelist/diagnoses/\n  method: get\n  operationId: listDiagnosisCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/agentic-access/provet-cloud-agentic-access.yml
summary_line: 55 operations · 29 acting
tags:
- Veterinary
- Practice Management
- PIMS
- Healthcare
- Nordhealth
- Animal Health
- Appointments
- Billing
---
