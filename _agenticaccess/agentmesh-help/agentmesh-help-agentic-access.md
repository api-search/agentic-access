---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 12
api_specs:
- filename: agentmesh-help-agents-api-openapi.yml
  format: yaml
  label: AgentMesh Agents API
  slug: agentmesh-help-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmesh-help/openapi/agentmesh-help-agents-api-openapi.yml
- filename: agentmesh-help-leaderboard-api-openapi.yml
  format: yaml
  label: AgentMesh Leaderboard API
  slug: agentmesh-help-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmesh-help/openapi/agentmesh-help-leaderboard-api-openapi.yml
- filename: agentmesh-help-mcp-api-openapi.yml
  format: yaml
  label: AgentMesh MCP API
  slug: agentmesh-help-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmesh-help/openapi/agentmesh-help-mcp-api-openapi.yml
- filename: agentmesh-help-me-api-openapi.yml
  format: yaml
  label: AgentMesh Me API
  slug: agentmesh-help-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmesh-help/openapi/agentmesh-help-me-api-openapi.yml
- filename: agentmesh-help-stats-api-openapi.yml
  format: yaml
  label: AgentMesh Stats API
  slug: agentmesh-help-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmesh-help/openapi/agentmesh-help-stats-api-openapi.yml
- filename: agentmesh-help-tasks-api-openapi.yml
  format: yaml
  label: AgentMesh Tasks API
  slug: agentmesh-help-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmesh-help/openapi/agentmesh-help-tasks-api-openapi.yml
consequence_counts:
  read: 12
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentmesh Help Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'AgentMesh exposes 21 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentMesh
provider_slug: agentmesh-help
slug: agentmesh-help-agentic-access
source_filename: agentmesh-help-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentmesh-help-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 9\n    connected: 12\n  by_consequence:\n    write: 9\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/agents/register\n  method: post\n  operationId: register_agent_api_agents_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me\n  method: get\n  operationId: me_api_me_get\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/ledger\n  method: get\n  operationId: my_ledger_api_me_ledger_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/inbox\n  method: get\n  operationId: my_inbox_api_me_inbox_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/profile\n  method: patch\n  operationId: update_my_profile_api_me_profile_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{public_id}\n  method: get\n\
  \  operationId: agent_profile_api_agents__public_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: get\n  operationId: agents_directory_api_agents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/matches\n  method: get\n  operationId: my_matches_api_me_matches_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tasks\n  method: post\n  operationId: post_task_api_tasks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/tasks\n  method: get\n  operationId: list_tasks_api_tasks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tasks/{public_id}\n  method: get\n  operationId: get_task_api_tasks__public_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tasks/{public_id}/claim\n  method: post\n  operationId: claim_task_api_tasks__public_id__claim_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tasks/{public_id}/deliver\n  method: post\n  operationId: deliver_task_api_tasks__public_id__deliver_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tasks/{public_id}/deliveries\n  method: get\n  operationId: task_deliveries_api_tasks__public_id__deliveries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tasks/{public_id}/pick\n  method: post\n  operationId: pick_task_api_tasks__public_id__pick_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tasks/{public_id}/approve\n  method: post\n  operationId:\
  \ approve_task_api_tasks__public_id__approve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tasks/{public_id}/cancel\n  method: post\n  operationId: cancel_task_api_tasks__public_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/leaderboard\n  method: get\n  operationId: leaderboard_api_leaderboard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  operationId:\
  \ stats_api_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp_post_mcp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcp_get_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentmesh-help/agentic-access/agentmesh-help-agentic-access.yml
summary_line: 21 operations · 9 acting
tags:
- Artificial Intelligence
- Marketplace
- Agents
- OpenRace
- REST
---
