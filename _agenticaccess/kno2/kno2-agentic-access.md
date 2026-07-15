---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: kno2-openapi.yml
  format: yaml
  label: Kno2 Messaging API
  slug: kno2-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-openapi.yml
- filename: kno2-openapi.yml
  format: yaml
  label: Kno2 Intake and Retrieval API
  slug: kno2-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-openapi.yml
- filename: kno2-openapi.yml
  format: yaml
  label: Kno2 Directory API
  slug: kno2-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kno2 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/messages/{id}/send
operation_count: 12
overview: 'Kno2 exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kno2
provider_slug: kno2
slug: kno2-agentic-access
source_filename: kno2-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kno2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 7\n    connected: 5\n  by_consequence:\n    write: 6\n    read: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/messages\n  method: get\n  operationId: searchMessages\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/messages\n  method: put\n  operationId: createMessageDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/messages/{id}\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/messages/{id}\n  method: put\n  operationId: updateMessageDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/messages/{id}/send\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/messages/{id}/process\n  method: post\n  operationId: processMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/messages/{id}/attachments/{attachmentId}\n  method: get\n  operationId: getAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /api/messages/{id}/attachments/{attachmentId}\n  method: post\n  operationId: uploadAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/messages/{id}/attachments/{attachmentId}/read\n  method: put\n  operationId: markAttachmentRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documenttypes\n  method: get\n  operationId: listDocumentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/directory/validate\n  method: get\n  operationId: validateAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/agentic-access/kno2-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Healthcare Interoperability
- Clinical Records
- Health Information Exchange
- Direct Secure Messaging
- FHIR
- Clinical Documents
- Patient Records
- Healthcare
- HIE
- Care Coordination
- QHIN
- TEFCA
- Carequality
---
