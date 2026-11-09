---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 13
api_specs:
- filename: hydrafetch-com-brand-api-openapi.yml
  format: yaml
  label: hydrafetch-com Brand API
  slug: hydrafetch-com-brand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hydrafetch-com/openapi/hydrafetch-com-brand-api-openapi.yml
- filename: hydrafetch-com-crawl-batch-api-openapi.yml
  format: yaml
  label: hydrafetch-com Crawl & batch API
  slug: hydrafetch-com-crawl-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hydrafetch-com/openapi/hydrafetch-com-crawl-batch-api-openapi.yml
- filename: hydrafetch-com-extract-api-openapi.yml
  format: yaml
  label: hydrafetch-com Extract API
  slug: hydrafetch-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hydrafetch-com/openapi/hydrafetch-com-extract-api-openapi.yml
- filename: hydrafetch-com-feedback-api-openapi.yml
  format: yaml
  label: hydrafetch-com Feedback API
  slug: hydrafetch-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hydrafetch-com/openapi/hydrafetch-com-feedback-api-openapi.yml
- filename: hydrafetch-com-logo-api-openapi.yml
  format: yaml
  label: hydrafetch-com Logo API
  slug: hydrafetch-com-logo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hydrafetch-com/openapi/hydrafetch-com-logo-api-openapi.yml
- filename: hydrafetch-com-media-api-openapi.yml
  format: yaml
  label: hydrafetch-com Media API
  slug: hydrafetch-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hydrafetch-com/openapi/hydrafetch-com-media-api-openapi.yml
- filename: hydrafetch-com-scrape-api-openapi.yml
  format: yaml
  label: hydrafetch-com Scrape API
  slug: hydrafetch-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hydrafetch-com/openapi/hydrafetch-com-scrape-api-openapi.yml
- filename: hydrafetch-com-search-api-openapi.yml
  format: yaml
  label: hydrafetch-com Search API
  slug: hydrafetch-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hydrafetch-com/openapi/hydrafetch-com-search-api-openapi.yml
consequence_counts:
  read: 13
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hydrafetch Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'hydrafetch-com exposes 25 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: hydrafetch-com
provider_slug: hydrafetch-com
slug: hydrafetch-com-agentic-access
source_filename: hydrafetch-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/hydrafetch-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 13\n    acting: 12\n  by_consequence:\n    read: 13\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/web/brand\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/brand\n  method: post\n  operationId: batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/brand/logo\n  method: get\n  operationId: logo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/brand/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/styleguide\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/scrape\n  method: post\n  operationId: scrape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/web/markdown\n  method: post\n  operationId: markdown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/html\n  method: post\n  operationId: html\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/raw-html\n  method: post\n  operationId: rawHtml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/links\n  method: post\n  operationId: links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/structured\n  method: post\n  operationId: structured\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/scrape/{id}\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/images\n  method: post\n  operationId: images\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /v1/web/screenshot\n  method: post\n  operationId: screenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/logo/{domain}\n  method: get\n  operationId: serve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/map\n  method: post\n  operationId: mapUrls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/crawl\n  method: post\n  operationId: startCrawl\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/batch\n  method: post\n  operationId: startBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/crawl/{id}\n  method: get\n  operationId: crawlStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/batch/{id}\n  method: get\n  operationId: batchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/crawl/{id}/deliveries\n  method: get\n  operationId: crawlDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/batch/{id}/deliveries\n  method: get\n  operationId: batchDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/search\n  method: post\n  operationId: run\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/extract\n  method: post\n  operationId: run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/feedback\n  method: post\n  operationId: rateResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/hydrafetch-com/agentic-access/hydrafetch-com-agentic-access.yml
summary_line: 25 operations · 12 acting
tags:
- Web Scraping
- Data Extraction
- Automation
- Markdown
---
