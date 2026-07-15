---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 7
api_specs:
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Crawling API
  slug: crawlbase-crawling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Scraper API
  slug: crawlbase-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Cloud Storage API
  slug: crawlbase-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Screenshots API
  slug: crawlbase-screenshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Leads API
  slug: crawlbase-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
consequence_counts:
  read: 7
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crawlbase Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Crawlbase exposes 11 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crawlbase
provider_slug: crawlbase
slug: crawlbase-agentic-access
source_filename: crawlbase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/crawlbase-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 7\n    acting: 4\n  by_consequence:\n    read: 7\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: crawl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: crawlPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /scraper\n  method: get\n  operationId: scrape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage\n  method: get\n  operationId: getStoredPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage\n  method: delete\n  operationId: deleteStoredPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/bulk\n  method: post\n  operationId: getStoredPagesBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/bulk_delete\n  method: post\n  operationId: deleteStoredPagesBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/rids\n  method: get\n  operationId: listStoredRids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/total_count\n  method: get\n  operationId: getStoredTotalCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screenshots\n  method: get\n\
  \  operationId: screenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: get\n  operationId: getLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/agentic-access/crawlbase-agentic-access.yml
summary_line: 11 operations · 4 acting
tags:
- Web Scraping
- Web Crawling
- Web Intelligence
- Data Extraction
- Proxy
- Scraper API
- Data Collection
- SERP
- Web Data
---
