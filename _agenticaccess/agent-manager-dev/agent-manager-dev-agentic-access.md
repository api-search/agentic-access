---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: agent-manager-dev-docs-api-openapi.yml
  format: yaml
  label: agent-manager-dev Docs API
  slug: agent-manager-dev-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-manager-dev/openapi/agent-manager-dev-docs-api-openapi.yml
- filename: agent-manager-dev-meta-api-openapi.yml
  format: yaml
  label: agent-manager-dev Meta API
  slug: agent-manager-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-manager-dev/openapi/agent-manager-dev-meta-api-openapi.yml
- filename: agent-manager-dev-product-api-openapi.yml
  format: yaml
  label: agent-manager-dev Product API
  slug: agent-manager-dev-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-manager-dev/openapi/agent-manager-dev-product-api-openapi.yml
- filename: agent-manager-dev-releases-api-openapi.yml
  format: yaml
  label: agent-manager-dev Releases API
  slug: agent-manager-dev-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-manager-dev/openapi/agent-manager-dev-releases-api-openapi.yml
consequence_counts:
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agent Manager Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'agent-manager-dev exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: agent-manager-dev
provider_slug: agent-manager-dev
slug: agent-manager-dev-agentic-access
source_filename: agent-manager-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/agent-manager-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/docs\n  method: get\n  operationId: listDocPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/docs/{slug}\n  method: get\n  operationId:\
  \ getDocPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: get\n  operationId: listSupportedAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools\n  method: get\n  operationId: listMcpTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/release\n  method: get\n  operationId: getLatestRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/batch\n  method: post\n  operationId: runBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ask\n  method: post\n  operationId: askNaturalLanguage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/search\n  method: get\n  operationId: searchDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agent-manager-dev/agentic-access/agent-manager-dev-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Artificial Intelligence
- Agents
- Terminal
- Open Source
- Go
---
