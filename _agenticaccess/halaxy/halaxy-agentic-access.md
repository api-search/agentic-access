---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 34
api_specs:
- filename: halaxy-appointment-api-openapi.yml
  format: yaml
  label: Halaxy Appointment API
  slug: halaxy-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-appointment-api-openapi.yml
- filename: halaxy-chargeitemdefinition-api-openapi.yml
  format: yaml
  label: Halaxy Charge Item Definition API
  slug: halaxy-chargeitemdefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-chargeitemdefinition-api-openapi.yml
- filename: halaxy-coverage-api-openapi.yml
  format: yaml
  label: Halaxy Coverage API
  slug: halaxy-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-coverage-api-openapi.yml
- filename: halaxy-invoice-api-openapi.yml
  format: yaml
  label: Halaxy Invoice API
  slug: halaxy-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-invoice-api-openapi.yml
- filename: halaxy-invoiceline-api-openapi.yml
  format: yaml
  label: Halaxy Invoice Line API
  slug: halaxy-invoiceline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-invoiceline-api-openapi.yml
- filename: halaxy-organization-api-openapi.yml
  format: yaml
  label: Halaxy Organization API
  slug: halaxy-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-organization-api-openapi.yml
- filename: halaxy-patient-api-openapi.yml
  format: yaml
  label: Halaxy Patient API
  slug: halaxy-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-patient-api-openapi.yml
- filename: halaxy-paymenttransaction-api-openapi.yml
  format: yaml
  label: Halaxy Payment Transaction API
  slug: halaxy-paymenttransaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-paymenttransaction-api-openapi.yml
- filename: halaxy-practitioner-api-openapi.yml
  format: yaml
  label: Halaxy Practitioner API
  slug: halaxy-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-practitioner-api-openapi.yml
- filename: halaxy-referral-api-openapi.yml
  format: yaml
  label: Halaxy Referral API
  slug: halaxy-referral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-referral-api-openapi.yml
- filename: halaxy-referraldefinition-api-openapi.yml
  format: yaml
  label: Halaxy Referral Definition API
  slug: halaxy-referraldefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-referraldefinition-api-openapi.yml
- filename: halaxy-schedule-api-openapi.yml
  format: yaml
  label: Halaxy Schedule API
  slug: halaxy-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-schedule-api-openapi.yml
- filename: halaxy-slot-api-openapi.yml
  format: yaml
  label: Halaxy Slot API
  slug: halaxy-slot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-slot-api-openapi.yml
- filename: halaxy-capability-statement-api-openapi.yml
  format: yaml
  label: Halaxy Capability Statement API
  slug: halaxy-capability-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-capability-statement-api-openapi.yml
- filename: halaxy-document-reference-api-openapi.yml
  format: yaml
  label: Halaxy Document Reference API
  slug: halaxy-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-document-reference-api-openapi.yml
- filename: halaxy-healthcare-service-api-openapi.yml
  format: yaml
  label: Halaxy Healthcare Service API
  slug: halaxy-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-healthcare-service-api-openapi.yml
- filename: halaxy-practitioner-role-api-openapi.yml
  format: yaml
  label: Halaxy Practitioner Role API
  slug: halaxy-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-practitioner-role-api-openapi.yml
- filename: halaxy-search-parameter-api-openapi.yml
  format: yaml
  label: Halaxy Search Parameter API
  slug: halaxy-search-parameter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/openapi/halaxy-search-parameter-api-openapi.yml
consequence_counts:
  read: 34
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Halaxy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 49
overview: 'Halaxy exposes 49 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Halaxy
provider_slug: halaxy
slug: halaxy-agentic-access
source_filename: halaxy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: generated\nsource: openapi/halaxy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 34\n    acting: 15\n  by_consequence:\n    read: 34\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /main/Appointment\n  method: get\n  operationId: findAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Appointment/$book\n  method: post\n  operationId: bookAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/Appointment/$find\n  method: get\n  operationId: findAvailableAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Appointment/{id}\n  method: get\n  operationId: getAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Appointment/{id}\n  method: patch\n  operationId: patchAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/ChargeItemDefinition\n  method: get\n  operationId: findChargeItemDefinitions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/ChargeItemDefinition/{id}\n  method: get\n  operationId: getChargeItemDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Coverage\n  method: get\n  operationId: findCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Coverage\n  method: post\n  operationId: createCoverage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/Coverage/{id}\n  method: get\n  operationId:\
  \ getCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Coverage/{id}\n  method: patch\n  operationId: patchCoverage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/DocumentReference\n  method: post\n  operationId: createNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/HealthcareService\n  method: get\n  operationId: findHealthcareService\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/HealthcareService/{id}\n  method: get\n  operationId: getHealthcareService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Invoice\n  method: get\n  operationId: findInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Invoice/{id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/InvoiceLine\n  method: get\n  operationId: findInvoiceLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/InvoiceLine/{id}\n\
  \  method: get\n  operationId: getInvoiceLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Organization\n  method: get\n  operationId: findOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Organization\n  method: post\n  operationId: createOrganisation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/Organization/{id}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /main/Patient\n  method: get\n  operationId: findPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Patient\n  method: post\n  operationId: createPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/Patient/$export-ids\n  method: get\n  operationId: getPatientIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Patient/{id}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /main/Patient/{id}\n  method: patch\n  operationId: patchPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/Patient/{id}\n  method: put\n  operationId: updatePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/PaymentTransaction\n  method: get\n  operationId: findPaymentTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/PaymentTransaction/{id}\n  method: get\n  operationId: getPaymentTransaction\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Practitioner\n  method: get\n  operationId: findPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Practitioner\n  method: post\n  operationId: createPractitioner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/Practitioner/{id}\n  method: get\n  operationId: getPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/PractitionerRole\n  method: get\n \
  \ operationId: findPractitionerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/PractitionerRole\n  method: post\n  operationId: createPractitionerRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/PractitionerRole/{id}\n  method: get\n  operationId: getPractitionerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Referral\n  method: get\n  operationId: findReferral\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /main/Referral\n  method: post\n  operationId: createReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/Referral/{id}\n  method: get\n  operationId: getReferral\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Referral/{id}\n  method: patch\n  operationId: patchReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/ReferralDefinition\n  method: get\n  operationId: findReferralDefinition\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/ReferralDefinition/{id}\n  method: get\n  operationId: getReferralDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Schedule\n  method: get\n  operationId: findSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Schedule\n  method: post\n  operationId: createSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/Schedule/{id}\n  method: get\n  operationId:\
  \ getSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Schedule/{id}/$generate\n  method: post\n  operationId: generateScheduleSlots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /main/SearchParameter\n  method: get\n  operationId: findSearchParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Slot\n  method: get\n  operationId: findSlots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/Slot/{id}\n  method:\
  \ get\n  operationId: getSlot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main/metadata\n  method: get\n  operationId: api_metadata_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halaxy/refs/heads/main/agentic-access/halaxy-agentic-access.yml
summary_line: 49 operations · 15 acting
tags:
- Company
- Healthcare
- Practice Management
- FHIR
- Telehealth
- Appointments
- Billing
- Patients
---
