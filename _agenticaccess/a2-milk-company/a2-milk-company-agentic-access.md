---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: a2-milk-company-article-listing-api-openapi.yml
  format: yaml
  label: The a2 Milk Company Article Listing API
  slug: a2-milk-company-article-listing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-milk-company/refs/heads/main/openapi/a2-milk-company-article-listing-api-openapi.yml
- filename: a2-milk-company-health-api-openapi.yml
  format: yaml
  label: The a2 Milk Company Health API
  slug: a2-milk-company-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-milk-company/refs/heads/main/openapi/a2-milk-company-health-api-openapi.yml
- filename: a2-milk-company-llms-full-txt-api-openapi.yml
  format: yaml
  label: The a2 Milk Company Llms Full.txt API
  slug: a2-milk-company-llms-full-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-milk-company/refs/heads/main/openapi/a2-milk-company-llms-full-txt-api-openapi.yml
- filename: a2-milk-company-llms-txt-api-openapi.yml
  format: yaml
  label: The a2 Milk Company Llms.txt API
  slug: a2-milk-company-llms-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-milk-company/refs/heads/main/openapi/a2-milk-company-llms-txt-api-openapi.yml
- filename: a2-milk-company-recipe-listing-api-openapi.yml
  format: yaml
  label: The a2 Milk Company Recipe Listing API
  slug: a2-milk-company-recipe-listing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-milk-company/refs/heads/main/openapi/a2-milk-company-recipe-listing-api-openapi.yml
- filename: a2-milk-company-search-api-openapi.yml
  format: yaml
  label: The a2 Milk Company Search API
  slug: a2-milk-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-milk-company/refs/heads/main/openapi/a2-milk-company-search-api-openapi.yml
- filename: a2-milk-company-sitemap-xml-api-openapi.yml
  format: yaml
  label: The a2 Milk Company Sitemap.xml API
  slug: a2-milk-company-sitemap-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-milk-company/refs/heads/main/openapi/a2-milk-company-sitemap-xml-api-openapi.yml
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: A2 Milk Company Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'The a2 Milk Company exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The a2 Milk Company
provider_slug: a2-milk-company
slug: a2-milk-company-agentic-access
source_filename: a2-milk-company-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/a2-milk-company-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 1\n    connected: 6\n  by_consequence:\n    write: 1\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/search\n  method: put\n  operationId: searchSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/article-listing\n  method: post\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recipe-listing\n  method: post\n  operationId: listRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  operationId: getSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a2-milk-company/refs/heads/main/agentic-access/a2-milk-company-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Company
- Dairy
- Food and Beverage
- Nutrition
- Infant Formula
- Consumer Goods
- ASX Listed
- New Zealand
---
