---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Actions / Prompt API
  slug: klu-actions-prompt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Data / Feedback API
  slug: klu-data-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Models API
  slug: klu-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Sessions API
  slug: klu-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
- filename: klu-ai-openapi.yml
  format: yaml
  label: Klu Apps / Workspaces API
  slug: klu-apps-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/openapi/klu-ai-openapi.yml
consequence_counts:
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Klu Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Klu exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Klu
provider_slug: klu-ai
slug: klu-ai-agentic-access
source_filename: klu-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/klu-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 7\n    connected: 7\n  by_consequence:\n    write: 7\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /actions\n  method: post\n  operationId: runAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /context\n  method: post\n  operationId: createContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /context/{guid}/documents\n  method: post\n  operationId: addContextDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /context/{guid}/add_files\n  method: post\n  operationId: addContextFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/{guid}\n  method: get\n  operationId: getDataPoint\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback\n  method: post\n  operationId: createFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{guid}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{guid}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{guid}\n  method:\
  \ get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klu-ai/refs/heads/main/agentic-access/klu-ai-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- AI
- LLM
- LLM App Platform
- Prompt Engineering
- Evaluation
- Observability
---
