---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 21
api_specs:
- filename: suki-ambient-api-openapi.yml
  format: yaml
  label: Suki Ambient API
  slug: suki-ambient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-ambient-api-openapi.yml
- filename: suki-dictation-api-openapi.yml
  format: yaml
  label: Suki Dictation API
  slug: suki-dictation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-dictation-api-openapi.yml
- filename: suki-form-filling-api-openapi.yml
  format: yaml
  label: Suki Form Filling API
  slug: suki-form-filling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-form-filling-api-openapi.yml
- filename: suki-auth-api-openapi.yml
  format: yaml
  label: Suki Auth API
  slug: suki-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-auth-api-openapi.yml
- filename: suki-info-api-openapi.yml
  format: yaml
  label: Suki Info API
  slug: suki-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/openapi/suki-info-api-openapi.yml
consequence_counts:
  read: 21
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Suki Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'Suki AI exposes 36 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Suki AI
provider_slug: suki
slug: suki-agentic-access
source_filename: suki-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/suki-ambient-api-openapi.yml, openapi/suki-auth-api-openapi.yml, openapi/suki-dictation-api-openapi.yml,\n  openapi/suki-form-filling-api-openapi.yml, openapi/suki-info-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 15\n    connected: 21\n  by_consequence:\n    write: 15\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /ambient/sessions\n  method: post\n  operationId: createAmbientSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /ambient/sessions/{sessionId}/context\n  method: post\n  operationId: seedAmbientSessionContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ambient/sessions/{sessionId}/context\n  method: patch\n  operationId: updateAmbientSessionContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ambient/sessions/{sessionId}/end\n  method: post\n  operationId: endAmbientSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ambient/sessions/{sessionId}/status\n  method: get\n  operationId: getAmbientSessionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ambient/sessions/{sessionId}/content\n  method: get\n  operationId: getAmbientSessionContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ambient/sessions/{sessionId}/transcript\n  method: get\n  operationId: getAmbientSessionTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ambient/sessions/{sessionId}/recording\n  method: get\n\
  \  operationId: getAmbientSessionRecording\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ambient/sessions/{sessionId}/structured-data\n  method: get\n  operationId: getAmbientSessionStructuredData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encounters/{encounterId}/content\n  method: get\n  operationId: getEncounterContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encounters/{encounterId}/structured-data\n  method: get\n  operationId: getEncounterStructuredData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-preferences\n  method: get\n  operationId:\
  \ getUserPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-preferences\n  method: patch\n  operationId: updateUserPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feedback/ambient\n  method: post\n  operationId: submitAmbientFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/register\n  method: post\n  operationId: registerProvider\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login\n  method: post\n  operationId: loginProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/jwks\n  method: get\n  operationId: getJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dictation/sessions\n  method: post\n  operationId: createDictationSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dictation/sessions/{sessionId}/end\n  method: post\n  operationId: endDictationSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /form-filling/sessions\n  method: post\n  operationId: createFormFillingSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /form-filling/sessions/{sessionId}/context\n  method: post\n  operationId: seedFormFillingContext\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /form-filling/sessions/{sessionId}/context\n  method: patch\n  operationId: updateFormFillingContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /form-filling/sessions/{sessionId}/end\n  method: post\n  operationId: endFormFillingSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /form-filling/sessions/{sessionId}/status\n  method: get\n  operationId: getFormFillingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /form-filling/sessions/{sessionId}/structured-data\n  method: get\n  operationId: getFormFillingStructuredData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /form-filling/sessions/{sessionId}/feedback\n  method: post\n  operationId: submitFormFillingFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /form-filling/templates\n  method: get\n  operationId: listFormTemplates\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/specialties\n  method: get\n  operationId: listSpecialties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/diagnoses\n  method: get\n  operationId: listDiagnoses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/encounter-types\n  method: get\n  operationId: listEncounterTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/visit-types\n  method: get\n  operationId: listVisitTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /info/loincs\n  method: get\n  operationId: listLoincs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/provider-roles\n  method: get\n  operationId: listProviderRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/medication-orders\n  method: get\n  operationId: listMedicationOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/orders-coding-systems\n  method: get\n  operationId: listOrderCodingSystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/orders-dosage-units\n  method: get\n  operationId: listOrderDosageUnits\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suki/refs/heads/main/agentic-access/suki-agentic-access.yml
summary_line: 36 operations · 15 acting
tags:
- AI
- Artificial Intelligence
- Ambient Clinical Intelligence
- Medical Scribe
- Clinical Documentation
- Voice AI
- Speech Recognition
- Healthcare
- EHR Integration
- Epic
- Oracle Health
- athenahealth
- MEDITECH
- Dictation
- Form Filling
- Note Generation
- Generative AI
- HIPAA
- SOC2
- Healthcare Technology
---
