---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
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
  label: Admin SDK Directory API
  slug: admin-sdk-directory-api
  spec_type: OpenAPI
  url: https://admin.googleapis.com/$discovery/rest?version=directory_v1
consequence_counts:
  physical: 1
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Suites Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmail/v1/users/{userId}/messages/send
operation_count: 14
overview: 'Google Workspace APIs exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Workspace APIs
provider_slug: google-suites
slug: google-suites-agentic-access
source_filename: google-suites-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-suites-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    physical: 1\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /gmail/v1/users/{userId}/profile\n  method: get\n  operationId: gmail.users.getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gmail/v1/users/{userId}/messages\n  method: get\n  operationId: gmail.users.messages.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /gmail/v1/users/{userId}/messages/send\n  method: post\n  operationId: gmail.users.messages.send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gmail/v1/users/{userId}/labels\n  method: get\n  operationId: gmail.users.labels.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/v3/users/me/calendarList\n  method: get\n  operationId: calendar.calendarList.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/v3/calendars/{calendarId}/events\n\
  \  method: get\n  operationId: calendar.events.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/v3/calendars/{calendarId}/events\n  method: post\n  operationId: calendar.events.insert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendar/v3/calendars/{calendarId}/events/{eventId}\n  method: get\n  operationId: calendar.events.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/v3/calendars/{calendarId}/events/{eventId}\n  method: patch\n  operationId: calendar.events.patch\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendar/v3/calendars/{calendarId}/events/{eventId}\n  method: delete\n  operationId: calendar.events.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v3/files\n  method: get\n  operationId: drive.files.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v3/files\n  method: post\n  operationId: drive.files.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drive/v3/files/{fileId}\n  method: get\n  operationId: drive.files.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drive/v3/files/{fileId}\n  method: delete\n  operationId: drive.files.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-suites/refs/heads/main/agentic-access/google-suites-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Cloud Storage
- Collaboration
- Email
- Office Suite
- Productivity
---
