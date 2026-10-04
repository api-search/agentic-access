---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 32
api_specs:
- filename: hyperbrowser-sessions-api-openapi.yml
  format: yaml
  label: Hyperbrowser Sessions API
  slug: sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-sessions-api-openapi.yml
- filename: hyperbrowser-profiles-api-openapi.yml
  format: yaml
  label: Hyperbrowser Profiles API
  slug: profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-profiles-api-openapi.yml
- filename: hyperbrowser-scrape-api-openapi.yml
  format: yaml
  label: Hyperbrowser Scrape API
  slug: scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-scrape-api-openapi.yml
- filename: hyperbrowser-crawl-api-openapi.yml
  format: yaml
  label: Hyperbrowser Crawl API
  slug: crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-crawl-api-openapi.yml
- filename: hyperbrowser-extract-api-openapi.yml
  format: yaml
  label: Hyperbrowser Extract API
  slug: extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-extract-api-openapi.yml
- filename: hyperbrowser-extensions-api-openapi.yml
  format: yaml
  label: Hyperbrowser Extensions API
  slug: extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-extensions-api-openapi.yml
- filename: hyperbrowser-web-api-openapi.yml
  format: yaml
  label: Hyperbrowser Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-web-api-openapi.yml
- filename: hyperbrowser-profile-api-openapi.yml
  format: yaml
  label: Hyperbrowser Profile API
  slug: hyperbrowser-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-profile-api-openapi.yml
- filename: hyperbrowser-session-api-openapi.yml
  format: yaml
  label: Hyperbrowser Session API
  slug: hyperbrowser-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-session-api-openapi.yml
- filename: hyperbrowser-task-api-openapi.yml
  format: yaml
  label: Hyperbrowser Task API
  slug: hyperbrowser-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-task-api-openapi.yml
- filename: hyperbrowser-x402-api-openapi.yml
  format: yaml
  label: Hyperbrowser X402 API
  slug: hyperbrowser-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-x402-api-openapi.yml
consequence_counts:
  read: 32
  safety-critical: 6
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Hyperbrowser Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/session/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/task/browser-use/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/task/claude-computer-use/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/task/cua/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/task/gemini-computer-use/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/task/hyper-agent/{id}/stop
operation_count: 54
overview: 'Hyperbrowser exposes 54 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 16 write, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hyperbrowser
provider_slug: hyperbrowser
slug: hyperbrowser-agentic-access
source_filename: hyperbrowser-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/hyperbrowser-crawl-api-openapi.yml, openapi/hyperbrowser-extensions-api-openapi.yml,\n  openapi/hyperbrowser-extract-api-openapi.yml, openapi/hyperbrowser-profile-api-openapi.yml,\n  openapi/hyperbrowser-profiles-api-openapi.yml, openapi/hyperbrowser-scrape-api-openapi.yml,\n  openapi/hyperbrowser-session-api-openapi.yml, openapi/hyperbrowser-sessions-api-openapi.yml,\n  openapi/hyperbrowser-task-api-openapi.yml, openapi/hyperbrowser-web-api-openapi.yml, openapi/hyperbrowser-x402-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    acting: 22\n    connected: 32\n  by_consequence:\n    write: 16\n    read: 32\n    safety-critical: 6\n  human_in_the_loop_required:\
  \ 6\noperations:\n- path: /api/crawl\n  method: post\n  operationId: postApiCrawl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/crawl/{id}\n  method: get\n  operationId: getApiCrawlById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/crawl/{id}/status\n  method: get\n  operationId: getApiCrawlByIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extensions/add\n  method: post\n  operationId: postApiExtensionsAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extensions/list\n  method: get\n  operationId: getApiExtensionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extract\n  method: post\n  operationId: postApiExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/extract/{id}\n  method: get\n  operationId: getApiExtractById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extract/{id}/status\n  method:\
  \ get\n  operationId: getApiExtractByIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profile\n  method: post\n  operationId: postApiProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profile/{id}\n  method: get\n  operationId: getApiProfileById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profile/{id}\n  method: delete\n  operationId: deleteApiProfileById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profiles\n  method: get\n  operationId: getApiProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/scrape\n  method: post\n  operationId: postApiScrape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scrape/{id}\n  method: get\n  operationId: getApiScrapeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/scrape/{id}/status\n  method: get\n  operationId: getApiScrapeByIdStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/scrape/batch\n  method: post\n  operationId: postApiScrapeBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scrape/batch/{id}\n  method: get\n  operationId: getApiScrapeBatchById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/scrape/batch/{id}/status\n  method: get\n  operationId: getApiScrapeBatchByIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/session\n  method: post\n  operationId:\
  \ postApiSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/session/{id}\n  method: get\n  operationId: getApiSessionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/session/{id}/stop\n  method: put\n  operationId: putApiSessionByIdStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/session/{id}/update\n  method: put\n  operationId: putApiSessionByIdUpdate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/session/{id}/captcha/evaluate\n  method: post\n  operationId: postApiSessionByIdCaptchaEvaluate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/session/{id}/recording-url\n  method: get\n  operationId: getApiSessionByIdRecordingUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/session/{id}/video-recording-url\n  method: get\n  operationId: getApiSessionByIdVideoRecordingUrl\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/session/{id}/downloads-url\n  method: get\n  operationId: getApiSessionByIdDownloadsUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sessions\n  method: get\n  operationId: getApiSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/hyper-agent\n  method: post\n  operationId: postApiTaskHyperAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/task/hyper-agent/{id}\n\
  \  method: get\n  operationId: getApiTaskHyperAgentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/hyper-agent/{id}/stop\n  method: put\n  operationId: putApiTaskHyperAgentByIdStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/task/hyper-agent/{id}/status\n  method: get\n  operationId: getApiTaskHyperAgentByIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/browser-use\n  method: post\n  operationId: postApiTaskBrowserUse\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/task/browser-use/{id}\n  method: get\n  operationId: getApiTaskBrowserUseById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/browser-use/{id}/stop\n  method: put\n  operationId: putApiTaskBrowserUseByIdStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/task/browser-use/{id}/status\n  method: get\n  operationId: getApiTaskBrowserUseByIdStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/claude-computer-use\n  method: post\n  operationId: postApiTaskClaudeComputerUse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/task/claude-computer-use/{id}\n  method: get\n  operationId: getApiTaskClaudeComputerUseById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/claude-computer-use/{id}/stop\n  method: put\n  operationId: putApiTaskClaudeComputerUseByIdStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/task/claude-computer-use/{id}/status\n  method: get\n  operationId: getApiTaskClaudeComputerUseByIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/gemini-computer-use\n  method: post\n  operationId: postApiTaskGeminiComputerUse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/task/gemini-computer-use/{id}\n  method: get\n  operationId: getApiTaskGeminiComputerUseById\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/gemini-computer-use/{id}/stop\n  method: put\n  operationId: putApiTaskGeminiComputerUseByIdStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/task/gemini-computer-use/{id}/status\n  method: get\n  operationId: getApiTaskGeminiComputerUseByIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/cua\n  method: post\n  operationId: postApiTaskCua\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/task/cua/{id}\n  method: get\n  operationId: getApiTaskCuaById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/task/cua/{id}/stop\n  method: put\n  operationId: putApiTaskCuaByIdStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/task/cua/{id}/status\n  method: get\n  operationId: getApiTaskCuaByIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/web/fetch\n \
  \ method: post\n  operationId: postApiWebFetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/web/search\n  method: post\n  operationId: postApiWebSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/web/crawl\n  method: post\n  operationId: postApiWebCrawl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/web/crawl/{id}\n  method: get\n  operationId: getApiWebCrawlById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/web/crawl/{id}/status\n\
  \  method: get\n  operationId: getApiWebCrawlByIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/web/fetch\n  method: post\n  operationId: postX402WebFetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/web/search\n  method: post\n  operationId: postX402WebSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/agentic-access/hyperbrowser-agentic-access.yml
summary_line: 54 operations · 22 acting · 6 human-in-the-loop
tags:
- Headless Browser
- Browser Infrastructure
- Web Scraping
- Web Crawling
- Data Extraction
- AI Agents
- Browser Automation
- Computer Use
- Stealth
- Proxies
- CAPTCHA Solving
- MCP
- HyperAgent
- x402
---
