---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 3
api_specs:
- filename: viewpoints-ai-study-openapi.json
  format: json
  label: Viewpoints Study API
  slug: viewpoints-study-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viewpoints-ai/refs/heads/main/openapi/viewpoints-ai-study-openapi.json
consequence_counts:
  read: 3
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Viewpoints Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Viewpoints AI exposes 7 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Viewpoints AI
provider_slug: viewpoints-ai
slug: viewpoints-ai-agentic-access
source_filename: viewpoints-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/viewpoints-ai-study-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 4\n    connected: 3\n  by_consequence:\n    write: 4\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/studies\n  method: post\n  operationId: post__v1_studies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/studies/jobs/{job_id}\n  method: get\n  operationId: get__v1_studies_jobs_{job_id}\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/studies/uploads/presigned-url\n  method: post\n  operationId: post__v1_studies_uploads_presigned-url\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/studies/{id}\n  method: get\n  operationId: get__v1_studies_{id}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/studies/{id}\n  method: put\n  operationId: put__v1_studies_{id}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/study-schedules/{schedule_id}\n  method: get\n  operationId: get__v1_study-schedules_{schedule_id}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/study-schedules/{study_id}\n  method: put\n  operationId: put__v1_study-schedules_{study_id}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viewpoints-ai/refs/heads/main/agentic-access/viewpoints-ai-agentic-access.yml
summary_line: 7 operations · 4 acting
tags:
- Company
- Ai
- Market Research
- Synthetic Personas
- Consumer Insights
- Litigation
- Jury Simulation
- Research
---
