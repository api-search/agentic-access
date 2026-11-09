---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: arpi-ai-authentication-api-openapi.yml
  format: yaml
  label: ARPI Inc. Authentication API
  slug: arpi-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arpi-ai/openapi/arpi-ai-authentication-api-openapi.yml
- filename: arpi-ai-diag-api-openapi.yml
  format: yaml
  label: ARPI Inc. Diag API
  slug: arpi-ai-diag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arpi-ai/openapi/arpi-ai-diag-api-openapi.yml
consequence_counts:
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Arpi Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'ARPI Inc. exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ARPI Inc.
provider_slug: arpi-ai
slug: arpi-ai-agentic-access
source_filename: arpi-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/arpi-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 5\n    connected: 6\n  by_consequence:\n    write: 5\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/hospital/login\n  method: post\n  operationId: hospitalLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hospital/token\n  method: post\n  operationId: issueToken\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/diag\n  method: get\n  operationId: listMyDiags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/diag\n  method: post\n  operationId: analyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/diag/{jobId}/result\n  method: get\n  operationId: getResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/diag/{jobId}/products\n  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/diag/{jobId}/comment\n  method: get\n  operationId: getAiComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/diag/{jobId}/retry\n  method: post\n  operationId: retry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/diag/{jobId}/title\n  method: patch\n  operationId: updateMyDiagTitle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/diag/available\n  method: get\n  operationId: getMyAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/diag/usage\n  method: get\n  operationId: getMyUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/arpi-ai/agentic-access/arpi-ai-agentic-access.yml
summary_line: 11 operations · 5 acting
tags:
- Medical AI
- Healthcare
- ECG
- Diagnostics
- Artificial Intelligence
---
