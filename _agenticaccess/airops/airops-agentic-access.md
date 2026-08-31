---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 13
api_specs:
- filename: airops-agent-api-openapi.yml
  format: yaml
  label: AirOps Agent API
  slug: airops-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-agent-api-openapi.yml
- filename: airops-analytics-api-openapi.yml
  format: yaml
  label: AirOps Analytics API
  slug: airops-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-analytics-api-openapi.yml
- filename: airops-answers-api-openapi.yml
  format: yaml
  label: AirOps Answers API
  slug: airops-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-answers-api-openapi.yml
- filename: airops-apps-api-openapi.yml
  format: yaml
  label: AirOps Apps API
  slug: airops-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-apps-api-openapi.yml
- filename: airops-brand-kits-api-openapi.yml
  format: yaml
  label: AirOps Brand Kits API
  slug: airops-brand-kits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-brand-kits-api-openapi.yml
- filename: airops-citations-api-openapi.yml
  format: yaml
  label: AirOps Citations API
  slug: airops-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-citations-api-openapi.yml
- filename: airops-competitors-api-openapi.yml
  format: yaml
  label: AirOps Competitors API
  slug: airops-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-competitors-api-openapi.yml
- filename: airops-content-updates-api-openapi.yml
  format: yaml
  label: AirOps Content Updates API
  slug: airops-content-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-content-updates-api-openapi.yml
- filename: airops-executions-api-openapi.yml
  format: yaml
  label: AirOps Executions API
  slug: airops-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-executions-api-openapi.yml
- filename: airops-files-api-openapi.yml
  format: yaml
  label: AirOps Files API
  slug: airops-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-files-api-openapi.yml
- filename: airops-grids-api-openapi.yml
  format: yaml
  label: AirOps Grids API
  slug: airops-grids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-grids-api-openapi.yml
- filename: airops-memory-stores-api-openapi.yml
  format: yaml
  label: AirOps Memory Stores API
  slug: airops-memory-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-memory-stores-api-openapi.yml
- filename: airops-personas-api-openapi.yml
  format: yaml
  label: AirOps Personas API
  slug: airops-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-personas-api-openapi.yml
- filename: airops-prompts-api-openapi.yml
  format: yaml
  label: AirOps Prompts API
  slug: airops-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-prompts-api-openapi.yml
- filename: airops-sentiment-theme-answers-api-openapi.yml
  format: yaml
  label: AirOps Sentiment Theme Answers API
  slug: airops-sentiment-theme-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-sentiment-theme-answers-api-openapi.yml
- filename: airops-tags-api-openapi.yml
  format: yaml
  label: AirOps Tags API
  slug: airops-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-tags-api-openapi.yml
- filename: airops-topics-api-openapi.yml
  format: yaml
  label: AirOps Topics API
  slug: airops-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-topics-api-openapi.yml
- filename: airops-web-pages-api-openapi.yml
  format: yaml
  label: AirOps Web Pages API
  slug: airops-web-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-web-pages-api-openapi.yml
consequence_counts:
  read: 13
  safety-critical: 1
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Airops Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public_api/brand_kits/{brand_kit_id}/topics/list
operation_count: 42
overview: 'AirOps exposes 42 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 28 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AirOps
provider_slug: airops
slug: airops-agentic-access
source_filename: airops-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/airops-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 13\n    acting: 29\n  by_consequence:\n    read: 13\n    write: 28\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /public_api/airops_apps/executions/{execution_uuid}\n  method: get\n  operationId: getExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/airops_apps/{app_uuid}/execute\n  method: post\n  operationId: executeApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/airops_apps/{app_uuid}/async_execute\n  method: post\n  operationId: asyncExecuteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/airops_apps/{app_uuid}/webhook_async_execute\n  method: post\n  operationId: WebhookAsyncExecuteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/airops_apps/executions/{execution_uuid}/cancel\n\
  \  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/airops_apps/executions/{execution_uuid}/retry\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/airops_apps/executions/{execution_uuid}/feedback\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /public_api/airops_apps/:airops_app_id/executions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/airops_apps\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/airops_apps/{app_uuid}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/agent_apps/{app_uuid}/chat\n  method: post\n  operationId: chatWithAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /public_api/agent_apps/{app_uuid}/async_chat\n  method: post\n  operationId: asyncChatWithAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/workspace_files\n  method: post\n  operationId: workspaceFileUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/grids/{grid_id}/sheets/{sheet_id}/generate_csv\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/grids/{grid_id}/sheets/{sheet_id}/download_csv/latest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/vector_stores/{memory_store_id}/search\n  method: get\n  operationId: searchMemoryStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/vector_stores/{memory_store_id}/vector_store_documents\n  method: post\n  operationId: addDocumentToMemoryStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /public_api/vector_stores/{memory_store_id}/vector_store_documents/{memory_store_document_id}\n  method: put\n  operationId: updateDocumentInMemoryStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/vector_stores/{memory_store_id}/vector_store_documents/{memory_store_document_id}\n  method: delete\n  operationId: deleteDocumentFromMemoryStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/list\n  method: post\n  operationId: listBrandKits\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/prompts/list\n  method: post\n  operationId: listBrandKitsPrompts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/prompts/{id}\n  method: get\n  operationId: getBrandKitsPrompt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/brand_kits/{brand_kit_id}/topics/list\n  method: post\n\
  \  operationId: listBrandKitsTopics\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/topics/{id}\n  method: get\n  operationId: getBrandKitsTopic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/brand_kits/{brand_kit_id}/personas/list\n  method: post\n  operationId: listBrandKitsPersonas\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /public_api/brand_kits/{brand_kit_id}/personas/{id}\n  method: get\n  operationId: getBrandKitsPersona\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/brand_kits/{brand_kit_id}/citations/list\n  method: post\n  operationId: listBrandKitsCitations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/citations/show\n  method: post\n  operationId: getBrandKitsCitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/competitors/list\n  method: post\n  operationId: listBrandKitsCompetitors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/competitors/{id}\n  method: get\n  operationId: getBrandKitsCompetitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/brand_kits/{brand_kit_id}/web_pages/list\n  method: post\n  operationId: listBrandKitsWebPages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/analytics\n  method: post\n  operationId: getBrandKitsAnalytic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{id}\n  method: get\n  operationId: getBrandKit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/brand_kits/{brand_kit_id}/sentiment_theme_answers\n  method: post\n  operationId: getBrandKitsSentimentThemeAnswer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/content_updates/list\n  method: post\n  operationId: listBrandKitsContentUpdates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/content_updates\n  method: post\n  operationId: createBrandKitsContentUpdates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/content_updates/{id}\n  method:\
  \ get\n  operationId: getBrandKitsContentUpdate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/brand_kits/{brand_kit_id}/content_updates/{id}\n  method: delete\n  operationId: destroyBrandKitsContentUpdates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/tags/list\n  method: post\n  operationId: listBrandKitsTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/tags/{id}\n\
  \  method: get\n  operationId: getBrandKitsTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_api/brand_kits/{brand_kit_id}/answers/list\n  method: post\n  operationId: listBrandKitsAnswers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public_api/brand_kits/{brand_kit_id}/answers/show\n  method: post\n  operationId: getBrandKitsAnswer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/agentic-access/airops-agentic-access.yml
summary_line: 42 operations · 29 acting · 1 human-in-the-loop
tags:
- Company
- Application
- Artificial Intelligence
- Content
- SEO
- AEO
- Answer Engine Optimization
- Generative Engine Optimization
- Workflows
- MCP
- Analytics
- Agent Skills
- OpenAPI
- Knowledge Base
- Content Marketing
- Citations
---
