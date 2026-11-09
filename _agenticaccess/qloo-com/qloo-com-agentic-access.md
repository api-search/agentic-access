---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: qloo-com-analysis-api-openapi.yml
  format: yaml
  label: Qloo Analysis API
  slug: qloo-com-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qloo-com/openapi/qloo-com-analysis-api-openapi.yml
- filename: qloo-com-audiences-api-openapi.yml
  format: yaml
  label: Qloo Audiences API
  slug: qloo-com-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qloo-com/openapi/qloo-com-audiences-api-openapi.yml
- filename: qloo-com-entities-api-openapi.yml
  format: yaml
  label: Qloo Entities API
  slug: qloo-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qloo-com/openapi/qloo-com-entities-api-openapi.yml
- filename: qloo-com-info-api-openapi.yml
  format: yaml
  label: Qloo Info API
  slug: qloo-com-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qloo-com/openapi/qloo-com-info-api-openapi.yml
- filename: qloo-com-insights-api-openapi.yml
  format: yaml
  label: Qloo Insights API
  slug: qloo-com-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qloo-com/openapi/qloo-com-insights-api-openapi.yml
- filename: qloo-com-search-api-openapi.yml
  format: yaml
  label: Qloo Search API
  slug: qloo-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qloo-com/openapi/qloo-com-search-api-openapi.yml
- filename: qloo-com-tags-api-openapi.yml
  format: yaml
  label: Qloo Tags API
  slug: qloo-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qloo-com/openapi/qloo-com-tags-api-openapi.yml
- filename: qloo-com-trends-api-openapi.yml
  format: yaml
  label: Qloo Trends API
  slug: qloo-com-trends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qloo-com/openapi/qloo-com-trends-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Qloo Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Qloo exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qloo
provider_slug: qloo-com
slug: qloo-com-agentic-access
source_filename: qloo-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/qloo-com-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: api-information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities\n  method: get\n  operationId: get-entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: get-search\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/analysis/compare\n  method: get\n  operationId: analysis-compare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/audiences\n  method: get\n  operationId: get-audiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/audiences/types\n  method: get\n  operationId: get-audience-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/insights\n  method: get\n  operationId: get-insights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/tags\n  method: get\n  operationId: get-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tags/types\n  method: get\n  operationId: get-tag-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trending\n  method: get\n  operationId: get-trending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/qloo-com/agentic-access/qloo-com-agentic-access.yml
summary_line: 10 operations
tags:
- Company
- Artificial Intelligence
- Cultural-Intelligence
- Data Analytics
- Personalization
---
