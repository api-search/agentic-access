---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: clearslide-insights-api-openapi.yml
  format: yaml
  label: ClearSlide Insights API
  slug: clearslide-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-insights-api-openapi.yml
- filename: clearslide-links-api-openapi.yml
  format: yaml
  label: ClearSlide Links API
  slug: clearslide-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-links-api-openapi.yml
- filename: clearslide-meetings-api-openapi.yml
  format: yaml
  label: ClearSlide Meetings API
  slug: clearslide-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-meetings-api-openapi.yml
- filename: clearslide-presentations-api-openapi.yml
  format: yaml
  label: ClearSlide Presentations API
  slug: clearslide-presentations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-presentations-api-openapi.yml
- filename: clearslide-upload-api-openapi.yml
  format: yaml
  label: ClearSlide Upload API
  slug: clearslide-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-upload-api-openapi.yml
- filename: clearslide-users-api-openapi.yml
  format: yaml
  label: ClearSlide Users API
  slug: clearslide-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/openapi/clearslide-users-api-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clearslide Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'ClearSlide exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ClearSlide
provider_slug: clearslide
slug: clearslide-agentic-access
source_filename: clearslide-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/clearslide-insights-api-openapi.yml, openapi/clearslide-links-api-openapi.yml,\n  openapi/clearslide-meetings-api-openapi.yml, openapi/clearslide-presentations-api-openapi.yml,\n  openapi/clearslide-upload-api-openapi.yml, openapi/clearslide-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /insights\n  method: get\n  operationId: getInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /links\n  method: post\n  operationId: postLinks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meeting/scheduled\n  method: get\n  operationId: getScheduledMeetings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meeting/scheduled\n  method: post\n  operationId: postScheduledMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /meeting/scheduled/{inviteMailVid}\n  method: put\n  operationId: putScheduledMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /presentations\n  method: get\n  operationId: getPresentations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upload\n  method: post\n  operationId: postUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /upload/{uploadID}\n  method: get\n  operationId: getUploadStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearslide/refs/heads/main/agentic-access/clearslide-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Company
- Sales Engagement
- Sales Enablement
- Content Management
- Presentations
- Analytics
- Meetings
- CRM
- Authentication
- SCIM
---
