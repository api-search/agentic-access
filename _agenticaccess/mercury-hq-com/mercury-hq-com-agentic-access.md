---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: mercury-hq-com-x402-storefront-openapi.yml
  format: yaml
  label: MERCURY x402 Storefront API
  slug: mercury-x402-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury-hq-com/refs/heads/main/openapi/mercury-hq-com-x402-storefront-openapi.yml
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mercury Hq Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'MERCURY exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MERCURY
provider_slug: mercury-hq-com
slug: mercury-hq-com-agentic-access
source_filename: mercury-hq-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/mercury-hq-com-x402-storefront-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /buy/signal\n  method: get\n  operationId: buy_signal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/fetch\n  method: get\n  operationId: buy_web_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/extract\n  method: get\n  operationId: buy_extract\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/markdown\n  method: get\n  operationId: buy_cited_markdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/metadata\n  method: get\n  operationId: buy_cited_metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/links\n  method: get\n  operationId: buy_cited_links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/robots\n  method: get\n  operationId: buy_cited_robots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /buy/diff\n  method: get\n  operationId: buy_cited_diff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/notarize\n  method: get\n  operationId: buy_cited_notarize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/headers\n  method: get\n  operationId: buy_cited_headers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/table\n  method: get\n  operationId: buy_cited_table\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/feed\n  method: get\n  operationId: buy_cited_feed\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/availability\n  method: get\n  operationId: buy_cited_availability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/validate\n  method: get\n  operationId: buy_cited_validate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/batch\n  method: get\n  operationId: buy_cited_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/sitemap\n  method: get\n  operationId: buy_cited_sitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/dns\n  method: get\n  operationId:\
  \ buy_cited_dns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/readability\n  method: get\n  operationId: buy_cited_readability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy/redirect\n  method: get\n  operationId: buy_cited_redirect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercury-hq-com/refs/heads/main/agentic-access/mercury-hq-com-agentic-access.yml
summary_line: 19 operations
tags:
- Company
- Agents
- A2A
- MCP
- x402
- HTTP 402
- Machine Payments
- Web Data
- Web Scraping
- Data Extraction
- Provenance
- Stablecoins
- Artificial Intelligence
---
