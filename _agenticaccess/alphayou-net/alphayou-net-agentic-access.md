---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 12
api_specs:
- filename: alphayou-net-alphayou-api-openapi.yml
  format: yaml
  label: alphayou-net Alpha You API
  slug: alphayou-net-alphayou-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphayou-net/openapi/alphayou-net-alphayou-api-openapi.yml
consequence_counts:
  read: 12
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Alphayou Net Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'alphayou-net exposes 13 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: alphayou-net
provider_slug: alphayou-net
slug: alphayou-net-agentic-access
source_filename: alphayou-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/alphayou-net-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 12\n    acting: 1\n  by_consequence:\n    read: 12\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/mcp/whoami\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/mcp\n  method: post\n  operationId: mcp_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/signals/alpha\n  method: get\n  operationId: alphayou_track_record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/signals/recent\n  method: get\n  operationId: alphayou_calls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets\n  method: get\n  operationId: alphayou_search_datasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds\n  method: get\n  operationId: alphayou_funds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tickers/{symbol}/disclosures\n\
  \  method: get\n  operationId: alphayou_company_disclosures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insiders/trades\n  method: get\n  operationId: alphayou_insider_trades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insiders/clusters\n  method: get\n  operationId: alphayou_insider_clusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds/{cik}/holdings\n  method: get\n  operationId: alphayou_fund_holdings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds/{cik}/changes\n  method: get\n  operationId: alphayou_fund_changes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tickers/{symbol}/holders\n  method: get\n  operationId: alphayou_ticker_holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/top-traders\n  method: get\n  operationId: alphayou_top_traders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/alphayou-net/agentic-access/alphayou-net-agentic-access.yml
summary_line: 13 operations · 1 acting
tags:
- Finance
- Stock Research
- TradingTools
- Market Analytics
- Alerts
---
