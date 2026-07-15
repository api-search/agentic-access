---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: llamacloud-openapi.yml
  format: yaml
  label: LlamaParse API
  slug: llamaparse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-openapi.yml
- filename: llamacloud-openapi.yml
  format: yaml
  label: LlamaCloud Pipelines and Indexes API
  slug: pipelines-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-openapi.yml
- filename: llamacloud-openapi.yml
  format: yaml
  label: LlamaCloud Documents and Files API
  slug: documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-openapi.yml
- filename: llamacloud-openapi.yml
  format: yaml
  label: LlamaCloud Retrieval API
  slug: retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-openapi.yml
- filename: llamacloud-openapi.yml
  format: yaml
  label: LlamaExtract API
  slug: llamaextract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/openapi/llamacloud-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Llamacloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pipelines/{pipeline_id}/files
operation_count: 19
overview: 'LlamaCloud exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 7 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LlamaCloud
provider_slug: llamacloud
slug: llamacloud-agentic-access
source_filename: llamacloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/llamacloud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 8\n    connected: 11\n  by_consequence:\n    write: 7\n    read: 11\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /parsing/upload\n  method: post\n  operationId: uploadParsingJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parsing/job/{job_id}\n  method: get\n  operationId: getParsingJob\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parsing/job/{job_id}/result/markdown\n  method: get\n  operationId: getParsingResultMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parsing/job/{job_id}/result/json\n  method: get\n  operationId: getParsingResultJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: get\n  operationId: listFiles\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines\n  method: post\n  operationId: createPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines\n  method: get\n  operationId: listPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipeline_id}\n  method: get\n  operationId: getPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipeline_id}/status\n  method: get\n  operationId: getPipelineStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipeline_id}/files\n  method: post\n  operationId: addFilesToPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pipelines/{pipeline_id}/documents\n  method: post\n  operationId: createPipelineDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipeline_id}/documents\n  method: get\n  operationId:\
  \ listPipelineDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipeline_id}/retrieve\n  method: post\n  operationId: retrieveFromPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extraction/extraction-agents\n  method: post\n  operationId: createExtractionAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extraction/extraction-agents\n  method: get\n  operationId: listExtractionAgents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extraction/jobs\n  method: post\n  operationId: runExtractionJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extraction/jobs/{job_id}\n  method: get\n  operationId: getExtractionJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extraction/jobs/{job_id}/result\n  method: get\n  operationId: getExtractionJobResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llamacloud/refs/heads/main/agentic-access/llamacloud-agentic-access.yml
summary_line: 19 operations · 8 acting · 1 human-in-the-loop
tags:
- AI
- Document Parsing
- Extraction
- Indexing
- Retrieval
- RAG
---
