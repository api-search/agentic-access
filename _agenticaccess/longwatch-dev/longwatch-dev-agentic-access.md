---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 4
api_specs:
- filename: longwatch-dev-mcp-api-openapi.yml
  format: yaml
  label: longwatch-dev MCP API
  slug: longwatch-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/longwatch-dev/openapi/longwatch-dev-mcp-api-openapi.yml
- filename: longwatch-dev-website-monitoring-api-openapi.yml
  format: yaml
  label: longwatch-dev website monitoring API
  slug: longwatch-dev-website-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/longwatch-dev/openapi/longwatch-dev-website-monitoring-api-openapi.yml
consequence_counts:
  physical: 7
  read: 4
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Longwatch Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-insider-trades
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-x402-endpoint
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /try
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /watch-insider-trades
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /watch-sec-filings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /watch-x402-endpoint
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /watches/{id}/credits
operation_count: 22
overview: 'longwatch-dev exposes 22 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 11 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: longwatch-dev
provider_slug: longwatch-dev
slug: longwatch-dev-agentic-access
source_filename: longwatch-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/longwatch-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 4\n    acting: 18\n  by_consequence:\n    read: 4\n    write: 11\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /check\n  method: get\n  operationId: get_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check\n  method: post\n  operationId: post_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-web-page\n  method: post\n  operationId: post_check_web_page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch-web-page\n  method: post\n  operationId: post_watch_web_page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-rss-feed\n  method: post\n  operationId: post_check_rss_feed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch-rss-feed\n  method: post\n  operationId: post_watch_rss_feed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-crypto-price\n  method: post\n  operationId: post_check_crypto_price\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch-crypto-price\n  method: post\n  operationId: post_watch_crypto_price\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-sec-filings\n  method: post\n  operationId: post_check_sec_filings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch-sec-filings\n  method: post\n  operationId: post_watch_sec_filings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /check-insider-trades\n  method: post\n  operationId: post_check_insider_trades\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch-insider-trades\n  method: post\n  operationId: post_watch_insider_trades\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-x402-endpoint\n  method: post\n  operationId: post_check_x402_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch-x402-endpoint\n  method: post\n  operationId: post_watch_x402_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watches/{id}/credits\n  method: post\n  operationId: post_watches__id__credits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watches\n  method: post\n  operationId: post_watches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watches/{id}/alerts\n  method: get\n  operationId: get_watches__id__alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demo\n  method: get\n  operationId: get_demo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /try\n  method: post\n  operationId: post_try\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /try/{id}\n  method: get\n  operationId: get_try__id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /watches/{id}\n  method: delete\n  operationId: delete_watches__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/longwatch-dev/agentic-access/longwatch-dev-agentic-access.yml
summary_line: 22 operations · 18 acting
tags:
- Company
- Monitoring
- Artificial Intelligence
- Web
- Finance
---
