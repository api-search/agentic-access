---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: roboto-discovery-api-openapi.yml
  format: yaml
  label: Roboto Discovery API
  slug: roboto-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-discovery-api-openapi.yml
- filename: roboto-markdown-api-openapi.yml
  format: yaml
  label: Roboto Markdown API
  slug: roboto-markdown-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-markdown-api-openapi.yml
- filename: roboto-navigation-api-openapi.yml
  format: yaml
  label: Roboto Navigation API
  slug: roboto-navigation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-navigation-api-openapi.yml
- filename: roboto-pages-api-openapi.yml
  format: yaml
  label: Roboto Pages API
  slug: roboto-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-pages-api-openapi.yml
- filename: roboto-search-api-openapi.yml
  format: yaml
  label: Roboto Search API
  slug: roboto-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roboto/openapi/roboto-search-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Roboto Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Roboto exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Roboto
provider_slug: roboto
slug: roboto-agentic-access
source_filename: roboto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/roboto-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/docs/pages.json\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/docs/pages/{route}.json\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/docs/navigation.json\n  method: get\n  operationId:\
  \ getNavigation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/docs/search\n  method: get\n  operationId: searchDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{route}.md\n  method: get\n  operationId: getPageMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /agent-readability.json\n  method: get\n  operationId: getAgentReadability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/roboto/agentic-access/roboto-agentic-access.yml
summary_line: 8 operations
tags:
- Company
- Robotics
- Artificial Intelligence
- Analytics
- Platform
---
