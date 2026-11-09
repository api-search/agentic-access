---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: cefradar-com-account-api-openapi.yml
  format: yaml
  label: CEF Radar Account API
  slug: cefradar-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-account-api-openapi.yml
- filename: cefradar-com-events-api-openapi.yml
  format: yaml
  label: CEF Radar Events API
  slug: cefradar-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-events-api-openapi.yml
- filename: cefradar-com-funds-api-openapi.yml
  format: yaml
  label: CEF Radar Funds API
  slug: cefradar-com-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-funds-api-openapi.yml
- filename: cefradar-com-investors-api-openapi.yml
  format: yaml
  label: CEF Radar Investors API
  slug: cefradar-com-investors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-investors-api-openapi.yml
- filename: cefradar-com-search-api-openapi.yml
  format: yaml
  label: CEF Radar Search API
  slug: cefradar-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cefradar-com/openapi/cefradar-com-search-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cefradar Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'CEF Radar exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CEF Radar
provider_slug: cefradar-com
slug: cefradar-com-agentic-access
source_filename: cefradar-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cefradar-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/campaigns\n  method: get\n  operationId: list_campaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activists\n  method: get\n  operationId: list_activists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activists/{slug}\n  method: get\n  operationId:\
  \ get_activist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds\n  method: get\n  operationId: list_funds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds/{ticker}\n  method: get\n  operationId: get_fund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds/{ticker}/facts\n  method: get\n  operationId: get_fund_facts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds/{ticker}/holdings\n  method: get\n  operationId: get_fund_holdings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds/{ticker}/events\n  method: get\n  operationId: get_fund_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events\n  method: get\n  operationId: list_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  operationId: search_funds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/holdings/search\n  method: get\n  operationId: search_holdings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/filings\n  method: get\n  operationId: list_filings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/filings/{accession}\n  method: get\n  operationId: get_filing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cefradar-com/agentic-access/cefradar-com-agentic-access.yml
summary_line: 14 operations
tags:
- Closed‑end funds
- SEC Filings
- Investor alerts
- Fund activity
- Buybacks
---
