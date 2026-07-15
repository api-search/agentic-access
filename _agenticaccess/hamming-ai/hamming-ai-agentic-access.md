---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 5
api_specs:
- filename: hamming-ai-openapi.yml
  format: yaml
  label: Hamming Experiments & Test Runs API
  slug: experiments-test-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-openapi.yml
- filename: hamming-ai-openapi.yml
  format: yaml
  label: Hamming Voice & Call Testing API
  slug: voice-call-testing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-openapi.yml
- filename: hamming-ai-openapi.yml
  format: yaml
  label: Hamming Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-openapi.yml
- filename: hamming-ai-openapi.yml
  format: yaml
  label: Hamming Scorers & Evaluations API
  slug: scorers-evaluations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-openapi.yml
- filename: hamming-ai-openapi.yml
  format: yaml
  label: Hamming Monitoring & Tracing API
  slug: monitoring-tracing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-openapi.yml
- filename: hamming-ai-openapi.yml
  format: yaml
  label: Hamming Prompt Optimizer & Registry API
  slug: prompts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-openapi.yml
consequence_counts:
  read: 5
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hamming Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Hamming AI exposes 16 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hamming AI
provider_slug: hamming-ai
slug: hamming-ai-agentic-access
source_filename: hamming-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hamming-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 11\n    connected: 5\n  by_consequence:\n    write: 11\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /experiments\n  method: post\n  operationId: createExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /experiments/{experimentId}\n  method: patch\n  operationId: updateExperiment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /experiments/{experimentId}/items\n  method: post\n  operationId: startExperimentItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /experiments/{experimentId}/items/{itemId}\n  method: patch\n  operationId: endExperimentItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /voice-agent/{agentId}/run\n  method: post\n  operationId: runVoiceAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voice-experiment/{voiceExperimentId}/calls\n  method: get\n  operationId: getVoiceExperimentCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /test-runs/create-livekit-rooms\n  method: post\n  operationId: createLivekitRooms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method:\
  \ get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{datasetId}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scoring/register-functions\n  method: post\n  operationId: registerScoringFunctions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /traces\n  method: post\n  operationId: ingestTraces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logs\n  method: post\n  operationId: ingestLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/call-logs\n  method: post\n  operationId: ingestCallLog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompts\n  method: get\n  operationId: listPrompts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prompts/{slug}\n  method: get\n  operationId: getPrompt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/agentic-access/hamming-ai-agentic-access.yml
summary_line: 16 operations · 11 acting
tags:
- AI
- Voice Agents
- LLM
- Testing
- Evaluation
- Observability
---
