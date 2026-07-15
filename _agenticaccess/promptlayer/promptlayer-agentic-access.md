---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 5
api_specs:
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Request Logging & Tracking API
  slug: request-logging-tracking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Prompt Registry & Templates API
  slug: prompt-registry-templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Evaluations & Datasets API
  slug: evaluations-datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
- filename: promptlayer-openapi.yml
  format: yaml
  label: PromptLayer Spans & Traces API
  slug: spans-traces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/openapi/promptlayer-openapi.yml
consequence_counts:
  read: 5
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Promptlayer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'PromptLayer exposes 16 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PromptLayer
provider_slug: promptlayer
slug: promptlayer-agentic-access
source_filename: promptlayer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/promptlayer-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 11\n    connected: 5\n  by_consequence:\n    write: 11\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /log-request\n  method: post\n  operationId: logRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/track-prompt\n  method: post\n  operationId: trackPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/track-score\n  method: post\n  operationId: trackScore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/track-metadata\n  method: post\n  operationId: trackMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompt-templates/{identifier}\n  method: post\n  operationId: getPromptTemplate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/prompt-templates\n  method: post\n  operationId: publishPromptTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluations\n  method: get\n  operationId: listEvaluations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /evaluations\n  method: post\n  operationId: createEvaluation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluations/{id}\n  method: get\n  operationId: getEvaluation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /evaluations/{id}/run\n  method: post\n  operationId: runEvaluation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluations/{id}/score\n  method: get\n  operationId: getEvaluationScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spans-bulk\n  method: post\n  operationId: createSpansBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /otlp/v1/traces\n  method: post\n  operationId: ingestOtlpTraces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /traces/{id}\n  method: get\n  operationId: getTrace\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /traces/{id}/close\n  method: post\n  operationId: closeTrace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/agentic-access/promptlayer-agentic-access.yml
summary_line: 16 operations · 11 acting
tags:
- AI
- LLM
- Prompt Engineering
- Prompt Management
- Observability
- Evaluation
---
