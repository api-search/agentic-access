---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 20
api_specs:
- filename: digitail-appointments-api-openapi.yml
  format: yaml
  label: Digitail Appointments API
  slug: digitail-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-appointments-api-openapi.yml
- filename: digitail-breeds-api-openapi.yml
  format: yaml
  label: Digitail Breeds API
  slug: digitail-breeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-breeds-api-openapi.yml
- filename: digitail-charges-api-openapi.yml
  format: yaml
  label: Digitail Charges API
  slug: digitail-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-charges-api-openapi.yml
- filename: digitail-clients-api-openapi.yml
  format: yaml
  label: Digitail Clients API
  slug: digitail-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-clients-api-openapi.yml
- filename: digitail-clinics-api-openapi.yml
  format: yaml
  label: Digitail Clinics API
  slug: digitail-clinics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-clinics-api-openapi.yml
- filename: digitail-files-api-openapi.yml
  format: yaml
  label: Digitail Files API
  slug: digitail-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-files-api-openapi.yml
- filename: digitail-invoices-api-openapi.yml
  format: yaml
  label: Digitail Invoices API
  slug: digitail-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-invoices-api-openapi.yml
- filename: digitail-labs-api-openapi.yml
  format: yaml
  label: Digitail Labs API
  slug: digitail-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-labs-api-openapi.yml
- filename: digitail-medication-api-openapi.yml
  format: yaml
  label: Digitail Medication API
  slug: digitail-medication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-medication-api-openapi.yml
- filename: digitail-pet-parents-api-openapi.yml
  format: yaml
  label: Digitail Pet Parents API
  slug: digitail-pet-parents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-pet-parents-api-openapi.yml
- filename: digitail-pets-api-openapi.yml
  format: yaml
  label: Digitail Pets API
  slug: digitail-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-pets-api-openapi.yml
- filename: digitail-prescriptions-api-openapi.yml
  format: yaml
  label: Digitail Prescriptions API
  slug: digitail-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-prescriptions-api-openapi.yml
- filename: digitail-records-api-openapi.yml
  format: yaml
  label: Digitail Records API
  slug: digitail-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-records-api-openapi.yml
- filename: digitail-reports-api-openapi.yml
  format: yaml
  label: Digitail Reports API
  slug: digitail-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-reports-api-openapi.yml
- filename: digitail-sales-api-openapi.yml
  format: yaml
  label: Digitail Sales API
  slug: digitail-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-sales-api-openapi.yml
- filename: digitail-species-api-openapi.yml
  format: yaml
  label: Digitail Species API
  slug: digitail-species-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-species-api-openapi.yml
- filename: digitail-vets-api-openapi.yml
  format: yaml
  label: Digitail Vets API
  slug: digitail-vets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-vets-api-openapi.yml
- filename: digitail-visit-types-api-openapi.yml
  format: yaml
  label: Digitail Visit Types API
  slug: digitail-visit-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-visit-types-api-openapi.yml
consequence_counts:
  read: 20
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Digitail Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Digitail exposes 21 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Digitail
provider_slug: digitail
slug: digitail-agentic-access
source_filename: digitail-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/digitail-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 20\n    acting: 1\n  by_consequence:\n    read: 20\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /pets\n  method: get\n  operationId: listPets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pets/{id}\n  method: get\n  operationId: retrievePet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments\n  method: get\n  operationId: listAppointments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/{id}\n  method: get\n  operationId: retrieveAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointment/{id}/change-status\n  method: put\n  operationId: changeAppointmentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vets/{id}\n  method: get\n  operationId: retrieveVet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clinic/{id}\n  method: get\n  operationId:\
  \ retrieveClinic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pet-parents\n  method: get\n  operationId: listPetParents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients\n  method: get\n  operationId: listClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charges\n  method: get\n  operationId: listCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /sales\n  method: get\n  operationId: listSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labs\n  method: get\n  operationId: listLabs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records\n  method: get\n  operationId: listRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prescriptions\n  method: get\n  operationId: listPrescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /medication\n  method: get\n  operationId: listMedication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /species\n  method: get\n  operationId: listSpecies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds\n  method: get\n  operationId: listBreeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visit-types\n  method: get\n  operationId: listVisitTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/agentic-access/digitail-agentic-access.yml
summary_line: 21 operations · 1 acting
tags:
- Veterinary
- PIMS
- Practice Management
- Pets
- Healthcare
- Scheduling
- Billing
- Software-as-a-Service
---
