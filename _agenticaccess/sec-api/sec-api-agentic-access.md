---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Filing Query API
  slug: sec-api-filing-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Full-Text Search API
  slug: sec-api-full-text-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-asyncapi.yml
  format: yaml
  label: SEC API Filing Stream API
  slug: sec-api-filing-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/asyncapi/sec-api-asyncapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API XBRL-to-JSON Converter API
  slug: sec-api-xbrl-to-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Extractor API
  slug: sec-api-extractor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Insider Trading API
  slug: sec-api-insider-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
- filename: sec-api-openapi.yml
  format: yaml
  label: SEC API Form 13F Holdings API
  slug: sec-api-form-13f-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/openapi/sec-api-openapi.yml
consequence_counts:
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sec Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'SEC API exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SEC API
provider_slug: sec-api
slug: sec-api-agentic-access
source_filename: sec-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sec-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 5\n    connected: 2\n  by_consequence:\n    write: 5\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: queryFilings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /full-text-search\n  method: post\n  operationId: fullTextSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /xbrl-to-json\n  method: get\n  operationId: xbrlToJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extractor\n  method: get\n  operationId: extractFilingSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insider-trading\n  method: post\n  operationId: queryInsiderTrading\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /form-13f/holdings\n\
  \  method: post\n  operationId: query13FHoldings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /form-13f/cover-pages\n  method: post\n  operationId: query13FCoverPages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sec-api/refs/heads/main/agentic-access/sec-api-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- SEC Filings
- Regulatory Filings
- EDGAR
- Financial Data
- Compliance
- Government Reports
- Insider Trading
- 13F
- XBRL
- Full-Text Search
---
