---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: oxylabs-openapi.yml
  format: yaml
  label: Oxylabs Web Scraper API
  slug: oxylabs-web-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/openapi/oxylabs-openapi.yml
- filename: oxylabs-openapi.yml
  format: yaml
  label: Oxylabs Residential Public API
  slug: oxylabs-residential-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/openapi/oxylabs-openapi.yml
- filename: oxylabs-openapi.yml
  format: yaml
  label: Oxylabs Dashboard API
  slug: oxylabs-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/openapi/oxylabs-openapi.yml
consequence_counts:
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Oxylabs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Oxylabs exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oxylabs
provider_slug: oxylabs
slug: oxylabs-agentic-access
source_filename: oxylabs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/oxylabs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 5\n    connected: 6\n  by_consequence:\n    write: 5\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /queries\n  method: post\n  operationId: submitQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/v1/filters/instances\n  method: get\n  operationId: listStatsFilters\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/v1/usage\n  method: get\n  operationId: getUsageStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login\n  method: post\n  operationId: residentialLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/sub-users\n  method: get\n  operationId: listSubUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/sub-users\n  method: post\n  operationId: createSubUser\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/sub-users/{subUserId}\n  method: get\n  operationId: getSubUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/sub-users/{subUserId}\n  method: patch\n  operationId: updateSubUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/sub-users/{subUserId}\n  method: delete\n  operationId: deleteSubUser\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/sub-users/{subUserId}/target-stats\n  method: get\n  operationId: getSubUserTargetStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/client-stats\n  method: get\n  operationId: getClientStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/agentic-access/oxylabs-agentic-access.yml
summary_line: 11 operations · 5 acting
tags:
- AI Web Scraping
- Bot Mitigation Bypass
- CAPTCHA Solving
- Data Extraction
- Datacenter Proxies
- Datasets
- E-Commerce Data
- Headless Browser
- ISP Proxies
- Mobile Proxies
- Proxies
- Residential Proxies
- SERP
- Scraper API
- Scraping
- Web Data
- Web Intelligence
- Web Unblocker
---
