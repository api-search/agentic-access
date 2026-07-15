---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 72
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Bamboo Investment API
  slug: bamboo-investment-api
  spec_type: OpenAPI
  url: https://docs.investbamboo.com/api/
consequence_counts:
  physical: 6
  read: 72
  safety-critical: 22
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 22
kind: agentic-access
layout: agentic-access
method: generated
name: Bamboo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/extended_hours/opt_in
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/extended_hours/opt_in
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/lsx/ng/order
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/lsx/ng/order
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/lsx/ng/order/calculate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/lsx/ng/order/calculate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/lsx/ng/withdraw
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/lsx/ng/withdraw
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/one_step_registration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/one_step_registration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/order
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/order
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/order/calculate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/order/calculate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/tenant_brokerage_withdraw
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/tenant_brokerage_withdraw
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/one_step_registration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/one_step_registration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bamboo/webhook
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bamboo/webhook
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/lsx/ng/deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/lsx/ng/deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/lsx/ng/order/:order_id/cancel
operation_count: 102
overview: 'Bamboo Invest exposes 102 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 72 read, 2 write, 6 physical, and 22 safety-critical.


  22 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bamboo Invest
provider_slug: bamboo
slug: bamboo-agentic-access
source_filename: bamboo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bamboo-openapi.json, openapi/bamboo-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 102\n  by_action_class:\n    acting: 30\n    connected: 72\n  by_consequence:\n    safety-critical: 22\n    read: 72\n    write: 2\n    physical: 6\n  human_in_the_loop_required: 22\noperations:\n- path: /oauth/token\n  method: post\n  operationId: Web.Api.AuthController.oauth\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /api/v2/one_step_registration\n  method: post\n  operationId: Web.Api.RegisterController.registration_step\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/one_step_registration\n  method: post\n  operationId: Web.Api.RegisterController.registration_step\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/dictionary\n  method: get\n  operationId: Web.Api.RegisterController.dictionary\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/brokerage_accounts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profile\n  method: get\n  operationId: Web.Api.ProfileController.profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/investment_profile\n  method: get\n  operationId: Web.Api.ProfileController.investment_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bamboo/webhook\n  method: post\n  operationId: Web.Api.TransactionController.webhook\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tenant/deposit\n  method: get\n  operationId: Web.Api.Tenant.TenantDepositController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/deposit/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/deposit/status/{txref}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant_brokerage_withdraw\n\
  \  method: post\n  operationId: Web.Api.WithdrawController.tenant_brokerage_withdraw_ngn\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tenant/withdraws\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/withdraw/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/withdraw/status/{reference}\n  method: get\n  operationId: Web.Api.Tenant.WithdrawController.withdraw_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/themes\n  method: get\n  operationId: Web.Api.ThemeController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/themed_stock/{theme_id}\n  method: get\n  operationId: Web.Api.ThemeController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/exchange_rate\n  method: get\n  operationId: Web.Api.Tenant.ExchangeRateController.exchange_rate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/market/open_date\n  method: get\n  operationId: Web.Api.Tenant.ExchangeRateController.market_activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extended_hours/opt_in\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/document_list\n  method: get\n  operationId: Web.Api.Tenant.ExchangeRateController.exchange_rate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/document\n  method: get\n  operationId: Web.Api.Tenant.DocumentController.document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/portfolio\n  method: get\n  operationId: Web.Api.PortfolioController.portfolio\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/portfolio/breakdown\n  method: get\n  operationId: Web.Api.PortfolioController.portfolio_breakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stock/{stockSymbol}/ownership\n  method: get\n  operationId: Web.Api.PortfolioController.ownership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stocks\n  method: get\n  operationId: Web.Api.StockController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/stock/{symbol}/details\n  method: get\n  operationId: Web.Api.StockDataController.details\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stock/search\n  method: get\n  operationId: Web.Api.StockController.search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/my_stocks\n  method: get\n  operationId: Web.Api.StockDataController.ownership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/order/calculate\n  method: post\n  operationId: Web.Api.OrderController.calculate_market_order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/order\n  method: post\n  operationId: Web.Api.OrderController.place_market_order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/order/{id}/status\n  method: get\n  operationId: Web.Api.OrderController.status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pending_orders\n  method: get\n  operationId: Web.Api.OrderController.pending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/order/{id}/cancel\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lsx/ng/dictionary\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: https://cscs-banks.investbamboo.com/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/portfolio/breakdown\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/user_cash_balance/{currency}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/deposit\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lsx/ng/deposit/{reference}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/withdraw\n  method: post\n  operationId: Web.Api.WithdrawController.tenant_brokerage_withdraw_ngn\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/lsx/ng/withdraw/{reference}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/stocks\n  method: get\n  operationId: Web.Api.StockController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/stocks/{symbol}\n  method: get\n  operationId: Web.Api.StockDataController.about\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/my_stocks\n  method: get\n  operationId: Web.Api.StockController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/order/calculate\n  method: post\n  operationId: Web.Api.OrderController.calculate_order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/lsx/ng/order\n  method: post\n  operationId: Web.Api.OrderController.order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/lsx/ng/order/:order_id\n  method: get\n  operationId: Web.Api.OrderController.status\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/order/:order_id/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/pending_orders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/order/:order_id/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: Web.Api.AuthController.oauth\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/one_step_registration\n  method: post\n  operationId: Web.Api.RegisterController.registration_step\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/one_step_registration\n  method: post\n  operationId: Web.Api.RegisterController.registration_step\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/dictionary\n  method: get\n  operationId: Web.Api.RegisterController.dictionary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/brokerage_accounts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/profile\n  method: get\n  operationId: Web.Api.ProfileController.profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/investment_profile\n  method: get\n \
  \ operationId: Web.Api.ProfileController.investment_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bamboo/webhook\n  method: post\n  operationId: Web.Api.TransactionController.webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tenant/deposit\n  method: get\n  operationId: Web.Api.Tenant.TenantDepositController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/deposit/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/deposit/status/{txref}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant_brokerage_withdraw\n  method: post\n  operationId: Web.Api.WithdrawController.tenant_brokerage_withdraw_ngn\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tenant/withdraws\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/withdraw/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/withdraw/status/{reference}\n  method: get\n  operationId: Web.Api.Tenant.WithdrawController.withdraw_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/themes\n  method: get\n  operationId: Web.Api.ThemeController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/themed_stock/{theme_id}\n  method: get\n  operationId: Web.Api.ThemeController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/exchange_rate\n  method: get\n  operationId: Web.Api.Tenant.ExchangeRateController.exchange_rate\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/market/open_date\n  method: get\n  operationId: Web.Api.Tenant.ExchangeRateController.market_activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extended_hours/opt_in\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/document_list\n  method: get\n  operationId: Web.Api.Tenant.ExchangeRateController.exchange_rate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/document\n  method: get\n  operationId: Web.Api.Tenant.DocumentController.document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/portfolio\n  method: get\n  operationId: Web.Api.PortfolioController.portfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/portfolio/breakdown\n  method: get\n  operationId: Web.Api.PortfolioController.portfolio_breakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stock/{stockSymbol}/ownership\n  method: get\n  operationId: Web.Api.PortfolioController.ownership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/stocks\n  method: get\n  operationId: Web.Api.StockController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenant/stock/{symbol}/details\n  method: get\n  operationId: Web.Api.StockDataController.details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stock/search\n  method: get\n  operationId: Web.Api.StockController.search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/my_stocks\n  method: get\n  operationId: Web.Api.StockDataController.ownership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/order/calculate\n  method:\
  \ post\n  operationId: Web.Api.OrderController.calculate_market_order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/order\n  method: post\n  operationId: Web.Api.OrderController.place_market_order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/order/{id}/status\n  method: get\n  operationId: Web.Api.OrderController.status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/pending_orders\n  method: get\n  operationId: Web.Api.OrderController.pending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/order/{id}/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lsx/ng/dictionary\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: https://cscs-banks.investbamboo.com/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/portfolio/breakdown\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/user_cash_balance/{currency}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/deposit\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lsx/ng/deposit/{reference}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/withdraw\n  method: post\n  operationId: Web.Api.WithdrawController.tenant_brokerage_withdraw_ngn\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/lsx/ng/withdraw/{reference}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/stocks\n  method: get\n  operationId: Web.Api.StockController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/stocks/{symbol}\n  method: get\n  operationId: Web.Api.StockDataController.about\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/my_stocks\n  method: get\n  operationId: Web.Api.StockController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/order/calculate\n  method: post\n  operationId: Web.Api.OrderController.calculate_order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/lsx/ng/order\n  method: post\n  operationId: Web.Api.OrderController.order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/lsx/ng/order/:order_id\n  method: get\n  operationId: Web.Api.OrderController.status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/order/:order_id/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/pending_orders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lsx/ng/order/:order_id/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bamboo/refs/heads/main/agentic-access/bamboo-agentic-access.yml
summary_line: 102 operations · 30 acting · 22 human-in-the-loop
tags:
- Investments
- Stocks
- Fractional Shares
- Africa
- Nigeria
- Portfolio Management
- Brokerage
- Fintech
---
