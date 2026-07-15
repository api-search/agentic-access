---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: ssc-geneva-fund-accounting-openapi.yml
  format: yaml
  label: SS&C Geneva Fund Accounting API
  slug: ssc-geneva-fund-accounting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssc-geneva/refs/heads/main/openapi/ssc-geneva-fund-accounting-openapi.yml
consequence_counts:
  physical: 1
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ssc Geneva Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolios/{portfolioId}/trades
operation_count: 7
overview: 'SS&C Geneva exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SS&C Geneva
provider_slug: ssc-geneva
slug: ssc-geneva-agentic-access
source_filename: ssc-geneva-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ssc-geneva-fund-accounting-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /portfolios\n  method: get\n  operationId: listPortfolios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolios/{portfolioId}\n  method: get\n  operationId: getPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolios/{portfolioId}/positions\n\
  \  method: get\n  operationId: getPortfolioPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolios/{portfolioId}/trades\n  method: get\n  operationId: listTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolios/{portfolioId}/trades\n  method: post\n  operationId: createTrade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolios/{portfolioId}/nav\n  method: get\n  operationId: getPortfolioNAV\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolios/{portfolioId}/investors\n  method: get\n  operationId: listInvestors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ssc-geneva/refs/heads/main/agentic-access/ssc-geneva-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Fund Accounting
- Asset Management
- Portfolio Management
- Financial Services
- Hedge Funds
- NAV Calculation
---
