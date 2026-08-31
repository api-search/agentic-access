---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: scrapingant-scraping-api-openapi.yml
  format: yaml
  label: ScrapingAnt Scraping API
  slug: scrapingant-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/openapi/scrapingant-scraping-api-openapi.yml
- filename: scrapingant-usage-api-openapi.yml
  format: yaml
  label: ScrapingAnt Usage API
  slug: scrapingant-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/openapi/scrapingant-usage-api-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scrapingant Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'ScrapingAnt exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ScrapingAnt
provider_slug: scrapingant
slug: scrapingant-agentic-access
source_filename: scrapingant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: generated\nsource: openapi/scrapingant-scraping-api-openapi.yml, openapi/scrapingant-usage-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/general\n  method: post\n  operationId: scrapingant_general_request_v2_general_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/general\n  method: get\n  operationId:\
  \ scrapingant_general_request_v2_general_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/general\n  method: put\n  operationId: scrapingant_general_request_v2_general_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/general\n  method: patch\n  operationId: scrapingant_general_request_v2_general_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/general\n  method: delete\n  operationId: scrapingant_general_request_v2_general_delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/usage\n  method: get\n  operationId: scrapingant_usage_v2_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/agentic-access/scrapingant-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Data Extraction
- Proxies
- Scraping
- Web Scraping
- Headless Browsers
- AI Agents
- MCP
- LLM
- Data Collection
- Web Data
---
