---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 15
api_specs:
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Agents API
  slug: agno-agentos-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Teams API
  slug: agno-agentos-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Workflows API
  slug: agno-agentos-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Sessions API
  slug: agno-agentos-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Memory API
  slug: agno-agentos-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Knowledge API
  slug: agno-agentos-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
- filename: agno-agi-openapi.yml
  format: yaml
  label: Agno AgentOS Evals API
  slug: agno-agentos-evals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/openapi/agno-agi-openapi.yml
consequence_counts:
  read: 15
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agno Agi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Agno exposes 26 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agno
provider_slug: agno-agi
slug: agno-agi-agentic-access
source_filename: agno-agi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/agno-agi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 15\n    acting: 11\n  by_consequence:\n    read: 15\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}/runs\n  method: post\n\
  \  operationId: createAgentRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs/{run_id}/cancel\n  method: post\n  operationId: cancelRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{team_id}/runs\n  method: post\n  operationId: createTeamRun\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflows\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/{workflow_id}\n  method: get\n  operationId: getWorkflowDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/{workflow_id}/runs\n  method: post\n  operationId: executeWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /workflows/{workflow_id}/runs/{run_id}\n  method: get\n  operationId: getWorkflowRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/{workflow_id}/runs/{run_id}\n  method: delete\n  operationId: cancelWorkflowRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}\n  method: get\n  operationId: getSessionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}\n  method: delete\n  operationId: deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/runs\n  method: get\n  operationId: getSessionRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /memories\n  method: get\n  operationId: listMemories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memories\n  method: post\n  operationId: createMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /memories/topics\n  method: get\n  operationId: getMemoryTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memories/stats\n  method: get\n  operationId: getUserMemoryStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memories/optimize\n\
  \  method: post\n  operationId: optimizeUserMemories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /knowledge/content\n  method: get\n  operationId: listContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /knowledge/content\n  method: post\n  operationId: uploadContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /knowledge/search\n  method: get\n  operationId: searchKnowledge\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eval-runs\n  method: get\n  operationId: listEvaluationRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eval-runs\n  method: post\n  operationId: executeEvaluation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agno-agi/refs/heads/main/agentic-access/agno-agi-agentic-access.yml
summary_line: 26 operations · 11 acting
tags:
- AI
- Agents
- Multi-Agent
- LLM
- Framework
- Open Source
- Runtime
---
