---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 5
api_specs:
- filename: rest
  format: yaml
  label: Gmail API
  slug: gmail-api
  spec_type: OpenAPI
  url: https://gmail.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Calendar API
  slug: google-calendar-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/calendar/v3/rest
- filename: rest
  format: yaml
  label: Google Drive API
  slug: google-drive-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/drive/v3/rest
- filename: rest
  format: yaml
  label: Google Docs API
  slug: google-docs-api
  spec_type: OpenAPI
  url: https://docs.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Sheets API
  slug: google-sheets-api
  spec_type: OpenAPI
  url: https://sheets.googleapis.com/$discovery/rest?version=v4
- filename: rest
  format: yaml
  label: Google Slides API
  slug: google-slides-api
  spec_type: OpenAPI
  url: https://slides.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Chat API
  slug: google-chat-api
  spec_type: OpenAPI
  url: https://chat.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Admin SDK
  slug: google-admin-sdk
  spec_type: OpenAPI
  url: https://admin.googleapis.com/$discovery/rest?version=directory_v1
consequence_counts:
  physical: 2
  read: 5
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Google Suite Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /gmail/v1/users/{userId}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmail/v1/users/{userId}/drafts/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmail/v1/users/{userId}/messages/send
operation_count: 11
overview: 'Google Workspace (G Suite) exposes 11 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 3 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Workspace (G Suite)
provider_slug: google-suite
slug: google-suite-agentic-access
source_filename: google-suite-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-suite-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 5\n    acting: 6\n  by_consequence:\n    read: 5\n    write: 3\n    safety-critical: 1\n    physical: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /gmail/v1/users/{userId}/profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/watch\n  method: post\n  operationId: watch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/stop\n  method: post\n  operationId: stop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/drafts\n  method: get\n  operationId: listDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/drafts\n  method: post\n  operationId: createDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/drafts/send\n  method: post\n  operationId: sendDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  \    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/messages/send\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/labels\n  method: get\n  operationId:\
  \ listLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/threads\n  method: get\n  operationId: listThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - gmail.labels\n    - gmail.modify\n    - gmail.readonly\n    - gmail.send\n- path: /gmail/v1/users/{userId}/settings/vacation\n  method: put\n  operationId: updateVacationSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - gmail.labels\n    - gmail.modify\n\
  \    - gmail.readonly\n    - gmail.send\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-suite/refs/heads/main/agentic-access/google-suite-agentic-access.yml
summary_line: 11 operations · 6 acting · 1 human-in-the-loop
tags:
- Cloud
- Collaboration
- Enterprise
- Google
- Productivity
- Workspace
---
