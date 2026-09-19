---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 15
api_specs:
- filename: haystack-ai-files-api-openapi.yml
  format: yaml
  label: Haystack / deepset Files API
  slug: haystack-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-files-api-openapi.yml
- filename: haystack-ai-pipelines-api-openapi.yml
  format: yaml
  label: Haystack / deepset Pipelines API
  slug: haystack-ai-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-pipelines-api-openapi.yml
- filename: haystack-ai-search-api-openapi.yml
  format: yaml
  label: Haystack / deepset Search API
  slug: haystack-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-search-api-openapi.yml
- filename: haystack-ai-workspaces-api-openapi.yml
  format: yaml
  label: Haystack / deepset Workspaces API
  slug: haystack-ai-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-workspaces-api-openapi.yml
- filename: haystack-ai-config-api-openapi.yml
  format: yaml
  label: Haystack / deepset Config API
  slug: haystack-ai-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-config-api-openapi.yml
- filename: haystack-ai-dashboard-api-openapi.yml
  format: yaml
  label: Haystack / deepset Dashboard API
  slug: haystack-ai-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-dashboard-api-openapi.yml
- filename: haystack-ai-openai-api-openapi.yml
  format: yaml
  label: Haystack / deepset Openai API
  slug: haystack-ai-openai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-openai-api-openapi.yml
- filename: haystack-ai-status-api-openapi.yml
  format: yaml
  label: Haystack / deepset Status API
  slug: haystack-ai-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/openapi/haystack-ai-status-api-openapi.yml
consequence_counts:
  physical: 5
  read: 15
  write: 17
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
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deploy-yaml
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deploy_files
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /undeploy/{pipeline_name}
operation_count: 37
overview: 'Haystack / deepset exposes 37 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 17 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Haystack / deepset
provider_slug: haystack-ai
slug: haystack-ai-agentic-access
source_filename: haystack-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/haystack-ai-config-api-openapi.yml, openapi/haystack-ai-dashboard-api-openapi.yml,\n  openapi/haystack-ai-files-api-openapi.yml, openapi/haystack-ai-openai-api-openapi.yml, openapi/haystack-ai-pipelines-api-openapi.yml,\n  openapi/haystack-ai-search-api-openapi.yml, openapi/haystack-ai-status-api-openapi.yml, openapi/haystack-ai-workspaces-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 15\n    acting: 22\n  by_consequence:\n    read: 15\n    physical: 5\n    write: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /draw/{pipeline_name}\n  method: get\n  operationId: pipeline_draw\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deploy-yaml\n  method: post\n  operationId: yaml_pipeline_deploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deploy_files\n  method: post\n  operationId: pipeline_deploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /undeploy/{pipeline_name}\n  method: post\n  operationId: pipeline_undeploy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/api/entrypoints\n  method: get\n  operationId: dashboard_entrypoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/api/config\n  method: get\n  operationId: dashboard_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/api/traces\n  method: get\n  operationId: dashboard_traces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /dashboard/api/traces/stream\n  method: get\n  operationId: dashboard_traces_stream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/api/traces/clear\n  method: post\n  operationId: dashboard_clear_traces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}/files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/files/{file_id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/files/{file_id}/meta\n  method: patch\n  operationId: updateFileMeta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/workspaces/{workspace_name}/upload_sessions\n  method: post\n  operationId: createUploadSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/upload_sessions/{session_id}\n  method: get\n  operationId: getUploadSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}/upload_sessions/{session_id}\n  method: put\n  operationId: closeUploadSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: openai_models_alias\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models\n  method: get\n  operationId: openai_models\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/completions\n  method: post\n  operationId: openai_chat_completions_alias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: openai_chat_completions\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /responses\n  method: post\n  operationId: openai_responses_alias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/responses\n  method: post\n  operationId: openai_responses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: post\n  operationId: openai_files_create_alias\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files\n  method: post\n  operationId: openai_files_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines\n  method: get\n  operationId: listPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}/pipelines\n  method: post\n  operationId: createPipeline\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}\n  method: get\n  operationId: getPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}\n  method: delete\n  operationId: deletePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}/deploy\n  method: post\n  operationId: deployPipeline\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}/undeploy\n  method: post\n  operationId: undeployPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}/pipelines/{pipeline_name}/search\n  method: post\n  operationId: searchPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: get\n  operationId: status_all\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/{pipeline_name}\n  method: get\n  operationId: status_pipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspaces/{workspace_name}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspaces/{workspace_name}\n  method: delete\n  operationId: deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haystack-ai/refs/heads/main/agentic-access/haystack-ai-agentic-access.yml
summary_line: 37 operations · 22 acting
tags:
- Artificial Intelligence
- LLM
- RAG
- Open-Source
- Orchestration
---
