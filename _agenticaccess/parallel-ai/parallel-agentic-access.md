---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 18
api_specs:
- filename: parallel-chat-api-beta-api-openapi.yml
  format: yaml
  label: Parallel Chat API (Beta) API
  slug: parallel-ai-chat-api-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-ai/refs/heads/main/openapi/parallel-chat-api-beta-api-openapi.yml
- filename: parallel-extract-api-openapi.yml
  format: yaml
  label: Parallel Extract API
  slug: parallel-ai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-ai/refs/heads/main/openapi/parallel-extract-api-openapi.yml
- filename: parallel-findall-api-openapi.yml
  format: yaml
  label: Parallel FindAll API
  slug: parallel-ai-findall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-ai/refs/heads/main/openapi/parallel-findall-api-openapi.yml
- filename: parallel-monitor-api-openapi.yml
  format: yaml
  label: Parallel Monitor API
  slug: parallel-ai-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-ai/refs/heads/main/openapi/parallel-monitor-api-openapi.yml
- filename: parallel-search-api-openapi.yml
  format: yaml
  label: Parallel Search API
  slug: parallel-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-ai/refs/heads/main/openapi/parallel-search-api-openapi.yml
- filename: parallel-tasks-api-openapi.yml
  format: yaml
  label: Parallel Tasks API
  slug: parallel-ai-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-ai/refs/heads/main/openapi/parallel-tasks-api-openapi.yml
- filename: parallel-memory-api-openapi.yml
  format: yaml
  label: Parallel Memory API
  slug: parallel-ai-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-ai/refs/heads/main/openapi/parallel-memory-api-openapi.yml
- filename: parallel-responses-api-api-openapi.yml
  format: yaml
  label: Parallel Responses API
  slug: parallel-ai-responses-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-ai/refs/heads/main/openapi/parallel-responses-api-api-openapi.yml
consequence_counts:
  read: 18
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Parallel Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'Parallel exposes 36 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Parallel
provider_slug: parallel-ai
slug: parallel-agentic-access
source_filename: parallel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/parallel-chat-api-beta-api-openapi.yml, openapi/parallel-extract-api-openapi.yml,\n  openapi/parallel-findall-api-openapi.yml, openapi/parallel-memory-api-openapi.yml, openapi/parallel-monitor-api-openapi.yml,\n  openapi/parallel-responses-api-api-openapi.yml, openapi/parallel-search-api-openapi.yml, openapi/parallel-tasks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 18\n    connected: 18\n  by_consequence:\n    write: 18\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /v1beta/chat/completions\n  method: post\n  operationId: chat_completions_v1beta_chat_completions_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extract\n  method: post\n  operationId: extract_v1_extract_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/findall/entity-search\n  method: post\n  operationId: findall_entity_search_v1beta_findall_entity_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v1beta/findall/ingest\n  method: post\n  operationId: ingest_findall_run_v1beta_findall_ingest_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/findall/runs\n  method: post\n  operationId: findall_runs_v1_v1beta_findall_runs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/findall/runs/{findall_id}\n  method: get\n  operationId: findall_runs_v1_get_v1beta_findall_runs__findall_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1beta/findall/runs/{findall_id}/cancel\n  method: post\n  operationId: cancel_findall_run_v1beta_findall_runs__findall_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/findall/runs/{findall_id}/enrich\n  method: post\n  operationId: enrich_findall_run_v1beta_findall_runs__findall_id__enrich_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/findall/runs/{findall_id}/events\n  method: get\n  operationId: get_findall_events_v1beta_findall_runs__findall_id__events_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/findall/runs/{findall_id}/extend\n  method: post\n  operationId: extend_findall_run_v1beta_findall_runs__findall_id__extend_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/findall/runs/{findall_id}/result\n  method: get\n  operationId: get_findall_result_v1beta_findall_runs__findall_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/findall/runs/{findall_id}/schema\n  method: get\n  operationId: get_findall_schema_v1beta_findall_runs__findall_id__schema_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/memory/clear\n  method: post\n  operationId: clear_memory_v1beta_memory_clear_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/memory/evict\n  method: post\n  operationId: evict_memory_source_v1beta_memory_evict_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/memory/retrieve\n  method: post\n  operationId: retrieve_memory_v1beta_memory_retrieve_post\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors\n  method: post\n  operationId: create_monitor_v1_monitors_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors\n  method: get\n  operationId: list_monitors_v1_monitors_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{monitor_id}\n  method: get\n  operationId: retrieve_monitor_v1_monitors__monitor_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/monitors/{monitor_id}/cancel\n  method: post\n  operationId: cancel_monitor_v1_monitors__monitor_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{monitor_id}/events\n  method: get\n  operationId: list_monitor_events_v1_monitors__monitor_id__events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{monitor_id}/trigger\n  method: post\n  operationId: trigger_monitor_run_v1_monitors__monitor_id__trigger_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{monitor_id}/update\n  method: post\n  operationId: update_monitor_v1_monitors__monitor_id__update_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/responses\n  method: post\n  operationId: create_response_v1_responses_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/search\n  method: post\n  operationId: v1_search_v1_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tasks/groups\n  method: post\n  operationId: tasks_taskgroups_post_v1_tasks_groups_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tasks/groups/{taskgroup_id}\n  method: get\n  operationId: tasks_taskgroups_get_v1_tasks_groups__taskgroup_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tasks/groups/{taskgroup_id}/events\n  method: get\n  operationId: tasks_sessions_events_get_v1_tasks_groups__taskgroup_id__events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/tasks/groups/{taskgroup_id}/runs\n  method: post\n  operationId: tasks_taskgroups_runs_post_v1_tasks_groups__taskgroup_id__runs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tasks/groups/{taskgroup_id}/runs\n  method: get\n  operationId: tasks_taskgroups_runs_get_v1_tasks_groups__taskgroup_id__runs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tasks/groups/{taskgroup_id}/runs/{run_id}\n  method: get\n  operationId: tasks_taskgroups_runs_id_get_v1_tasks_groups__taskgroup_id__runs__run_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/tasks/runs\n  method: post\n  operationId: tasks_runs_post_v1_tasks_runs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tasks/runs/{run_id}\n  method: get\n  operationId: tasks_runs_get_v1_tasks_runs__run_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tasks/runs/{run_id}/events\n  method: get\n  operationId: tasks_runs_events_get_v1_tasks_runs__run_id__events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tasks/runs/{run_id}/input\n  method: get\n  operationId:\
  \ tasks_runs_input_get_v1_tasks_runs__run_id__input_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tasks/runs/{run_id}/result\n  method: get\n  operationId: tasks_runs_result_get_v1_tasks_runs__run_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/tasks/runs/{run_id}/events\n  method: get\n  operationId: tasks_runs_events_get_v1beta_tasks_runs__run_id__events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel-ai/refs/heads/main/agentic-access/parallel-agentic-access.yml
summary_line: 36 operations · 18 acting
tags:
- Company
- Artificial Intelligence
- Web Search
- Agents
- Deep Research
- Web Extraction
- Data Enrichment
- Web Monitoring
- LLM Tools
- A2A
- Ai Ml
- AI Agents
- MCP
- Agent Skills
- Content Extraction
- Entity Resolution
---
