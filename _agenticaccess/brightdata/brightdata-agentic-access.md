---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Web Scraper API
  slug: brightdata-web-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data SERP API
  slug: brightdata-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Web Unlocker API
  slug: brightdata-web-unlocker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Proxy & Zone Management API
  slug: brightdata-proxy-zone-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Datasets API
  slug: brightdata-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Browser API (Scraping Browser)
  slug: brightdata-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Brightdata Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request
operation_count: 8
overview: 'Bright Data exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bright Data
provider_slug: brightdata
slug: brightdata-agentic-access
source_filename: brightdata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/brightdata-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 4\n    connected: 4\n  by_consequence:\n    write: 3\n    read: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /datasets/v3/trigger\n  method: post\n  operationId: triggerCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/v3/scrape\n  method: post\n  operationId: scrapeSynchronous\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/v3/progress/{snapshot_id}\n  method: get\n  operationId: getSnapshotProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/v3/snapshot/{snapshot_id}\n  method: get\n  operationId: getSnapshotData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /request\n  method: post\n  operationId: sendRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zone\n  method: get\n  operationId: getZone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zone\n  method: post\n  operationId: addZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browser_sessions/{session_id}\n  method: get\n  operationId: getBrowserSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/agentic-access/brightdata-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- Web Data
- Web Scraping
- Web Intelligence
- Proxy
- Data Extraction
- SERP
- Web Unlocker
- Datasets
- Data Collection
- Browser Automation
---
