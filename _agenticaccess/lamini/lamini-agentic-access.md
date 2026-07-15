---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 3
api_specs:
- filename: lamini-openapi.yml
  format: yaml
  label: Lamini Inference Completions API
  slug: lamini-inference-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-openapi.yml
- filename: lamini-openapi.yml
  format: yaml
  label: Lamini Fine-Tuning & Memory Tuning API
  slug: lamini-fine-tuning-memory-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-openapi.yml
- filename: lamini-openapi.yml
  format: yaml
  label: Lamini Classify API
  slug: lamini-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-openapi.yml
- filename: lamini-openapi.yml
  format: yaml
  label: Lamini Embeddings API
  slug: lamini-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/openapi/lamini-openapi.yml
consequence_counts:
  read: 3
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lamini Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Lamini exposes 12 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lamini
provider_slug: lamini
slug: lamini-agentic-access
source_filename: lamini-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lamini-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 9\n    connected: 3\n  by_consequence:\n    write: 9\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/streaming_completions\n  method: post\n  operationId: createStreamingCompletion\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embedding\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/train\n  method: post\n  operationId: createTrainingJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/train/jobs\n  method: get\n  operationId: listTrainingJobs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/train/jobs/{job_id}\n  method: get\n  operationId: getTrainingJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/train/jobs/{job_id}/cancel\n  method: post\n  operationId: cancelTrainingJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/train/jobs/{job_id}/resume\n  method: post\n  operationId: resumeTrainingJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/train/jobs/cancel\n  method: post\n  operationId: cancelAllTrainingJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/classifier/{model_id}/classification\n  method: post\n  operationId: classify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/classifier/{model_id}/prediction\n  method: post\n  operationId: predict\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/agentic-access/lamini-agentic-access.yml
summary_line: 12 operations · 9 acting
tags:
- AI
- LLM
- Fine-Tuning
- Memory Tuning
- Inference
---
