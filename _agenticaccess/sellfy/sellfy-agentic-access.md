---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: sellfy-content-api-openapi.yml
  format: yaml
  label: Sellfy Content API
  slug: sellfy-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-content-api-openapi.yml
- filename: sellfy-discovery-api-openapi.yml
  format: yaml
  label: Sellfy Discovery API
  slug: sellfy-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-discovery-api-openapi.yml
- filename: sellfy-feeds-api-openapi.yml
  format: yaml
  label: Sellfy Feeds API
  slug: sellfy-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-feeds-api-openapi.yml
- filename: sellfy-licenses-api-openapi.yml
  format: yaml
  label: Sellfy Licenses API
  slug: sellfy-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-licenses-api-openapi.yml
- filename: sellfy-ping-api-openapi.yml
  format: yaml
  label: Sellfy Ping API
  slug: sellfy-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sellfy/openapi/sellfy-ping-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sellfy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Sellfy exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sellfy
provider_slug: sellfy
slug: sellfy-agentic-access
source_filename: sellfy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/sellfy-api-openapi.json, openapi/sellfy-website-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getOpenApi\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /index.md\n  method: get\n  operationId: getHomepageMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing.md\n  method: get\n  operationId: getPricingMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog.md\n  method: get\n  operationId: getChangelogMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp.md\n  method: get\n  operationId: getMcpMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /sitemap.xml\n  method: get\n  operationId: getSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blog/rss.xml\n  method: get\n  operationId: getBlogRss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog/rss.xml\n  method: get\n  operationId: getChangelogRss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/sellfy/agentic-access/sellfy-agentic-access.yml
summary_line: 10 operations
tags:
- E-Commerce
- Digital Products
- Software-as-a-Service
- Payments
- Creators
---
