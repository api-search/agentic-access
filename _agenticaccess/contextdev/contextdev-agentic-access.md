---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 29
api_specs:
- filename: contextdev-brand-intelligence-api-openapi.yml
  format: yaml
  label: Context.dev Brand Intelligence API
  slug: contextdev-brand-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-brand-intelligence-api-openapi.yml
- filename: contextdev-monitors-api-openapi.yml
  format: yaml
  label: Context.dev Monitors API
  slug: contextdev-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-monitors-api-openapi.yml
- filename: contextdev-parsing-api-openapi.yml
  format: yaml
  label: Context.dev Parsing API
  slug: contextdev-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-parsing-api-openapi.yml
- filename: contextdev-people-api-openapi.yml
  format: yaml
  label: Context.dev People API
  slug: contextdev-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-people-api-openapi.yml
- filename: contextdev-utility-api-openapi.yml
  format: yaml
  label: Context.dev Utility API
  slug: contextdev-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-utility-api-openapi.yml
- filename: contextdev-web-extraction-api-openapi.yml
  format: yaml
  label: Context.dev Web Extraction API
  slug: contextdev-web-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-web-extraction-api-openapi.yml
- filename: contextdev-web-scraping-api-openapi.yml
  format: yaml
  label: Context.dev Web Scraping API
  slug: contextdev-web-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-web-scraping-api-openapi.yml
consequence_counts:
  read: 29
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Contextdev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'Context.dev exposes 42 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Context.dev
provider_slug: contextdev
slug: contextdev-agentic-access
source_filename: contextdev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/contextdev-brand-intelligence-api-openapi.yml, openapi/contextdev-monitors-api-openapi.yml,\n  openapi/contextdev-parsing-api-openapi.yml, openapi/contextdev-people-api-openapi.yml, openapi/contextdev-utility-api-openapi.yml,\n  openapi/contextdev-web-extraction-api-openapi.yml, openapi/contextdev-web-scraping-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 29\n    acting: 13\n  by_consequence:\n    read: 29\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /brand/retrieve\n  method: get\n  operationId: getBrandRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/retrieve\n  method: post\n  operationId: postBrandRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/retrieve-by-name\n  method: get\n  operationId: getBrandRetrieveByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/retrieve-by-email\n  method: get\n  operationId: getBrandRetrieveByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/retrieve-by-ticker\n  method: get\n  operationId: getBrandRetrieveByTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/retrieve-by-isin\n\
  \  method: get\n  operationId: getBrandRetrieveByIsin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/transaction_identifier\n  method: get\n  operationId: getBrandTransactionIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/retrieve-simplified\n  method: get\n  operationId: getBrandRetrieveSimplified\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors\n  method: post\n  operationId: createMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /monitors\n  method: get\n  operationId: listMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{monitor_id}\n  method: get\n  operationId: getMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{monitor_id}\n  method: patch\n  operationId: updateMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/{monitor_id}\n  method: delete\n  operationId: deleteMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/{monitor_id}/runs\n  method: get\n  operationId: listMonitorRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{monitor_id}/changes\n  method: get\n  operationId: listMonitorChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/runs\n  method: get\n  operationId: listAccountRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/credit-usage\n  method: get\n  operationId: listMonitorCreditUsage\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/limits\n  method: get\n  operationId: getMonitorLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/changes\n  method: get\n  operationId: listChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/changes/{change_id}\n  method: get\n  operationId: getChange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{monitor_id}/run\n  method: post\n  operationId: runMonitorNow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parse\n  method: post\n  operationId: postParse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/retrieve\n  method: post\n  operationId: postPeopleRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/prefetch\n  method: post\n  operationId: postBrandPrefetch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /brand/prefetch-by-email\n  method: post\n  operationId: postBrandPrefetchByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /utility/prefetch\n  method: post\n  operationId: postUtilityPrefetch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/extract\n  method: post\n  operationId: postWebExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/competitors\n  method: get\n  operationId: getWebCompetitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/styleguide\n  method: get\n  operationId: getWebStyleguide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/fonts\n  method: get\n  operationId: getWebFonts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/naics\n  method: get\n  operationId: getWebNaics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/sic\n  method: get\n  operationId: getWebSic\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/ai/query\n  method: post\n  operationId: postBrandAiQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand/ai/product\n  method: post\n  operationId: postBrandAiProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brand/ai/products\n  method: post\n  operationId: postBrandAiProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /web/scrape/html\n  method: get\n  operationId: getWebScrapeHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/scrape/markdown\n  method: get\n  operationId: getWebScrapeMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/scrape/images\n  method: get\n  operationId: getWebScrapeImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/scrape/sitemap\n  method: get\n  operationId: getWebScrapeSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/crawl\n  method: post\n  operationId:\
  \ postWebCrawl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/search\n  method: post\n  operationId: postWebSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/screenshot\n  method: get\n  operationId: getWebScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/agentic-access/contextdev-agentic-access.yml
summary_line: 42 operations · 13 acting
tags:
- Web Scraping
- Brand Intelligence
- Data Enrichment
- AI Agents
- Web Data
- Classification
- Website Monitoring
- Company Data
- Developer Tools
- A2A
---
