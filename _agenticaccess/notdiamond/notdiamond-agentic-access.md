---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: notdiamond-openapi.yml
  format: yaml
  label: Not Diamond Model Select API
  slug: notdiamond-model-select-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/openapi/notdiamond-openapi.yml
- filename: notdiamond-openapi.yml
  format: yaml
  label: Not Diamond Models API
  slug: notdiamond-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/openapi/notdiamond-openapi.yml
- filename: notdiamond-openapi.yml
  format: yaml
  label: Not Diamond Feedback API
  slug: notdiamond-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/openapi/notdiamond-openapi.yml
- filename: notdiamond-openapi.yml
  format: yaml
  label: Not Diamond Custom Routers API
  slug: notdiamond-custom-routers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/openapi/notdiamond-openapi.yml
consequence_counts:
  read: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Notdiamond Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Not Diamond exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Not Diamond
provider_slug: notdiamond
slug: notdiamond-agentic-access
source_filename: notdiamond-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/notdiamond-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 5\n    connected: 1\n  by_consequence:\n    write: 5\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /modelRouter/modelSelect\n  method: post\n  operationId: modelSelect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/metrics/feedback\n  method: post\n  operationId: reportFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /report/metrics/latency\n  method: post\n  operationId: reportLatency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pzn/trainCustomRouter\n  method: post\n  operationId: trainCustomRouter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /preferences/userPreferenceCreate\n  method: post\n  operationId: createUserPreference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/agentic-access/notdiamond-agentic-access.yml
summary_line: 6 operations · 5 acting
tags:
- AI
- LLM
- Model Routing
- Router
- Orchestration
---
