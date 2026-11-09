---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: ai-portal-ai-ai-portal-public-api-api-openapi.yml
  format: yaml
  label: AI-Portal AI Portal Public API
  slug: ai-portal-ai-ai-portal-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-portal-ai/openapi/ai-portal-ai-ai-portal-public-api-api-openapi.yml
- filename: ai-portal-ai-glossary-api-openapi.yml
  format: yaml
  label: AI-Portal Glossary API
  slug: ai-portal-ai-glossary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-portal-ai/openapi/ai-portal-ai-glossary-api-openapi.yml
- filename: ai-portal-ai-news-api-openapi.yml
  format: yaml
  label: AI-Portal News API
  slug: ai-portal-ai-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-portal-ai/openapi/ai-portal-ai-news-api-openapi.yml
- filename: ai-portal-ai-regulations-api-openapi.yml
  format: yaml
  label: AI-Portal Regulations API
  slug: ai-portal-ai-regulations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-portal-ai/openapi/ai-portal-ai-regulations-api-openapi.yml
- filename: ai-portal-ai-releases-api-openapi.yml
  format: yaml
  label: AI-Portal Releases API
  slug: ai-portal-ai-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-portal-ai/openapi/ai-portal-ai-releases-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ai Portal Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'AI-Portal exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AI-Portal
provider_slug: ai-portal-ai
slug: ai-portal-ai-agentic-access
source_filename: ai-portal-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/ai-portal-ai.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/releases\n  method: get\n  operationId: listReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/regulations\n  method: get\n  operationId: listRegulations\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/glossary\n  method: get\n  operationId: searchGlossary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/news\n  method: get\n  operationId: getLatestNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ai-portal-ai/agentic-access/ai-portal-ai-agentic-access.yml
summary_line: 5 operations
tags:
- Artificial Intelligence
- News
- Tools
- Courses
- Compliance
- Company
---
