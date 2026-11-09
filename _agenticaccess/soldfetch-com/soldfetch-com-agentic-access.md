---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 10
api_specs:
- filename: soldfetch-com-bulk-search-api-openapi.yml
  format: yaml
  label: soldfetch-com Bulk Search API
  slug: soldfetch-com-bulk-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldfetch-com/openapi/soldfetch-com-bulk-search-api-openapi.yml
- filename: soldfetch-com-capabilities-api-openapi.yml
  format: yaml
  label: soldfetch-com Capabilities API
  slug: soldfetch-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldfetch-com/openapi/soldfetch-com-capabilities-api-openapi.yml
- filename: soldfetch-com-item-api-openapi.yml
  format: yaml
  label: soldfetch-com Item API
  slug: soldfetch-com-item-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldfetch-com/openapi/soldfetch-com-item-api-openapi.yml
- filename: soldfetch-com-public-api-openapi.yml
  format: yaml
  label: soldfetch-com Public API
  slug: soldfetch-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldfetch-com/openapi/soldfetch-com-public-api-openapi.yml
- filename: soldfetch-com-rapidapi-api-openapi.yml
  format: yaml
  label: soldfetch-com Rapidapi API
  slug: soldfetch-com-rapidapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldfetch-com/openapi/soldfetch-com-rapidapi-api-openapi.yml
- filename: soldfetch-com-requests-api-openapi.yml
  format: yaml
  label: soldfetch-com Requests API
  slug: soldfetch-com-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldfetch-com/openapi/soldfetch-com-requests-api-openapi.yml
- filename: soldfetch-com-scrape-api-openapi.yml
  format: yaml
  label: soldfetch-com Scrape API
  slug: soldfetch-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldfetch-com/openapi/soldfetch-com-scrape-api-openapi.yml
- filename: soldfetch-com-usage-api-openapi.yml
  format: yaml
  label: soldfetch-com Usage API
  slug: soldfetch-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldfetch-com/openapi/soldfetch-com-usage-api-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Soldfetch Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/scrape/max
operation_count: 13
overview: 'soldfetch-com exposes 13 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: soldfetch-com
provider_slug: soldfetch-com
slug: soldfetch-com-agentic-access
source_filename: soldfetch-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/soldfetch-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 10\n    acting: 3\n  by_consequence:\n    read: 10\n    physical: 1\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/scrape\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrape/category\n  method: get\n  operationId: category\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/item/{itemId}\n \
  \ method: get\n  operationId: product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/scrape\n  method: get\n  operationId: searchAlias0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rapidapi/scrape-ebay\n  method: get\n  operationId: searchAlias1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /requests\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrape/max\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scrape/max/results/{jobId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrape/max/{jobId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scrape/max/{jobId}/download.csv\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bulk-search\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/soldfetch-com/agentic-access/soldfetch-com-agentic-access.yml
summary_line: 13 operations · 3 acting
tags:
- Company
- eBay
- Listings
- Pricing
- Reseller
---
