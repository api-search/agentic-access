---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: rest
  format: yaml
  label: Google Analytics Data API
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://analyticsdata.googleapis.com/$discovery/rest?version=v1beta
- filename: rest
  format: yaml
  label: Google Analytics Admin API
  slug: google-analytics-admin-api
  spec_type: OpenAPI
  url: https://analyticsadmin.googleapis.com/$discovery/rest?version=v1beta
consequence_counts:
  read: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Analytics 4 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Google Analytics 4 exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Analytics 4
provider_slug: google-analytics-4
slug: google-analytics-4-agentic-access
source_filename: google-analytics-4-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-analytics-4-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 6\n    connected: 2\n  by_consequence:\n    write: 6\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1beta/{property}:runReport\n  method: post\n  operationId: runReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - analytics\n    - analytics.readonly\n- path: /v1beta/{property}:runPivotReport\n  method:\
  \ post\n  operationId: runPivotReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - analytics\n    - analytics.readonly\n- path: /v1beta/{property}:batchRunReports\n  method: post\n  operationId: batchRunReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - analytics\n    - analytics.readonly\n- path: /v1beta/{property}:batchRunPivotReports\n  method: post\n  operationId: batchRunPivotReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - analytics\n    - analytics.readonly\n- path: /v1beta/{property}:runRealtimeReport\n  method: post\n  operationId: runRealtimeReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - analytics\n    - analytics.readonly\n- path: /v1beta/{name}/metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - analytics\n    - analytics.readonly\n- path: /v1beta/{parent}/audienceExports\n  method: post\n  operationId:\
  \ createAudienceExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - analytics\n    - analytics.readonly\n- path: /v1beta/{name}\n  method: get\n  operationId: getAudienceExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - analytics\n    - analytics.readonly\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/agentic-access/google-analytics-4-agentic-access.yml
summary_line: 8 operations · 6 acting
tags:
- Analytics
- Data Collection
- Marketing
- Measurement
- Mobile Analytics
- Reporting
- Web Analytics
---
