---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 13
api_specs:
- filename: coviu-auth-api-openapi.yml
  format: yaml
  label: Coviu Auth API
  slug: coviu-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-auth-api-openapi.yml
- filename: coviu-collections-api-openapi.yml
  format: yaml
  label: Coviu Collections API
  slug: coviu-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-collections-api-openapi.yml
- filename: coviu-participants-api-openapi.yml
  format: yaml
  label: Coviu Participants API
  slug: coviu-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-participants-api-openapi.yml
- filename: coviu-sessions-api-openapi.yml
  format: yaml
  label: Coviu Sessions API
  slug: coviu-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-sessions-api-openapi.yml
- filename: coviu-waiting-area-api-openapi.yml
  format: yaml
  label: Coviu Waiting Area API
  slug: coviu-waiting-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-waiting-area-api-openapi.yml
- filename: coviu-webhook-requests-api-openapi.yml
  format: yaml
  label: Coviu Webhook Requests API
  slug: coviu-webhook-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-webhook-requests-api-openapi.yml
consequence_counts:
  read: 13
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coviu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Coviu exposes 21 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Coviu
provider_slug: coviu
slug: coviu-agentic-access
source_filename: coviu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/coviu-rest-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 8\n    connected: 13\n  by_consequence:\n    write: 8\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/auth/token\n  method: post\n  operationId: access-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}\n  method: put\n  operationId: updateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/sessions/{session_id}\n  method: delete\n  operationId: cancelSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/summary\n  method: get\n  operationId: getSessionSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/participants\n  method: get\n  operationId: listParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/participants\n  method: post\n  operationId: addParticipant\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/participants/{participant_id}\n  method: get\n  operationId: getParticipant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/participants/{participant_id}\n  method: put\n  operationId: updateParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/participants/{participant_id}\n  method: delete\n  operationId: cancelParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/waiting/{teamId}\n  method: get\n  operationId: getCurrentlyWaitingCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/waiting/{teamId}/queue/{waitingQueueId}\n  method: get\n  operationId: getCurrentlyWaitingCallsForQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/waiting/{teamId}/calls/{callId}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections/{teamId}\n  method: get\n  operationId: getCollections\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections/{teamId}/collection/{collectionId}\n  method: get\n  operationId: listSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections/{teamId}/collection/{collectionId}/submission/{submissionId}\n  method: get\n  operationId: getSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections/{teamId}/collection/{collectionId}/submission/{submissionId}/file/{fileId}\n  method: get\n  operationId: getSubmissionFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections/{teamId}/collection/{collectionId}/recording/{submissionId}\n\
  \  method: get\n  operationId: getAudioRecording\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/agentic-access/coviu-agentic-access.yml
summary_line: 21 operations · 8 acting
tags:
- Healthcare
- Telehealth
- Australia
- Virtual Care
- Video
- WebRTC
- Appointments
- Remote Monitoring
- REST
---
