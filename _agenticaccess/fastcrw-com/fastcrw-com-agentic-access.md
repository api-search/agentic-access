---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
api_specs:
- filename: fastcrw-com-batch-api-openapi.yml
  format: yaml
  label: fastcrw-com Batch API
  slug: fastcrw-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastcrw-com/openapi/fastcrw-com-batch-api-openapi.yml
- filename: fastcrw-com-capabilities-api-openapi.yml
  format: yaml
  label: fastcrw-com Capabilities API
  slug: fastcrw-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastcrw-com/openapi/fastcrw-com-capabilities-api-openapi.yml
- filename: fastcrw-com-change-tracking-api-openapi.yml
  format: yaml
  label: fastcrw-com Change Tracking API
  slug: fastcrw-com-change-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastcrw-com/openapi/fastcrw-com-change-tracking-api-openapi.yml
- filename: fastcrw-com-crawl-api-openapi.yml
  format: yaml
  label: fastcrw-com Crawl API
  slug: fastcrw-com-crawl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastcrw-com/openapi/fastcrw-com-crawl-api-openapi.yml
- filename: fastcrw-com-extract-api-openapi.yml
  format: yaml
  label: fastcrw-com Extract API
  slug: fastcrw-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastcrw-com/openapi/fastcrw-com-extract-api-openapi.yml
- filename: fastcrw-com-map-api-openapi.yml
  format: yaml
  label: fastcrw-com Map API
  slug: fastcrw-com-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastcrw-com/openapi/fastcrw-com-map-api-openapi.yml
- filename: fastcrw-com-scrape-api-openapi.yml
  format: yaml
  label: fastcrw-com Scrape API
  slug: fastcrw-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastcrw-com/openapi/fastcrw-com-scrape-api-openapi.yml
- filename: fastcrw-com-search-api-openapi.yml
  format: yaml
  label: fastcrw-com Search API
  slug: fastcrw-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastcrw-com/openapi/fastcrw-com-search-api-openapi.yml
consequence_counts:
  read: 5
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fastcrw Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'fastcrw-com exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: fastcrw-com
provider_slug: fastcrw-com
slug: fastcrw-com-agentic-access
source_filename: fastcrw-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/fastcrw-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 5\n    acting: 8\n  by_consequence:\n    read: 5\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrape\n  method: post\n  operationId: scrape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/map\n  method: post\n  operationId: map\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crawl\n  method: post\n  operationId: crawlStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crawl/{id}\n  method: get\n  operationId: crawlStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/scrape\n  method: post\n \
  \ operationId: batchScrapeStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/scrape/{id}\n  method: get\n  operationId: batchScrapeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/scrape/{id}\n  method: delete\n  operationId: batchScrapeCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/change-tracking/diff\n  method: post\n  operationId: changeTrackingDiff\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/capabilities\n  method: get\n  operationId: capabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/extract\n  method: post\n  operationId: extractStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extract/{id}\n  method: get\n  operationId: extractStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v1/extract/{id}\n  method: delete\n  operationId: extractCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/fastcrw-com/agentic-access/fastcrw-com-agentic-access.yml
summary_line: 13 operations · 8 acting
tags:
- Company
- Web Scraping
- AI Agents
- Rust
- Open Source
- SERP
---
