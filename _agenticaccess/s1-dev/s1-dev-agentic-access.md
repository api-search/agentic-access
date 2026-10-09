---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: s1-dev-account-api-openapi.yml
  format: yaml
  label: Search1API Account API
  slug: s1-dev-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-account-api-openapi.yml
- filename: s1-dev-crawl-api-openapi.yml
  format: yaml
  label: Search1API Crawl API
  slug: s1-dev-crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-crawl-api-openapi.yml
- filename: s1-dev-feedback-api-openapi.yml
  format: yaml
  label: Search1API Feedback API
  slug: s1-dev-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-feedback-api-openapi.yml
- filename: s1-dev-screenshot-api-openapi.yml
  format: yaml
  label: Search1API Screenshot API
  slug: s1-dev-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-screenshot-api-openapi.yml
- filename: s1-dev-search-api-openapi.yml
  format: yaml
  label: Search1API Search API
  slug: s1-dev-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-search-api-openapi.yml
- filename: s1-dev-system-api-openapi.yml
  format: yaml
  label: Search1API System API
  slug: s1-dev-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-system-api-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: S1 Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Search1API exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Search1API
provider_slug: s1-dev
slug: s1-dev-agentic-access
source_filename: s1-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/s1-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 6\n    connected: 7\n  by_consequence:\n    write: 6\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /feedback\n  method: post\n  operationId: feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screenshot\n  method: post\n  operationId: screenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news\n  method: post\n  operationId: news\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: post\n  operationId: ask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crawl\n  method: post\n  operationId: crawl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sitemap\n  method: post\n  operationId: sitemap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trending\n  method: post\n  operationId: trending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extract\n  method: post\n  operationId: extract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /deepcrawl\n  method: post\n  operationId: deepcrawl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deepcrawl/status/{taskId}\n  method: get\n  operationId: deepcrawlStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/agentic-access/s1-dev-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Company
- Search
- Web Search
- Crawling
- Web Scraping
- News
- AI Agents
- MCP
- Agent Tools
- Data Extraction
- Screenshots
---
