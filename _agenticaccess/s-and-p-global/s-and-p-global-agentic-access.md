---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: servicecatalog
  format: yaml
  label: S&P Global Commodity Insights API
  slug: commodity-insights
  spec_type: OpenAPI
  url: https://developer.spglobal.com/commodityinsights/servicecatalog
- filename: s-and-p-global-kensho-link-openapi.yml
  format: yaml
  label: Kensho Link API
  slug: kensho-link
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s-and-p-global/refs/heads/main/openapi/s-and-p-global-kensho-link-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: S And P Global Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'S&P Global exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: S&P Global
provider_slug: s-and-p-global
slug: s-and-p-global-agentic-access
source_filename: s-and-p-global-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/s-and-p-global-commodity-insights-openapi.yml, openapi/s-and-p-global-kensho-link-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 2\n    connected: 6\n  by_consequence:\n    write: 2\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/api\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market-data/v1/value/current\n  method: get\n  operationId:\
  \ getCurrentMarketData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market-data/v1/value/history\n  method: get\n  operationId: getHistoricalMarketData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market-data/v1/symbols\n  method: get\n  operationId: listSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market-data/v1/modified-date\n  method: get\n  operationId: getModifiedSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link\n  method: post\n  operationId: linkEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entity/{keid}\n  method: get\n  operationId: getEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/s-and-p-global/refs/heads/main/agentic-access/s-and-p-global-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Financial Data
- Credit Ratings
- Market Intelligence
- Commodity Insights
- Energy Markets
- Capital Markets
- Fortune 500
---
