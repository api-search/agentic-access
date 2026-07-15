---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 10
api_specs:
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Parse Task API
  slug: chunkr-parse-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Extract Task API
  slug: chunkr-extract-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Task Management API
  slug: chunkr-task-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Files API
  slug: chunkr-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Health and Extras API
  slug: chunkr-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
consequence_counts:
  read: 10
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chunkr Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Chunkr exposes 16 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chunkr
provider_slug: chunkr-ai
slug: chunkr-ai-agentic-access
source_filename: chunkr-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chunkr-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 6\n    connected: 10\n  by_consequence:\n    write: 6\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /tasks/parse\n  method: post\n  operationId: createParseTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/extract\n  method: post\n  operationId: createExtractTask\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}\n  method: delete\n  operationId: deleteTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /tasks/{task_id}/parse\n  method: get\n  operationId: getParseTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/extract\n  method: get\n  operationId: getExtractTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/cancel\n  method: post\n  operationId: cancelTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}/download\n  method: get\n  operationId: downloadFileContent\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}/url\n  method: get\n  operationId: getFileUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extras/supported-file-types\n  method: get\n  operationId: getSupportedFileTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/agentic-access/chunkr-ai-agentic-access.yml
summary_line: 16 operations · 6 acting
tags:
- Document Parsing
- OCR
- Chunking
- RAG
- Document Intelligence
---
