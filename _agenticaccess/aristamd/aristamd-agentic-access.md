---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 21
api_specs:
- filename: aristamd-comments-api-openapi.yml
  format: yaml
  label: AristaMD Comments API
  slug: aristamd-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-comments-api-openapi.yml
- filename: aristamd-diagnostic-api-openapi.yml
  format: yaml
  label: AristaMD Diagnostic API
  slug: aristamd-diagnostic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-diagnostic-api-openapi.yml
- filename: aristamd-econsults-api-openapi.yml
  format: yaml
  label: AristaMD E Consults API
  slug: aristamd-econsults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-econsults-api-openapi.yml
- filename: aristamd-intergy-patients-api-openapi.yml
  format: yaml
  label: AristaMD Intergy/Patients API
  slug: aristamd-intergy-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-intergy-patients-api-openapi.yml
- filename: aristamd-panelists-api-openapi.yml
  format: yaml
  label: AristaMD Panelists API
  slug: aristamd-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-panelists-api-openapi.yml
- filename: aristamd-patients-api-openapi.yml
  format: yaml
  label: AristaMD Patients API
  slug: aristamd-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-patients-api-openapi.yml
- filename: aristamd-requests-api-openapi.yml
  format: yaml
  label: AristaMD Requests API
  slug: aristamd-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-requests-api-openapi.yml
- filename: aristamd-reviews-api-openapi.yml
  format: yaml
  label: AristaMD Reviews API
  slug: aristamd-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-reviews-api-openapi.yml
- filename: aristamd-specialties-api-openapi.yml
  format: yaml
  label: AristaMD Specialties API
  slug: aristamd-specialties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-specialties-api-openapi.yml
- filename: aristamd-specialty-api-openapi.yml
  format: yaml
  label: AristaMD Specialty API
  slug: aristamd-specialty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-specialty-api-openapi.yml
- filename: aristamd-users-api-openapi.yml
  format: yaml
  label: AristaMD Users API
  slug: aristamd-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-users-api-openapi.yml
- filename: aristamd-workup-checklists-api-openapi.yml
  format: yaml
  label: AristaMD Workup Checklists API
  slug: aristamd-workup-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-workup-checklists-api-openapi.yml
consequence_counts:
  read: 21
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aristamd Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'AristaMD exposes 42 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AristaMD
provider_slug: aristamd
slug: aristamd-agentic-access
source_filename: aristamd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/aristamd-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 21\n    connected: 21\n  by_consequence:\n    write: 21\n    read: 21\n  human_in_the_loop_required: 0\nx-apievangelist-review:\n  # The per-operation contracts below are the UNMODIFIED mechanical output of\n  # derive-agentic-access.py. This block records where the generic heuristic is\n  # under-calibrated for this specific API. It does not override the generated\n  # classifications; it tells a reviewer what to change before deploying them.\n  reviewed: '2026-08-06'\n  domain: clinical / US protected health information\n  findings:\n  - id: consequence-underrated\n \
  \   detail: >-\n      The heuristic classifies all 21 writes as consequence \"write\" because none\n      matches its payment/order/transfer or control/stop/dispatch keyword sets.\n      In this API a write creates or alters a clinical record — a patient, an\n      eConsult, a specialist recommendation, a state transition on a care\n      episode. For a healthcare deployment these warrant a consequence tier at\n      least equivalent to \"physical\", not the default write tier.\n    affects: [POST /econsults, POST /patients, POST /HL7/messages,\n      'PUT /econsults/{econsultId}', 'PATCH /econsults/{econsultId}',\n      'DELETE /econsults/{econsultId}', 'POST /econsults/{eConsultId}/events',\n      'PUT /patients/{patientId}', 'PATCH /patients/{patientId}',\n      'DELETE /diagnostics/{diagnosticId}',\n      'POST /{request}/{requestId}/diagnostics/{diagnosticId}/events']\n  - id: human-in-the-loop-zero\n    detail: >-\n      human_in_the_loop_required is 0. For clinical record creation\
  \ and care-state\n      transitions the correct value is \"required\", not the \"conditional\" the\n      heuristic assigned. Ten operations should be raised before any agent is\n      pointed at this API.\n  - id: reads-are-phi\n    detail: >-\n      Nine of the 21 read operations return protected health information\n      (patients, patient history, patient identifiers, top-referral patients,\n      Intergy passthrough, and any eConsult read, which embeds the patient). The\n      heuristic treats reads as low-consequence \"connected\"; here a read is a PHI\n      disclosure and needs audit and purpose-binding on a par with a write.\n    affects: [GET /patients, 'GET /patients/{patientId}', GET /patients/search,\n      'GET /patients/{patientId}/history', 'GET /patients/{patientId}/identifiers',\n      'GET /patients/top-patients/{length}', 'GET /intergy/patients/{id}',\n      GET /econsults, 'GET /econsults/{econsultId}']\n  - id: no-idempotency-backstop\n    detail: >-\n      The API\
  \ publishes no idempotency key, so an agent retry on any acting\n      operation can duplicate a clinical record. Any deployment must supply\n      idempotency at the gateway; the API will not supply it.\n  - id: audience-unbound\n    detail: >-\n      `audience` is null on every operation, as designed. It must be bound per\n      deployment before these contracts mean anything.\n  disposition: >-\n    Treat this file as a starting point that needs clinical review, not as a\n    ready-to-apply policy. It is an API Evangelist artifact, not an AristaMD one.\noperations:\n- path: /comments\n  method: post\n  operationId: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /diagnostics/{diagnosticId}\n  method: delete\n  operationId: destroy\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{request}/{requestId}/diagnostics/{diagnosticId}/events\n  method: post\n  operationId: events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /econsults\n  method: get\n  operationId: index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /econsults\n  method: post\n  operationId: store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /econsults/{econsultId}\n  method: get\n  operationId: show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /econsults/{econsultId}\n  method: put\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /econsults/{econsultId}\n  method: delete\n  operationId: destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /econsults/{econsultId}\n  method: patch\n  operationId: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /econsults/{econsultId}/assign-to-me\n  method: patch\n  operationId: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /econsults/search\n  method: get\n  operationId: searchByStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /econsults/logAvailability\n  method: post\n  operationId: LogPanelistAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /econsults/{eConsultId}/events\n  method: post\n  operationId: events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /econsults/{eConsultId}/heartbeat\n  method: post\n  operationId: events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /HL7/messages\n  method: post\n  operationId: store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intergy/patients/{id}\n  method: get\n  operationId: index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /panelists\n  method: get\n  operationId: index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /panelists/getNextAvailable/{code}/{patient_id}\n  method: get\n  operationId: index\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients\n  method: get\n  operationId: index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients\n  method: post\n  operationId: store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{patientId}\n  method: get\n  operationId: show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientId}\n  method: put\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/{patientId}\n  method: patch\n  operationId: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patients/search\n  method: get\n  operationId: show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/top-patients/{length}\n  method: get\n  operationId: getTopReferralPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientId}/history\n\
  \  method: get\n  operationId: history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patients/{patientId}/identifiers\n  method: get\n  operationId: identifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews\n  method: post\n  operationId: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reviews/{id}\n  method: get\n  operationId:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews/{id}\n  method: put\n  operationId: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /specialties/{specialtyId}\n  method: get\n  operationId: show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /specialties/{specialtyId}\n  method: put\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /specialties\n  method: post\n  operationId: store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /specialties/withAvailablePanelists/{filter}\n  method: get\n  operationId: index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}\n  method: get\n  operationId: show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /users/search\n  method: post\n  operationId: index\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/update\n  method: patch\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workup-checklists/specialties\n  method: get\n  operationId: specialties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workup-checklists/specialties/{specialtyCode}/chief-complaints\n\
  \  method: get\n  operationId: chiefComplaints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workup-checklists/specialties/{specialtyCode}/chief-complaints/{chiefComplaintCode}\n  method: get\n  operationId: searchBySpecialtyAndChiefComplaint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/agentic-access/aristamd-agentic-access.yml
summary_line: 42 operations · 21 acting
tags:
- Company
- Healthcare
- Digital Health
- Telehealth
- eConsult
- Specialty Care
- Referrals
- Care Coordination
- Health Plans
- Medicaid
- HL7
- Electronic Health Records
---
