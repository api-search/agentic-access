---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 5
api_specs:
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Pipes API
  slug: langbase-pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Agent API
  slug: langbase-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Memory API
  slug: langbase-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Threads API
  slug: langbase-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Tools API
  slug: langbase-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Parser API
  slug: langbase-parser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Chunker API
  slug: langbase-chunker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Embed API
  slug: langbase-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Workflows API
  slug: langbase-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
consequence_counts:
  read: 5
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Langbase Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Langbase exposes 23 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Langbase
provider_slug: langbase
slug: langbase-agentic-access
source_filename: langbase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/langbase-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 18\n    connected: 5\n  by_consequence:\n    write: 18\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/pipes/run\n  method: post\n  operationId: runPipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pipes\n  method: get\n  operationId: listPipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pipes\n  method: post\n  operationId: createPipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pipes/{name}\n  method: post\n  operationId: updatePipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/run\n  method: post\n  operationId: runAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/memory\n  method: get\n  operationId: listMemories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/memory\n  method: post\n  operationId: createMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/memory/{name}\n  method: delete\n  operationId: deleteMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/memory/retrieve\n  method: post\n  operationId: retrieveMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/memory/{name}/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/memory/{name}/documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/memory/{name}/documents/{documentName}\n  method: delete\n\
  \  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/threads\n  method: post\n  operationId: createThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/threads/{threadId}\n  method: get\n  operationId: getThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/threads/{threadId}\n  method: patch\n  operationId: updateThread\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/threads/{threadId}\n  method: delete\n  operationId: deleteThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/threads/{threadId}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/threads/{threadId}/messages\n  method: post\n  operationId: appendMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/web-search\n  method: post\n  operationId: webSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/crawl\n  method: post\n  operationId: crawl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parser\n  method: post\n  operationId: parseDocument\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chunker\n  method: post\n  operationId: chunkContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embed\n  method: post\n  operationId: embed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/agentic-access/langbase-agentic-access.yml
summary_line: 23 operations · 18 acting
tags:
- AI
- Agents
- RAG
- LLM
- Serverless
---
