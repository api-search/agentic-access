---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: ayushrai-site-ask-api-openapi.yml
  format: yaml
  label: ayushrai-site Ask API
  slug: ayushrai-site-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayushrai-site/openapi/ayushrai-site-ask-api-openapi.yml
- filename: ayushrai-site-compare-api-openapi.yml
  format: yaml
  label: ayushrai-site Compare API
  slug: ayushrai-site-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayushrai-site/openapi/ayushrai-site-compare-api-openapi.yml
- filename: ayushrai-site-mcp-api-openapi.yml
  format: yaml
  label: ayushrai-site MCP API
  slug: ayushrai-site-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayushrai-site/openapi/ayushrai-site-mcp-api-openapi.yml
- filename: ayushrai-site-projects-api-openapi.yml
  format: yaml
  label: ayushrai-site Projects API
  slug: ayushrai-site-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayushrai-site/openapi/ayushrai-site-projects-api-openapi.yml
- filename: ayushrai-site-search-api-openapi.yml
  format: yaml
  label: ayushrai-site Search API
  slug: ayushrai-site-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayushrai-site/openapi/ayushrai-site-search-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ayushrai Site Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'ayushrai-site exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ayushrai-site
provider_slug: ayushrai-site
slug: ayushrai-site-agentic-access
source_filename: ayushrai-site-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/ayushrai-site-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/search\n  method: get\n  operationId: searchPortfolioV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: get\n  operationId: searchPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects\n  method: get\n\
  \  operationId: projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects\n  method: get\n  operationId: listProjectsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/{slug}\n  method: get\n  operationId: getProjectV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/compare\n  method: get\n  operationId: compareProjectsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/server-card\n  method: get\n  operationId: getMcpServerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: get\n  operationId: askGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: post\n  operationId: askPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ayushrai-site/agentic-access/ayushrai-site-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Company
- Artificial Intelligence
- Engineering
- Consulting
- Portfolio
---
