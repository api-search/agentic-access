---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: taskbullet-com-api-openapi.json
  format: json
  label: TaskBullet Agent API API
  slug: taskbullet-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taskbullet-com/openapi/_original/taskbullet-com-api-openapi.json
consequence_counts:
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Taskbullet Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'taskbullet-com exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: taskbullet-com
provider_slug: taskbullet-com
slug: taskbullet-com-agentic-access
source_filename: taskbullet-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/taskbullet-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 1\n    connected: 1\n  by_consequence:\n    write: 1\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /delegate\n  method: post\n  operationId: delegateTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/taskbullet-com/agentic-access/taskbullet-com-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Company
- Virtual Assistant
- Software-as-a-Service
- USBusiness
- Productivity
---
