---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 11
api_specs:
- filename: writer-openapi.yml
  format: yaml
  label: Writer Chat Completion API
  slug: writer-chat-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Text Generation API
  slug: writer-text-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Tool Calling API
  slug: writer-tool-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Knowledge Graph API
  slug: writer-knowledge-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Files API
  slug: writer-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Applications API
  slug: writer-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Vision API
  slug: writer-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Web Search API
  slug: writer-web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Translation API
  slug: writer-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Models API
  slug: writer-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Guardrails API
  slug: writer-guardrails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer API Keys API
  slug: writer-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
consequence_counts:
  read: 11
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Writer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Writer exposes 30 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Writer
provider_slug: writer
slug: writer-agentic-access
source_filename: writer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/writer-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 19\n    connected: 11\n  by_consequence:\n    write: 19\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/chat\n  method: post\n  operationId: chat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/completions\n  method: post\n  operationId: completions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: models\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/graphs\n  method: get\n  operationId: findGraphsWithFileStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/graphs\n  method: post\n  operationId: createGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/graphs/question\n\
  \  method: post\n  operationId: question\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/graphs/{graph_id}\n  method: get\n  operationId: findGraphWithFileStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/graphs/{graph_id}\n  method: put\n  operationId: updateGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/graphs/{graph_id}\n  method: delete\n  operationId: deleteGraph\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/graphs/{graph_id}/file\n  method: post\n  operationId: addFileToGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/graphs/{graph_id}/file/{file_id}\n  method: delete\n  operationId: removeFileFromGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/files/{file_id}\n  method: get\n  operationId: gatewayGetFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_id}\n  method: delete\n  operationId: gatewayDeleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files\n  method: get\n  operationId: gatewayGetFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files\n  method: post\n  operationId: gatewayUploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{file_id}/download\n  method: get\n  operationId: gatewayDownloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/retry\n  method: post\n  operationId: gatewayRetryFailedFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{application_id}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{application_id}\n  method: post\n  operationId: generateContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/{application_id}/jobs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{application_id}/jobs\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/applications/jobs/{job_id}/retry\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/jobs/{job_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{application_id}/graphs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{application_id}/graphs\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/pdf-parser/{file_id}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/web-search\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vision\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/translation\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/agentic-access/writer-agentic-access.yml
summary_line: 30 operations · 19 acting
tags:
- AI
- LLM
- Enterprise
- Content Generation
- Palmyra
- Agents
---
