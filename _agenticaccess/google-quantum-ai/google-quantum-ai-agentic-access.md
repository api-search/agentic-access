---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 15
api_specs:
- filename: quantum-engine-api-openapi.yml
  format: yaml
  label: Google Quantum Engine API
  slug: quantum-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/quantum-engine-api-openapi.yml
consequence_counts:
  read: 15
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Quantum Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Google Quantum AI exposes 27 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Quantum AI
provider_slug: google-quantum-ai
slug: google-quantum-ai-agentic-access
source_filename: google-quantum-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/quantum-engine-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 12\n    connected: 15\n  by_consequence:\n    write: 12\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /v1alpha1/{parent}/programs\n  method: post\n  operationId: CreateQuantumProgram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/programs\n\
  \  method: get\n  operationId: ListQuantumPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}\n  method: get\n  operationId: GetQuantumProgram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}\n  method: patch\n  operationId: UpdateQuantumProgram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}\n\
  \  method: delete\n  operationId: DeleteQuantumProgram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/jobs\n  method: post\n  operationId: CreateQuantumJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/jobs\n  method: get\n  operationId: ListQuantumJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}/job\n  method: get\n  operationId: GetQuantumJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}/job\n  method: patch\n  operationId: UpdateQuantumJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}/job\n  method: delete\n  operationId: DeleteQuantumJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}:cancel\n  method: post\n  operationId: CancelQuantumJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/result\n  method: get\n  operationId: GetQuantumResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/events\n\
  \  method: get\n  operationId: ListQuantumJobEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/processors\n  method: get\n  operationId: ListQuantumProcessors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}/processor\n  method: get\n  operationId: GetQuantumProcessor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/calibrations\n  method: get\n  operationId: ListQuantumCalibrations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}/calibration\n  method: get\n  operationId: GetQuantumCalibration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/reservations\n  method: post\n  operationId: CreateQuantumReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/reservations\n  method: get\n  operationId: ListQuantumReservations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}/reservation\n  method: get\n  operationId: GetQuantumReservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}/reservation\n  method: patch\n  operationId: UpdateQuantumReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}/reservation\n  method:\
  \ delete\n  operationId: DeleteQuantumReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}/reservation:cancel\n  method: post\n  operationId: CancelQuantumReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/timeSlots\n  method: get\n  operationId: ListQuantumTimeSlots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/reservationBudgets\n  method: get\n  operationId: ListQuantumReservationBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{parent}/reservationGrant\n  method: get\n  operationId: ListQuantumReservationGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /v1alpha1/{name}:reallocate\n  method: post\n  operationId: ReallocateQuantumReservationGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/agentic-access/google-quantum-ai-agentic-access.yml
summary_line: 27 operations · 12 acting
tags:
- Quantum Computing
- Quantum
- Hardware
- NISQ
- Error Correction
- Willow
- Sycamore
- Cirq
- Quantum Engine
- Superconducting Qubits
- Google Cloud
---
