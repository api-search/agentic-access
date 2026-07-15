---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 13
api_specs:
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Query Chat API
  slug: kapa-ai-query-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Threads Conversations API
  slug: kapa-ai-threads-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Search and Retrieval API
  slug: kapa-ai-search-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Projects API
  slug: kapa-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
- filename: kapa-ai-openapi.yml
  format: yaml
  label: kapa.ai Analytics API
  slug: kapa-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/openapi/kapa-ai-openapi.yml
consequence_counts:
  read: 13
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kapa Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'kapa.ai exposes 20 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: kapa.ai
provider_slug: kapa-ai
slug: kapa-ai-agentic-access
source_filename: kapa-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kapa-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 7\n    connected: 13\n  by_consequence:\n    write: 7\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /query/v1/projects/{project_id}/chat\n  method: post\n  operationId: chat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/v1/projects/{project_id}/chat/stream\n  method: post\n  operationId: chatStream\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/v1/projects/{project_id}/chat/custom\n  method: post\n  operationId: chatCustom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/v1/threads/{thread_id}/chat\n  method: post\n  operationId: chatInThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /query/v1/threads/{thread_id}/chat/stream\n  method: post\n  operationId: chatInThreadStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/v1/threads/{thread_id}\n  method: get\n  operationId: getThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/v1/projects/{project_id}/threads\n  method: get\n  operationId: listThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/v1/feedback\n  method: post\n  operationId: upsertFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/v1/projects/{project_id}/retrieval\n  method: post\n  operationId: retrieval\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/v1/projects/{project_id}/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/v1/projects/{project_id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /query/v1/projects/{project_id}/integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ingestion/v1/projects/{project_id}/sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/v1/projects/{project_id}/activity\n  method: get\n  operationId: getActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/v1/projects/{project_id}/question-answers\n  method: get\n  operationId: listQuestionAnswers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /query/v1/projects/{project_id}/end-users\n  method: get\n  operationId: listEndUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/v1/projects/{project_id}/coverage-gaps/periods\n  method: get\n  operationId: listCoverageGapsPeriods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/v1/coverage-gaps/periods/{period_id}\n  method: get\n  operationId: getCoverageGapsPeriod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/v1/projects/{project_id}/top-questions/periods\n  method: get\n  operationId: listTopQuestionsPeriods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /query/v1/top-questions/periods/{period_id}\n  method: get\n  operationId: getTopQuestionsPeriod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kapa-ai/refs/heads/main/agentic-access/kapa-ai-agentic-access.yml
summary_line: 20 operations · 7 acting
tags:
- AI
- Answer Engine
- RAG
- Documentation
- Developer Tools
---
