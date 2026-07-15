---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Indexes API
  slug: twelvelabs-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Tasks (Upload) API
  slug: twelvelabs-tasks-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Search API
  slug: twelvelabs-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Analyze / Generate API
  slug: twelvelabs-analyze-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Embed API
  slug: twelvelabs-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
consequence_counts:
  read: 9
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Twelvelabs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'TwelveLabs exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TwelveLabs
provider_slug: twelvelabs
slug: twelvelabs-agentic-access
source_filename: twelvelabs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/twelvelabs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 9\n    acting: 13\n  by_consequence:\n    read: 9\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /indexes\n  method: get\n  operationId: listIndexes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indexes\n  method: post\n  operationId: createIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /indexes/{index_id}\n  method: get\n  operationId: retrieveIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indexes/{index_id}\n  method: put\n  operationId: updateIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /indexes/{index_id}\n  method: delete\n  operationId: deleteIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /indexes/{index_id}/videos\n  method: get\n  operationId: listVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indexes/{index_id}/videos/{video_id}\n  method: get\n  operationId: retrieveVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indexes/{index_id}/videos/{video_id}\n  method: put\n  operationId: updateVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /indexes/{index_id}/videos/{video_id}\n  method: delete\n  operationId: deleteVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}\n  method: get\n  operationId: retrieveTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}\n  method: delete\n  operationId:\
  \ deleteTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  operationId: createSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/{page_token}\n  method: get\n  operationId: retrieveSearchPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze\n  method: post\n  operationId: analyzeVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gist\n  method: post\n  operationId: generateGist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /summarize\n  method: post\n  operationId: summarizeVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embed\n  method: post\n  operationId: createEmbeddings\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embed/tasks\n  method: post\n  operationId: createEmbeddingTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embed/tasks\n  method: get\n  operationId: listEmbeddingTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embed/tasks/{task_id}\n  method: get\n  operationId: retrieveEmbeddingTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/agentic-access/twelvelabs-agentic-access.yml
summary_line: 22 operations · 13 acting
tags:
- AI
- Video Understanding
- Multimodal
- Search
- Embeddings
---
