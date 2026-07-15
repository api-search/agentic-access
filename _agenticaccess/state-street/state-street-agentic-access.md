---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: state-street-alpha-data-platform-openapi.yml
  format: yaml
  label: Alpha Data Platform API
  slug: alpha-data-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/openapi/state-street-alpha-data-platform-openapi.yml
- filename: state-street-fund-connect-openapi.yml
  format: yaml
  label: Fund Connect API
  slug: fund-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/openapi/state-street-fund-connect-openapi.yml
consequence_counts:
  physical: 2
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: State Street Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/cancel
operation_count: 13
overview: 'State Street exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: State Street
provider_slug: state-street
slug: state-street-agentic-access
source_filename: state-street-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/state-street-alpha-data-platform-openapi.yml, openapi/state-street-fund-connect-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 11\n    acting: 2\n  by_consequence:\n    read: 11\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /portfolios\n  method: get\n  operationId: listPortfolios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - performance:read\n    - portfolio:read\n    - positions:read\n    - risk:read\n    - transactions:read\n- path: /portfolios/{portfolioId}\n  method: get\n  operationId:\
  \ getPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - performance:read\n    - portfolio:read\n    - positions:read\n    - risk:read\n    - transactions:read\n- path: /portfolios/{portfolioId}/positions\n  method: get\n  operationId: listPortfolioPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - performance:read\n    - portfolio:read\n    - positions:read\n    - risk:read\n    - transactions:read\n- path: /portfolios/{portfolioId}/transactions\n  method: get\n  operationId: listPortfolioTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - performance:read\n    - portfolio:read\n    - positions:read\n    - risk:read\n\
  \    - transactions:read\n- path: /portfolios/{portfolioId}/performance\n  method: get\n  operationId: getPortfolioPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - performance:read\n    - portfolio:read\n    - positions:read\n    - risk:read\n    - transactions:read\n- path: /portfolios/{portfolioId}/risk\n  method: get\n  operationId: getPortfolioRisk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - performance:read\n    - portfolio:read\n    - positions:read\n    - risk:read\n    - transactions:read\n- path: /funds\n  method: get\n  operationId: listFunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fund-connect:baskets:read\n\
  \    - fund-connect:orders:read\n    - fund-connect:orders:write\n- path: /funds/{fundId}\n  method: get\n  operationId: getFund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fund-connect:baskets:read\n    - fund-connect:orders:read\n    - fund-connect:orders:write\n- path: /funds/{fundId}/baskets\n  method: get\n  operationId: getFundBasket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fund-connect:baskets:read\n    - fund-connect:orders:read\n    - fund-connect:orders:write\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - fund-connect:baskets:read\n    - fund-connect:orders:read\n    - fund-connect:orders:write\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fund-connect:baskets:read\n    - fund-connect:orders:read\n    - fund-connect:orders:write\n- path: /orders/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - fund-connect:baskets:read\n    - fund-connect:orders:read\n    - fund-connect:orders:write\n- path: /orders/{orderId}/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - fund-connect:baskets:read\n    - fund-connect:orders:read\n    - fund-connect:orders:write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/agentic-access/state-street-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Fortune 500
---
