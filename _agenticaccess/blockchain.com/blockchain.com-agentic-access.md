---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 30
api_specs:
- filename: blockchain.com-nft-market-api-swagger.json
  format: json
  label: Blockchain.com NFT Market API
  slug: blockchaincom-nft-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/_original/blockchain.com-nft-market-api-swagger.json
- filename: blockchain.com-eligibility-api-openapi.yml
  format: yaml
  label: Blockchain.com Eligibility API
  slug: blockchain.com-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-eligibility-api-openapi.yml
- filename: blockchain.com-nft-api-openapi.yml
  format: yaml
  label: Blockchain.com Nft API
  slug: blockchain.com-nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-nft-api-openapi.yml
- filename: blockchain.com-nft-v2-api-openapi.yml
  format: yaml
  label: Blockchain.com Nft V2 API
  slug: blockchain.com-nft-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-nft-v2-api-openapi.yml
- filename: blockchain.com-orders-api-openapi.yml
  format: yaml
  label: Blockchain.com Orders API
  slug: blockchain.com-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-orders-api-openapi.yml
- filename: blockchain.com-payments-api-openapi.yml
  format: yaml
  label: Blockchain.com Payments API
  slug: blockchain.com-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-payments-api-openapi.yml
- filename: blockchain.com-public-api-openapi.yml
  format: yaml
  label: Blockchain.com Public API
  slug: blockchain.com-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-public-api-openapi.yml
- filename: blockchain.com-quote-api-openapi.yml
  format: yaml
  label: Blockchain.com Quote API
  slug: blockchain.com-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-quote-api-openapi.yml
- filename: blockchain.com-trading-api-openapi.yml
  format: yaml
  label: Blockchain.com Trading API
  slug: blockchain.com-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-trading-api-openapi.yml
- filename: blockchain.com-unauthenticated-api-openapi.yml
  format: yaml
  label: Blockchain.com Unauthenticated API
  slug: blockchain.com-unauthenticated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/openapi/blockchain.com-unauthenticated-api-openapi.yml
consequence_counts:
  physical: 5
  read: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blockchain.Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deposits/{currency}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdrawals
operation_count: 35
overview: 'Blockchain.com exposes 35 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blockchain.com
provider_slug: blockchain.com
slug: blockchain.com-agentic-access
source_filename: blockchain.com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/blockchain.com-exchange-openapi.yml, openapi/blockchain.com-nft-market-api-swagger.json,\n  openapi/blockchain.com-pay-partner-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 30\n    acting: 5\n  by_consequence:\n    read: 30\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /l2/{symbol}\n  method: get\n  operationId: getL2OrderBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /l3/{symbol}\n  method: get\n  operationId: getL3OrderBook\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickers\n  method: get\n  operationId: getTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickers/{symbol}\n  method: get\n  operationId: getTickerBySymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /symbols\n  method: get\n  operationId: getSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /symbols/{symbol}\n  method: get\n  operationId: getSymbolByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account}/{currency}\n  method: get\n  operationId: getAccountByTypeAndCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fees\n  method: get\n  operationId: getFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: delete\n  operationId: deleteAllOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: get\n  operationId: getOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trades\n  method: get\n  operationId: getFills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposits/{currency}\n  method: post\n  operationId: getDepositAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deposits\n  method: get\n  operationId: getDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /deposits/{depositId}\n  method: get\n  operationId: getDepositById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whitelist\n  method: get\n  operationId: getWhitelist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whitelist/{currency}\n  method: get\n  operationId: getWhitelistByCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals\n  method: get\n  operationId: getWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals\n  method: post\n  operationId: createWithdrawal\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdrawals/{withdrawalId}\n  method: get\n  operationId: getWithdrawalById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/nft/account_assets/{owner_address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/nft/account_assets/{owner_address}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/nft/v2/asset/{network}/{contract_address}/{token_id}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/nft/v2/account_assets/{owner_address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/nft/v2/account_assets/{owner_address}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/nft/v2/asset/{network}/{contract_address}/{token_id}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/currencies\n  method: get\n  operationId: GetCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/regions\n  method: get\n  operationId: GetRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment-methods\n  method: get\n  operationId: GetPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders\n  method: get\n  operationId: ListOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{id}\n  method: get\n  operationId: GetOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quote/buy\n  method: get\n  operationId: GetQuoteBuy\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchain.com/refs/heads/main/agentic-access/blockchain.com-agentic-access.yml
summary_line: 35 operations · 5 acting
tags:
- Cryptocurrency
- Bitcoin
- Blockchain
- Exchange
- Trading
- Market Data
- Payments
- On-Ramp
- Wallets
- Block Explorer
- Fintech
- Webhook
---
