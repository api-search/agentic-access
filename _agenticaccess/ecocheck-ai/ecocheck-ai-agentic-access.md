---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: ecocheck-ai-about-api-openapi.yml
  format: yaml
  label: EcoCheck About API
  slug: ecocheck-ai-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-about-api-openapi.yml
- filename: ecocheck-ai-articles-api-openapi.yml
  format: yaml
  label: EcoCheck Articles API
  slug: ecocheck-ai-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-articles-api-openapi.yml
- filename: ecocheck-ai-cbam-api-openapi.yml
  format: yaml
  label: EcoCheck Cbam API
  slug: ecocheck-ai-cbam-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-cbam-api-openapi.yml
- filename: ecocheck-ai-health-api-openapi.yml
  format: yaml
  label: EcoCheck Health API
  slug: ecocheck-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-health-api-openapi.yml
- filename: ecocheck-ai-obligation-api-openapi.yml
  format: yaml
  label: EcoCheck Obligation API
  slug: ecocheck-ai-obligation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-obligation-api-openapi.yml
- filename: ecocheck-ai-pricing-api-openapi.yml
  format: yaml
  label: EcoCheck Pricing API
  slug: ecocheck-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-pricing-api-openapi.yml
- filename: ecocheck-ai-regulations-api-openapi.yml
  format: yaml
  label: EcoCheck Regulations API
  slug: ecocheck-ai-regulations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-regulations-api-openapi.yml
- filename: ecocheck-ai-search-api-openapi.yml
  format: yaml
  label: EcoCheck Search API
  slug: ecocheck-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-search-api-openapi.yml
- filename: ecocheck-ai-services-api-openapi.yml
  format: yaml
  label: EcoCheck Services API
  slug: ecocheck-ai-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-services-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ecocheck Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'EcoCheck exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EcoCheck
provider_slug: ecocheck-ai
slug: ecocheck-ai-agentic-access
source_filename: ecocheck-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/ecocheck-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /obligation\n  method: get\n  operationId: checkObligation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cbam/scope\n  method: get\n  operationId: cbamScopeCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cbam/default-value\n  method: get\n  operationId: cbamDefaultValue\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cbam/cost\n  method: get\n  operationId: estimateCbamCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regulations\n  method: get\n  operationId: getRegulations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n\
  \  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles\n  method: get\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{id}\n  method: get\n  operationId: getArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /about\n  method: get\n  operationId: about\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://artifacts.apis.io/ecocheck-ai/agentic-access/ecocheck-ai-agentic-access.yml
summary_line: 12 operations
tags:
- Company
- Greenhouse Gas
- Emissions
- Vietnam
- Software-as-a-Service
- Climate
---
