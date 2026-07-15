---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 11
api_specs:
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Patients API
  slug: dosespot-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Prescriptions API
  slug: dosespot-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Medications API
  slug: dosespot-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Pharmacies API
  slug: dosespot-pharmacies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Prescribers API
  slug: dosespot-prescribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Notifications API
  slug: dosespot-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
consequence_counts:
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dosespot Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'DoseSpot exposes 17 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DoseSpot
provider_slug: dosespot
slug: dosespot-agentic-access
source_filename: dosespot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dosespot-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 11\n    acting: 6\n  by_consequence:\n    read: 11\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /patients\n  method: get\n  operationId: searchPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients\n  method: post\n  operationId: createPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{patientId}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientId}\n  method: post\n  operationId: updatePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{patientId}/prescriptions\n  method: get\n  operationId: getPatientPrescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientId}/prescriptions\n  method: post\n  operationId: createPatientPrescription\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{patientId}/prescriptions/{prescriptionId}\n  method: get\n  operationId: getPatientPrescription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientId}/medicationHistory\n  method: get\n  operationId: getMedicationHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /medications/search\n  method: get\n  operationId: searchMedications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /medications/interactions\n  method: post\n  operationId: checkMedicationInteractions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pharmacies/search\n  method: get\n  operationId: searchPharmacies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientId}/pharmacies\n  method: get\n  operationId: getPatientPharmacies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientId}/pharmacies\n  method: post\n  operationId: addPatientPharmacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clinicians\n  method: get\n  operationId: searchClinicians\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clinicians\n  method: post\n  operationId: createClinician\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clinicians/{clinicianId}\n  method: get\n  operationId: getClinician\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /notifications/counts\n  method: get\n  operationId: getNotificationCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/agentic-access/dosespot-agentic-access.yml
summary_line: 17 operations · 6 acting
tags:
- e-Prescribing
- eRx
- Healthcare
- EHR
- Pharmacy
- EPCS
---
