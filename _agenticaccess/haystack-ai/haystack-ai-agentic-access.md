---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 6
api_specs:
- filename: haystack-ai-openapi.yml
  format: yaml
  label: deepset Cloud API - Pipelines
  slug: deepset-cloud-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openapi.yml
- filename: haystack-ai-openapi.yml
  format: yaml
  label: deepset Cloud API - Search
  slug: deepset-cloud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openapi.yml
- filename: haystack-ai-openapi.yml
  format: yaml
  label: deepset Cloud API - Files
  slug: deepset-cloud-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openapi.yml
- filename: haystack-ai-openapi.yml
  format: yaml
  label: deepset Cloud API - Workspaces
  slug: deepset-cloud-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openapi.yml
consequence_counts:
  physical: 2
  read: 6
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Haystack Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}/undeploy
operation_count: 18
overview: 'Haystack / deepset exposes 18 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 10 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Haystack / deepset
provider_slug: haystack-ai
slug: haystack-ai-agentic-access
source_filename: haystack-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/haystack-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 6\n    acting: 12\n  by_consequence:\n    read: 6\n    write: 10\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}\n  method: delete\n  operationId: deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines\n  method: get\n  operationId: listPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}/pipelines\n\
  \  method: post\n  operationId: createPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}\n  method: get\n  operationId: getPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}\n  method: delete\n  operationId: deletePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}/deploy\n\
  \  method: post\n  operationId: deployPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}/undeploy\n  method: post\n  operationId: undeployPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}/search\n  method: post\n  operationId: searchPipeline\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}/files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/files/{file_id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/files/{file_id}/meta\n  method: patch\n  operationId: updateFileMeta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/upload_sessions\n  method: post\n  operationId: createUploadSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/workspaces/{workspace_name}/upload_sessions/{session_id}\n  method: get\n  operationId: getUploadSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}/upload_sessions/{session_id}\n  method: put\n  operationId: closeUploadSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/agentic-access/haystack-ai-agentic-access.yml
summary_line: 18 operations · 12 acting
tags:
- AI
- LLM
- RAG
- Open Source
- Orchestration
---
