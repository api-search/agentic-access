---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: tabby-ml-openapi.yml
  format: yaml
  label: Tabby Code Completions API
  slug: tabby-ml-code-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-openapi.yml
- filename: tabby-ml-openapi.yml
  format: yaml
  label: Tabby Chat Completions API
  slug: tabby-ml-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-openapi.yml
- filename: tabby-ml-openapi.yml
  format: yaml
  label: Tabby Doc Ingestion API
  slug: tabby-ml-answer-engine-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-openapi.yml
- filename: tabby-ml-openapi.yml
  format: yaml
  label: Tabby Models API
  slug: tabby-ml-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-openapi.yml
- filename: tabby-ml-openapi.yml
  format: yaml
  label: Tabby Health API
  slug: tabby-ml-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-openapi.yml
- filename: tabby-ml-openapi.yml
  format: yaml
  label: Tabby Events API
  slug: tabby-ml-events-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/openapi/tabby-ml-openapi.yml
consequence_counts:
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tabby Ml Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Tabby exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tabby
provider_slug: tabby-ml
slug: tabby-ml-agentic-access
source_filename: tabby-ml-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tabby-ml-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 5\n    connected: 3\n  by_consequence:\n    write: 5\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/completions\n  method: post\n  operationId: completion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: chatCompletions\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/chat/completions\n  method: post\n  operationId: chatCompletionsBeta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/ingestion\n  method: post\n  operationId: ingestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/models\n  method: get\n  operationId: models\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/server_setting\n  method: get\n  operationId: serverSetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: post\n  operationId: event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabby-ml/refs/heads/main/agentic-access/tabby-ml-agentic-access.yml
summary_line: 8 operations · 5 acting
tags:
- AI Coding Assistant
- Code Completion
- Open Source
- Developer Tools
- LLM
- AI
- Self-Hosted
- Code Generation
- Copilot Alternative
---
