---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 8
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Meet API
  slug: google-meet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-meet/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 8
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Meet Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Google Meet exposes 11 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Meet
provider_slug: google-meet
slug: google-meet-agentic-access
source_filename: google-meet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 3\n    connected: 8\n  by_consequence:\n    write: 3\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/spaces\n  method: post\n  operationId: createSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{name}\n  method: get\n  operationId: getSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{name}\n  method: patch\n  operationId: updateSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{name}:endActiveConference\n  method: post\n  operationId: endActiveConference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conferenceRecords\n  method: get\n  operationId: listConferenceRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/conferenceRecords/{conferenceRecordId}\n  method: get\n  operationId: getConferenceRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conferenceRecords/{conferenceRecordId}/participants\n  method: get\n  operationId: listParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conferenceRecords/{conferenceRecordId}/participants/{participantId}\n  method: get\n  operationId: getParticipant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conferenceRecords/{conferenceRecordId}/recordings\n  method: get\n  operationId: listRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v2/conferenceRecords/{conferenceRecordId}/transcripts\n  method: get\n  operationId: listTranscripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conferenceRecords/{conferenceRecordId}/transcripts/{transcriptId}/entries\n  method: get\n  operationId: listTranscriptEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-meet/refs/heads/main/agentic-access/google-meet-agentic-access.yml
summary_line: 11 operations · 3 acting
tags:
- Google
- Google Workspace
- Meetings
- Recordings
- Transcripts
- Video Conferencing
---
