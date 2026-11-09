---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 7
api_specs:
- filename: deepskyai-com-compliance-api-openapi.yml
  format: yaml
  label: Deepsky Compliance API
  slug: deepskyai-com-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-compliance-api-openapi.yml
- filename: deepskyai-com-deepsky-aviation-agent-api-api-openapi.yml
  format: yaml
  label: Deepsky Deepsky Aviation Agent API
  slug: deepskyai-com-deepsky-aviation-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-deepsky-aviation-agent-api-api-openapi.yml
- filename: deepskyai-com-mcp-api-openapi.yml
  format: yaml
  label: Deepsky MCP API
  slug: deepskyai-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-mcp-api-openapi.yml
- filename: deepskyai-com-search-api-openapi.yml
  format: yaml
  label: Deepsky Search API
  slug: deepskyai-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-search-api-openapi.yml
- filename: deepskyai-com-skills-api-openapi.yml
  format: yaml
  label: Deepsky Skills API
  slug: deepskyai-com-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepskyai-com/openapi/deepskyai-com-skills-api-openapi.yml
consequence_counts:
  read: 7
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deepskyai Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Deepsky exposes 11 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Deepsky
provider_slug: deepskyai-com
slug: deepskyai-com-agentic-access
source_filename: deepskyai-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/deepskyai-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 7\n    acting: 4\n  by_consequence:\n    read: 7\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/search/{query}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/compliance/audit\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/skills\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/skills\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/deepskyai-com/agentic-access/deepskyai-com-agentic-access.yml
summary_line: 11 operations · 4 acting
tags:
- Aviation
- Artificial Intelligence
- Automation
- Documentation
- Compliance
- Company
---
