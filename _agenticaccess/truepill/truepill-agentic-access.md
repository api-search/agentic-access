---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Patients API
  slug: truepill-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Prescriptions & Orders API
  slug: truepill-prescriptions-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Medications & Insurance API
  slug: truepill-medications-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Shipments & Fulfillment API
  slug: truepill-shipments-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
- filename: truepill-openapi.yml
  format: yaml
  label: Truepill Webhooks API
  slug: truepill-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-openapi.yml
consequence_counts:
  physical: 3
  read: 8
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Truepill Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /direct_transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer_request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/direct_transfer
operation_count: 15
overview: 'Truepill exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 4 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Truepill
provider_slug: truepill
slug: truepill-agentic-access
source_filename: truepill-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/truepill-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 7\n    connected: 8\n  by_consequence:\n    write: 4\n    read: 8\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /patient\n  method: put\n  operationId: createPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient\n  method: get\n  operationId: findPatient\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient/{patient_token}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient/{patient_token}\n  method: post\n  operationId: updatePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient/{patient_token}/prescriptions\n  method: get\n  operationId: listPatientPrescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prescription/{prescription_token}\n  method: get\n  operationId: getPrescription\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer_request\n  method: post\n  operationId: createTransferRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer_request\n  method: get\n  operationId: listTransferRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer_request/{transfer_token}\n  method: get\n  operationId: getTransferRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /direct_transfer\n  method: post\n  operationId: createDirectTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/direct_transfer\n  method: post\n  operationId: createDirectTransferV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insurance\n  method: post\n  operationId: createInsurance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /copay_request\n  method: post\n  operationId: createCopayRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insurance_claim\n  method: get\n  operationId: getInsuranceClaim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook_events/{webhook_type}\n  method: get\n  operationId: getWebhookEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/agentic-access/truepill-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Pharmacy
- Healthcare
- Prescription Fulfillment
- Telehealth
- Diagnostics
- Insurance
---
