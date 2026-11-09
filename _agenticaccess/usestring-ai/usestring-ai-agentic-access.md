---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 29
api_specs:
- filename: usestring-ai-browser-api-openapi.yml
  format: yaml
  label: usestring-ai Browser API
  slug: usestring-ai-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-browser-api-openapi.yml
- filename: usestring-ai-builds-api-openapi.yml
  format: yaml
  label: usestring-ai Builds API
  slug: usestring-ai-builds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-builds-api-openapi.yml
- filename: usestring-ai-contexts-api-openapi.yml
  format: yaml
  label: usestring-ai Contexts API
  slug: usestring-ai-contexts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-contexts-api-openapi.yml
- filename: usestring-ai-documentation-api-openapi.yml
  format: yaml
  label: usestring-ai Documentation API
  slug: usestring-ai-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-documentation-api-openapi.yml
- filename: usestring-ai-feeds-api-openapi.yml
  format: yaml
  label: usestring-ai Feeds API
  slug: usestring-ai-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-feeds-api-openapi.yml
- filename: usestring-ai-fetch-api-openapi.yml
  format: yaml
  label: usestring-ai Fetch API
  slug: usestring-ai-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-fetch-api-openapi.yml
- filename: usestring-ai-search-api-openapi.yml
  format: yaml
  label: usestring-ai Search API
  slug: usestring-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-search-api-openapi.yml
- filename: usestring-ai-sessions-api-openapi.yml
  format: yaml
  label: usestring-ai Sessions API
  slug: usestring-ai-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-sessions-api-openapi.yml
- filename: usestring-ai-sitemap-api-openapi.yml
  format: yaml
  label: usestring-ai Sitemap API
  slug: usestring-ai-sitemap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usestring-ai/openapi/usestring-ai-sitemap-api-openapi.yml
consequence_counts:
  physical: 1
  read: 29
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Usestring Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/builds/{id}/messages
operation_count: 47
overview: 'String exposes 47 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 17 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: String
provider_slug: usestring-ai
slug: usestring-ai-agentic-access
source_filename: usestring-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/feedbuilder-usestring-ai-openapi.yaml, openapi/request-usestring-ai-openapi.json,\n  openapi/usestring-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 29\n    acting: 18\n  by_consequence:\n    read: 29\n    write: 17\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /docs\n  method: get\n  operationId: getDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.yaml\n  method: get\n  operationId: getOpenAPIDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/builds\n  method: get\n  operationId: listBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/builds\n  method: post\n  operationId: createBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/builds/{id}\n  method: delete\n  operationId: deleteBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/builds/{id}\n  method: get\n\
  \  operationId: getBuild\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/builds/{id}\n  method: patch\n  operationId: updateBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/builds/{id}/cancel\n  method: post\n  operationId: cancelBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/builds/{id}/events\n  method: get\n  operationId: streamBuild\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/builds/{id}/gates/{gate_id}\n  method: post\n  operationId: answerGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/builds/{id}/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/builds/{id}/sample\n  method: get\n  operationId: getSample\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feeds\n  method: get\n  operationId: listFeeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feeds/{feed}/data\n  method: get\n  operationId: getFeedData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feeds/{feed}/download\n  method: get\n  operationId: downloadFeedObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fetch\n  method: post\n  operationId: fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap\n  method: post\n  operationId: createSitemapJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sitemap\n  method: get\n  operationId: listSitemapJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap/{jobId}\n  method: get\n  operationId: getSitemapJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap/{jobId}\n  method: delete\n  operationId: cancelSitemapJob\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sitemap/{jobId}/approve\n  method: post\n  operationId: approveSitemapJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sitemap/{jobId}/urls\n  method: get\n  operationId: getSitemapUrls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contexts\n  method: post\n  operationId: createBrowserContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contexts\n  method: get\n  operationId: listBrowserContexts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contexts/{contextId}\n  method: get\n  operationId: getBrowserContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contexts/{contextId}\n  method: delete\n  operationId: deleteBrowserContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n\
  \  method: post\n  operationId: createBrowserSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: get\n  operationId: listBrowserSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}\n  method: get\n  operationId: getBrowserSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/replay\n  method: get\n  operationId: getBrowserSessionReplay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /sessions/{sessionId}/files\n  method: get\n  operationId: listBrowserSessionFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/files/{name}\n  method: put\n  operationId: putBrowserSessionFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{sessionId}/files/{name}\n  method: get\n  operationId: getBrowserSessionFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fetch\n  method: post\n  operationId: fetchUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: searchWeb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap\n  method: post\n  operationId: createSitemapJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sitemap\n  method: get\n  operationId: listSitemapJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap/{jobId}/approve\n  method: post\n  operationId: approveSitemapJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sitemap/{jobId}\n  method: get\n  operationId: getSitemapJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap/{jobId}\n  method: delete\n  operationId: cancelSitemapJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sitemap/{jobId}/urls\n  method: get\n  operationId: listSitemapJobUrls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contexts\n\
  \  method: post\n  operationId: createBrowserContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contexts\n  method: get\n  operationId: listBrowserContexts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contexts/{contextId}\n  method: get\n  operationId: getBrowserContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contexts/{contextId}\n  method: delete\n  operationId: deleteBrowserContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wss\n  method: get\n  operationId: connectBrowser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/usestring-ai/agentic-access/usestring-ai-agentic-access.yml
summary_line: 47 operations · 18 acting
tags:
- Web Scraping
- Data Extraction
- Markdown
- JSON
---
