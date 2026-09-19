---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: hyperice-collections-api-openapi.yml
  format: yaml
  label: Hyperice Collections API
  slug: hyperice-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/openapi/hyperice-collections-api-openapi.yml
- filename: hyperice-discovery-api-openapi.yml
  format: yaml
  label: Hyperice Discovery API
  slug: hyperice-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/openapi/hyperice-discovery-api-openapi.yml
- filename: hyperice-products-api-openapi.yml
  format: yaml
  label: Hyperice Products API
  slug: hyperice-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/openapi/hyperice-products-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hyperice Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Hyperice exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hyperice
provider_slug: hyperice
slug: hyperice-agentic-access
source_filename: hyperice-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/hyperice-collections-api-openapi.yml, openapi/hyperice-discovery-api-openapi.yml,\n  openapi/hyperice-products-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /collections.json\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{handle}/products.json\n  method: get\n  operationId: listCollectionProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  operationId: getSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents.md\n  method: get\n  operationId: getAgentsMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ucp\n  method: get\n  operationId: getUcpProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products.json\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{handle}.json\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperice/refs/heads/main/agentic-access/hyperice-agentic-access.yml
summary_line: 8 operations
tags:
- Company
- Commerce
- Retail
- Health and Wellness
- Consumer Hardware
- Sports And Fitness
- Agentic Commerce
- GraphQL
- MCP
- Shopify
---
