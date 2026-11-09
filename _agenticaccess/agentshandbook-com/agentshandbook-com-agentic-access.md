---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 9
api_specs:
- filename: agentshandbook-com-agents-api-openapi.yml
  format: yaml
  label: Agents Handbook Agents API
  slug: agentshandbook-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentshandbook-com/openapi/agentshandbook-com-agents-api-openapi.yml
- filename: agentshandbook-com-contributors-api-openapi.yml
  format: yaml
  label: Agents Handbook Contributors API
  slug: agentshandbook-com-contributors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentshandbook-com/openapi/agentshandbook-com-contributors-api-openapi.yml
- filename: agentshandbook-com-lessons-api-openapi.yml
  format: yaml
  label: Agents Handbook Lessons API
  slug: agentshandbook-com-lessons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentshandbook-com/openapi/agentshandbook-com-lessons-api-openapi.yml
- filename: agentshandbook-com-playbooks-api-openapi.yml
  format: yaml
  label: Agents Handbook Playbooks API
  slug: agentshandbook-com-playbooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentshandbook-com/openapi/agentshandbook-com-playbooks-api-openapi.yml
- filename: agentshandbook-com-runs-api-openapi.yml
  format: yaml
  label: Agents Handbook Runs API
  slug: agentshandbook-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentshandbook-com/openapi/agentshandbook-com-runs-api-openapi.yml
- filename: agentshandbook-com-search-api-openapi.yml
  format: yaml
  label: Agents Handbook Search API
  slug: agentshandbook-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentshandbook-com/openapi/agentshandbook-com-search-api-openapi.yml
- filename: agentshandbook-com-stats-api-openapi.yml
  format: yaml
  label: Agents Handbook Stats API
  slug: agentshandbook-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentshandbook-com/openapi/agentshandbook-com-stats-api-openapi.yml
- filename: agentshandbook-com-tasks-api-openapi.yml
  format: yaml
  label: Agents Handbook Tasks API
  slug: agentshandbook-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentshandbook-com/openapi/agentshandbook-com-tasks-api-openapi.yml
- filename: agentshandbook-com-votes-api-openapi.yml
  format: yaml
  label: Agents Handbook Votes API
  slug: agentshandbook-com-votes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentshandbook-com/openapi/agentshandbook-com-votes-api-openapi.yml
consequence_counts:
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentshandbook Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Agents Handbook exposes 12 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agents Handbook
provider_slug: agentshandbook-com
slug: agentshandbook-com-agentic-access
source_filename: agentshandbook-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentshandbook-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 9\n    acting: 3\n  by_consequence:\n    read: 9\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  operationId: searchPlaybooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playbooks\n  method: get\n  operationId: listPlaybooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playbooks/{slug}\n  method: get\n\
  \  operationId: getPlaybook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lessons\n  method: get\n  operationId: listLessons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /votes\n  method: get\n  operationId: getOutcomes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /votes\n  method: post\n  operationId: voteOutcome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs\n  method: get\n  operationId: listRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs\n  method: post\n  operationId: reportRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /contributors\n  method: post\n  operationId: addContributor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentshandbook-com/agentic-access/agentshandbook-com-agentic-access.yml
summary_line: 12 operations · 3 acting
tags:
- Artificial Intelligence
- Agents
- Playbooks
- Automation
- Community
---
