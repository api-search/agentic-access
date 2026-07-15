---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 11
api_specs:
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Authentication API
  slug: heidi-api-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Templates API
  slug: heidi-api-templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Patient Profiles API
  slug: heidi-api-patient-profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Sessions API
  slug: heidi-api-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Session Context API
  slug: heidi-api-session-context
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Session Coding API
  slug: heidi-api-session-coding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Transcription API
  slug: heidi-api-transcription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Consult Notes API
  slug: heidi-api-consult-notes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Documents API
  slug: heidi-api-documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
- filename: heidi-health-openapi.yml
  format: yaml
  label: Heidi Ask Heidi API
  slug: heidi-api-ask-heidi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/openapi/heidi-health-openapi.yml
consequence_counts:
  read: 11
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Heidi Health Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Heidi Health exposes 24 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Heidi Health
provider_slug: heidi-health
slug: heidi-health-agentic-access
source_filename: heidi-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/heidi-health-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 11\n    acting: 13\n  by_consequence:\n    read: 11\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /jwt\n  method: get\n  operationId: getJwt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/document-templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient-profiles\n  method:\
  \ post\n  operationId: createPatientProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient-profiles\n  method: get\n  operationId: listPatientProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient-profiles/{patient_profile_id}\n  method: get\n  operationId: getPatientProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patient-profiles/{patient_profile_id}\n  method: patch\n  operationId: updatePatientProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient-profiles:batch-delete\n  method: post\n  operationId: batchDeletePatientProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patient-profiles/{patient_profile_id}/sessions\n  method: post\n  operationId: linkSessionToPatientProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: post\n  operationId: createSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}\n  method: patch\n  operationId: updateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/linked-user\n  method: get\n  operationId: listLinkedUserSessions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/context-documents\n  method: post\n  operationId: uploadContextDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/context-documents\n  method: get\n  operationId: listContextDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/context-documents\n  method: delete\n  operationId: deleteContextDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/upload-audio\n  method: post\n  operationId: uploadSessionAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/transcript\n  method: get\n  operationId: getSessionTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/transcript/live\n  method: get\n  operationId: getLiveSessionTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/consult-note\n\
  \  method: post\n  operationId: generateConsultNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/client-customised-template/response\n  method: post\n  operationId: generateCustomTemplateConsultNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/documents\n  method: post\n  operationId: generateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/documents\n  method: get\n  operationId: listSessionDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/clinical-codes\n  method: get\n  operationId: getSessionClinicalCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/ask-ai\n  method: post\n  operationId: askHeidi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heidi-health/refs/heads/main/agentic-access/heidi-health-agentic-access.yml
summary_line: 24 operations · 13 acting
tags:
- Healthcare
- Health Tech
- AI Medical Scribe
- Ambient AI
- Clinical Documentation
- Clinical Decision Support
- Artificial Intelligence
- Speech To Text
- Transcription
- EHR Integration
- Electronic Health Records
- Telehealth
- Clinical Coding
- ICD-10
- SNOMED
- HIPAA
- GDPR
- SOC 2
- ISO 27001
- ISO 42001
- Wearables
- Voice
- Audio
- Australia
- Melbourne
---
