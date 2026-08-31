---
acting_count: 0
action_class_counts:
  connected: 26
api_specs:
- filename: caplight-companies-api-openapi.yml
  format: yaml
  label: Caplight Companies API
  slug: caplight-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-companies-api-openapi.yml
- filename: caplight-company-api-openapi.yml
  format: yaml
  label: Caplight Company API
  slug: caplight-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-api-openapi.yml
- filename: caplight-company-details-api-openapi.yml
  format: yaml
  label: Caplight Company Details API
  slug: caplight-company-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-details-api-openapi.yml
- filename: caplight-company-filings-api-openapi.yml
  format: yaml
  label: Caplight Company Filings API
  slug: caplight-company-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-filings-api-openapi.yml
- filename: caplight-company-lookup-api-openapi.yml
  format: yaml
  label: Caplight Company Lookup API
  slug: caplight-company-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-company-lookup-api-openapi.yml
- filename: caplight-composite-index-api-openapi.yml
  format: yaml
  label: Caplight Composite Index API
  slug: caplight-composite-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-composite-index-api-openapi.yml
- filename: caplight-comps-api-openapi.yml
  format: yaml
  label: Caplight Comps API
  slug: caplight-comps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-comps-api-openapi.yml
- filename: caplight-fund-marks-api-openapi.yml
  format: yaml
  label: Caplight Fund Marks API
  slug: caplight-fund-marks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-fund-marks-api-openapi.yml
- filename: caplight-funding-rounds-api-openapi.yml
  format: yaml
  label: Caplight Funding Rounds API
  slug: caplight-funding-rounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-funding-rounds-api-openapi.yml
- filename: caplight-investors-api-openapi.yml
  format: yaml
  label: Caplight Investors API
  slug: caplight-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-investors-api-openapi.yml
- filename: caplight-live-orderbook-api-openapi.yml
  format: yaml
  label: Caplight Live Orderbook API
  slug: caplight-live-orderbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-live-orderbook-api-openapi.yml
- filename: caplight-marketprice-api-openapi.yml
  format: yaml
  label: Caplight Market Price API
  slug: caplight-marketprice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-marketprice-api-openapi.yml
- filename: caplight-news-api-openapi.yml
  format: yaml
  label: Caplight News API
  slug: caplight-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-news-api-openapi.yml
- filename: caplight-order-history-api-openapi.yml
  format: yaml
  label: Caplight Order History API
  slug: caplight-order-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-order-history-api-openapi.yml
- filename: caplight-stock-splits-api-openapi.yml
  format: yaml
  label: Caplight Stock Splits API
  slug: caplight-stock-splits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-stock-splits-api-openapi.yml
- filename: caplight-trade-history-api-openapi.yml
  format: yaml
  label: Caplight Trade History API
  slug: caplight-trade-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/openapi/caplight-trade-history-api-openapi.yml
consequence_counts:
  read: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Caplight Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Caplight exposes 26 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Caplight
provider_slug: caplight
slug: caplight-agentic-access
source_filename: caplight-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/caplight-rest-api-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 26\n  by_consequence:\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/companies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/all-with-data\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/all-marketprices\n  method: get\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market-price-history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/live-orderbook\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/quarterly-market-summary\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fund-marks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/news\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trade-history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order-history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market-price-fixed-eod\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stock-splits\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings/cois/all\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/filings/cois/get-download-urls\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings/cois/download-stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/comps-performance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/funding-rounds\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/companies/{companyId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/funding-rounds/updates\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/funding-rounds/{roundId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/comps\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/investors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/composite-index\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/composite-index/sectors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/composite-index/verticals\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caplight/refs/heads/main/agentic-access/caplight-agentic-access.yml
summary_line: 26 operations
tags:
- private-markets
- secondary-market
- Market Data
- venture-capital
- company-data
- investor-data
- funding-rounds
- pricing-data
- Financial Data
- Fintech
- MCP
- agent-native
---
