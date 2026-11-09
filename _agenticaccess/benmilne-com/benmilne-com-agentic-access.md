---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 15
api_specs:
- filename: benmilne-com-ask-api-openapi.yml
  format: yaml
  label: Ben Milne Ask API
  slug: benmilne-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-ask-api-openapi.yml
- filename: benmilne-com-batch-api-openapi.yml
  format: yaml
  label: Ben Milne Batch API
  slug: benmilne-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-batch-api-openapi.yml
- filename: benmilne-com-categories-api-openapi.yml
  format: yaml
  label: Ben Milne Categories API
  slug: benmilne-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-categories-api-openapi.yml
- filename: benmilne-com-contact-api-openapi.yml
  format: yaml
  label: Ben Milne Contact API
  slug: benmilne-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-contact-api-openapi.yml
- filename: benmilne-com-languages-api-openapi.yml
  format: yaml
  label: Ben Milne Languages API
  slug: benmilne-com-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-languages-api-openapi.yml
- filename: benmilne-com-mcp-api-openapi.yml
  format: yaml
  label: Ben Milne MCP API
  slug: benmilne-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-mcp-api-openapi.yml
- filename: benmilne-com-posts-api-openapi.yml
  format: yaml
  label: Ben Milne Posts API
  slug: benmilne-com-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-posts-api-openapi.yml
- filename: benmilne-com-products-api-openapi.yml
  format: yaml
  label: Ben Milne Products API
  slug: benmilne-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-products-api-openapi.yml
- filename: benmilne-com-search-api-openapi.yml
  format: yaml
  label: Ben Milne Search API
  slug: benmilne-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-search-api-openapi.yml
- filename: benmilne-com-site-api-openapi.yml
  format: yaml
  label: Ben Milne Site API
  slug: benmilne-com-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-site-api-openapi.yml
- filename: benmilne-com-status-api-openapi.yml
  format: yaml
  label: Ben Milne Status API
  slug: benmilne-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-status-api-openapi.yml
- filename: benmilne-com-stream-api-openapi.yml
  format: yaml
  label: Ben Milne Stream API
  slug: benmilne-com-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-stream-api-openapi.yml
- filename: benmilne-com-tags-api-openapi.yml
  format: yaml
  label: Ben Milne Tags API
  slug: benmilne-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-tags-api-openapi.yml
- filename: benmilne-com-graph-ql-api-openapi.yml
  format: yaml
  label: Ben Milne Graph QL API
  slug: benmilne-com-graph-ql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/benmilne-com/openapi/benmilne-com-graph-ql-api-openapi.yml
consequence_counts:
  physical: 1
  read: 15
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Benmilne Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contact/send
operation_count: 19
overview: 'Ben Milne exposes 19 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ben Milne
provider_slug: benmilne-com
slug: benmilne-com-agentic-access
source_filename: benmilne-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/benmilne-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 15\n    acting: 4\n  by_consequence:\n    read: 15\n    write: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/languages\n  method: get\n  operationId: listLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/site\n  method: get\n  operationId: getSiteInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/posts\n  method:\
  \ get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/posts/{slug}\n  method: get\n  operationId: getPostBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: get\n  operationId: searchPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/categories/{slug}\n  method: get\n  operationId: listPostsByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tags/{slug}\n  method: get\n  operationId: listPostsByTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/v1/posts\n  method: get\n  operationId: mcpListPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/v1/search\n  method: get\n  operationId: mcpSearchPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/the-value-layer\n  method: get\n  operationId: getValueLayerProduct\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stream/search\n  method: get\n  operationId: streamSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: post\n  operationId: nlwebAsk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/batch\n  method: post\n  operationId: batchApiCalls\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/send\n  method: post\n  operationId: sendContactMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: graphqlQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: get\n  operationId:\
  \ graphqlIntrospection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/benmilne-com/agentic-access/benmilne-com-agentic-access.yml
summary_line: 19 operations · 4 acting
tags:
- Personal
- Blog
- Fintech
- Payments
- Value-Design
---
