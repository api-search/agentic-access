---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 3
api_specs:
- filename: langdb-openapi.yml
  format: yaml
  label: LangDB Chat Completions / Routing API
  slug: langdb-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-openapi.yml
- filename: langdb-openapi.yml
  format: yaml
  label: LangDB Embeddings API
  slug: langdb-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-openapi.yml
- filename: langdb-openapi.yml
  format: yaml
  label: LangDB Images API
  slug: langdb-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-openapi.yml
- filename: langdb-openapi.yml
  format: yaml
  label: LangDB Models API
  slug: langdb-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-openapi.yml
- filename: langdb-openapi.yml
  format: yaml
  label: LangDB Threads / Messages API
  slug: langdb-threads-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-openapi.yml
- filename: langdb-openapi.yml
  format: yaml
  label: LangDB Analytics / Usage API
  slug: langdb-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-openapi.yml
- filename: langdb-openapi.yml
  format: yaml
  label: LangDB MCP Gateway API
  slug: langdb-mcp-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-openapi.yml
consequence_counts:
  read: 3
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Langdb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'LangDB exposes 10 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LangDB
provider_slug: langdb
slug: langdb-agentic-access
source_filename: langdb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/langdb-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 7\n    connected: 3\n  by_consequence:\n    write: 7\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generations\n  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /threads/{thread_id}/messages\n  method: get\n  operationId: getThreadMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /threads/{thread_id}/cost\n  method: get\n  operationId: getThreadCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics\n  method: post\n  operationId: fetchAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/summary\n  method: post\n  operationId: fetchAnalyticsSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usage/total\n  method: post\n  operationId:\
  \ getTotalUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usage/models\n  method: post\n  operationId: getUsageByModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/agentic-access/langdb-agentic-access.yml
summary_line: 10 operations · 7 acting
tags:
- AI
- LLM
- AI Gateway
- Routing
- Governance
- MCP
---
