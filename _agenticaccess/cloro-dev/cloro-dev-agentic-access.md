---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 5
api_specs:
- filename: cloro-dev-async-api-openapi.yml
  format: yaml
  label: cloro Async API
  slug: cloro-dev-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-async-api-openapi.yml
- filename: cloro-dev-countries-api-openapi.yml
  format: yaml
  label: cloro Countries API
  slug: cloro-dev-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-countries-api-openapi.yml
- filename: cloro-dev-credits-api-openapi.yml
  format: yaml
  label: cloro Credits API
  slug: cloro-dev-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-credits-api-openapi.yml
- filename: cloro-dev-monitor-api-openapi.yml
  format: yaml
  label: cloro Monitor API
  slug: cloro-dev-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-monitor-api-openapi.yml
- filename: cloro-dev-states-api-openapi.yml
  format: yaml
  label: cloro States API
  slug: cloro-dev-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-states-api-openapi.yml
consequence_counts:
  read: 5
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloro Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'cloro exposes 17 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: cloro
provider_slug: cloro-dev
slug: cloro-dev-agentic-access
source_filename: cloro-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/cloro-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 12\n    connected: 5\n  by_consequence:\n    write: 12\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/monitor/chatgpt\n  method: post\n  operationId: monitorChatgpt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/gemini\n  method: post\n  operationId: monitorGemini\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/grok\n  method: post\n  operationId: monitorGrok\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/google\n  method: post\n  operationId: monitorGoogle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/google/goto\n  method: post\n  operationId: resolveGoogleGoto\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/google/news\n  method: post\n  operationId: monitorGoogleNews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/copilot\n  method: post\n  operationId: monitorCopilot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/perplexity\n\
  \  method: post\n  operationId: monitorPerplexity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitor/aimode\n  method: post\n  operationId: monitorAiMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/countries\n  method: get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/async/task\n  method: post\n  operationId: createAsyncTask\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/async/task/batch\n  method: post\n  operationId: createBatchAsyncTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/async/task/{taskId}\n  method: get\n  operationId: getTaskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/async/status\n  method: get\n  operationId: getAsyncStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/async/queue\n  method: delete\n  operationId: clearAsyncQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/states\n  method: get\n  operationId: getStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/agentic-access/cloro-dev-agentic-access.yml
summary_line: 17 operations · 12 acting
tags:
- Company
- Search
- AI
- Web Scraping
- SERP
- Generative Engine Optimization
- SEO
- Brand Monitoring
- Market Research
- Data Extraction
- MCP
---
