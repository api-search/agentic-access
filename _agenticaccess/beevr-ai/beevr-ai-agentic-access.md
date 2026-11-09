---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: beevr-ai-about-api-openapi.yml
  format: yaml
  label: BeevR About API
  slug: beevr-ai-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beevr-ai/openapi/beevr-ai-about-api-openapi.yml
- filename: beevr-ai-articles-api-openapi.yml
  format: yaml
  label: BeevR Articles API
  slug: beevr-ai-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beevr-ai/openapi/beevr-ai-articles-api-openapi.yml
- filename: beevr-ai-case-studies-api-openapi.yml
  format: yaml
  label: BeevR Case Studies API
  slug: beevr-ai-case-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beevr-ai/openapi/beevr-ai-case-studies-api-openapi.yml
- filename: beevr-ai-health-api-openapi.yml
  format: yaml
  label: BeevR Health API
  slug: beevr-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beevr-ai/openapi/beevr-ai-health-api-openapi.yml
- filename: beevr-ai-pricing-api-openapi.yml
  format: yaml
  label: BeevR Pricing API
  slug: beevr-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beevr-ai/openapi/beevr-ai-pricing-api-openapi.yml
- filename: beevr-ai-search-api-openapi.yml
  format: yaml
  label: BeevR Search API
  slug: beevr-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beevr-ai/openapi/beevr-ai-search-api-openapi.yml
- filename: beevr-ai-services-api-openapi.yml
  format: yaml
  label: BeevR Services API
  slug: beevr-ai-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beevr-ai/openapi/beevr-ai-services-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Beevr Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'BeevR exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BeevR
provider_slug: beevr-ai
slug: beevr-ai-agentic-access
source_filename: beevr-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/beevr-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /case-studies\n  method: get\n  operationId: listCaseStudies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /case-studies/{slug}\n  method: get\n  operationId: getCaseStudy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles\n  method: get\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{slug}\n  method: get\n  operationId: getArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /about\n  method: get\n\
  \  operationId: about\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/beevr-ai/agentic-access/beevr-ai-agentic-access.yml
summary_line: 9 operations
tags:
- Software
- Artificial Intelligence
- Development
- Vietnam
- Regulated Industries
---
