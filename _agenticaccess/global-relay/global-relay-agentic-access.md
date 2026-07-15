---
acting_count: 8
action_class_counts:
  acting: 8
api_specs:
- filename: global-relay-conversation-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Conversation Archiving API
  slug: conversation-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-conversation-archiving-api-openapi.yml
- filename: global-relay-email-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Email Archiving API
  slug: email-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-email-archiving-api-openapi.yml
- filename: global-relay-voice-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Voice Archiving API
  slug: voice-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-voice-archiving-api-openapi.yml
- filename: global-relay-event-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Event Archiving API
  slug: event-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-event-archiving-api-openapi.yml
consequence_counts:
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Global Relay Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Global Relay exposes 8 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Global Relay
provider_slug: global-relay
slug: global-relay-agentic-access
source_filename: global-relay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/global-relay-conversation-archiving-api-openapi.yml, openapi/global-relay-email-archiving-api-openapi.yml,\n  openapi/global-relay-event-archiving-api-openapi.yml, openapi/global-relay-voice-archiving-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 8\n  by_consequence:\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /conversations\n  method: post\n  operationId: archiveConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email\n  method: post\n  operationId: archiveEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: post\n  operationId: uploadEmailAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: post\n  operationId: archiveEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: post\n  operationId: uploadEventFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voice\n  method: post\n  operationId: archiveVoiceRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: post\n  operationId: uploadVoiceFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/agentic-access/global-relay-agentic-access.yml
summary_line: 8 operations · 8 acting
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
---
