---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: coala-life-patientsessions-api-openapi.yml
  format: yaml
  label: Coala Life Patient Sessions API
  slug: coala-life-patientsessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/openapi/coala-life-patientsessions-api-openapi.yml
- filename: coala-life-platform-api-api-openapi.yml
  format: yaml
  label: Coala Life Platform.Api API
  slug: coala-life-platform-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/openapi/coala-life-platform-api-api-openapi.yml
- filename: coala-life-sessions-api-openapi.yml
  format: yaml
  label: Coala Life Sessions API
  slug: coala-life-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/openapi/coala-life-sessions-api-openapi.yml
consequence_counts:
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coala Life Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Coala Life exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Coala Life
provider_slug: coala-life
slug: coala-life-agentic-access
source_filename: coala-life-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/coala-life-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 3\n    acting: 1\n  by_consequence:\n    read: 3\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/patients/{patientId}/sessions\n  method: get\n  operationId: ListPatientSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: 'HTTP: GET /health'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sessions/{sessionId}\n\
  \  method: get\n  operationId: GetSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sessions/{sessionId}/tags/{tag}\n  method: put\n  operationId: AddSessionTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coala-life/refs/heads/main/agentic-access/coala-life-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Company
- Healthcare
- Cardiology
- Remote Monitoring
- Digital Health
---
