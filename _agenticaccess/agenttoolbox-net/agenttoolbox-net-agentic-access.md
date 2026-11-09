---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: agenttoolbox-net-directory-api-openapi.yml
  format: yaml
  label: Agent Toolbox Directory API
  slug: agenttoolbox-net-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenttoolbox-net/openapi/agenttoolbox-net-directory-api-openapi.yml
- filename: agenttoolbox-net-tools-api-openapi.yml
  format: yaml
  label: Agent Toolbox Tools API
  slug: agenttoolbox-net-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenttoolbox-net/openapi/agenttoolbox-net-tools-api-openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agenttoolbox Net Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Agent Toolbox exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agent Toolbox
provider_slug: agenttoolbox-net
slug: agenttoolbox-net-agentic-access
source_filename: agenttoolbox-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agenttoolbox-net-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 2\n    acting: 3\n  by_consequence:\n    read: 2\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/tools\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/directory\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tools/estimate_tokens\n  method: post\n  operationId: estimate_tokens\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/convert_schema\n  method: post\n  operationId: convert_schema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/mcp_config\n  method: post\n  operationId: mcp_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agenttoolbox-net/agentic-access/agenttoolbox-net-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Artificial Intelligence
- Tools
- Free
- Browser
- Agents
---
