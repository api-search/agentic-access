---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 9
api_specs:
- filename: gatherhq-com-agents-api-openapi.yml
  format: yaml
  label: Gather Agents API
  slug: gatherhq-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-agents-api-openapi.yml
- filename: gatherhq-com-dimensions-api-openapi.yml
  format: yaml
  label: Gather Dimensions API
  slug: gatherhq-com-dimensions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-dimensions-api-openapi.yml
- filename: gatherhq-com-health-api-openapi.yml
  format: yaml
  label: Gather Health API
  slug: gatherhq-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-health-api-openapi.yml
- filename: gatherhq-com-mcp-api-openapi.yml
  format: yaml
  label: Gather MCP API
  slug: gatherhq-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-mcp-api-openapi.yml
- filename: gatherhq-com-questions-api-openapi.yml
  format: yaml
  label: Gather Questions API
  slug: gatherhq-com-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-questions-api-openapi.yml
- filename: gatherhq-com-reviews-api-openapi.yml
  format: yaml
  label: Gather Reviews API
  slug: gatherhq-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-reviews-api-openapi.yml
- filename: gatherhq-com-sources-api-openapi.yml
  format: yaml
  label: Gather Sources API
  slug: gatherhq-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-sources-api-openapi.yml
- filename: gatherhq-com-stats-api-openapi.yml
  format: yaml
  label: Gather Stats API
  slug: gatherhq-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-stats-api-openapi.yml
- filename: gatherhq-com-tools-api-openapi.yml
  format: yaml
  label: Gather Tools API
  slug: gatherhq-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatherhq-com/openapi/gatherhq-com-tools-api-openapi.yml
consequence_counts:
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gatherhq Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Gather exposes 11 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gather
provider_slug: gatherhq-com
slug: gatherhq-com-agentic-access
source_filename: gatherhq-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/gatherhq-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 9\n    acting: 2\n  by_consequence:\n    read: 9\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/tools\n  method: get\n  operationId: get_tools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tools/{tool_id}\n  method: get\n  operationId: get_tools_tool_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reviews\n  method: get\n\
  \  operationId: get_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reviews\n  method: post\n  operationId: submit_review\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/stats\n  method: get\n  operationId: get_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dimensions\n  method: get\n  operationId: get_dimensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sources\n  method: get\n  operationId: get_sources\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: get_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/questions\n  method: get\n  operationId: get_questions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: get\n  operationId: get_agents\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/gatherhq-com/agentic-access/gatherhq-com-agentic-access.yml
summary_line: 11 operations · 2 acting
tags:
- Company
- Buyer Intelligence
- Market Research
- GTM-Tools
- Software-as-a-Service
---
