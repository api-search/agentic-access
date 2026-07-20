---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 40
api_specs:
- filename: dinari-openapi-original.yml
  format: yaml
  label: Dinari Enterprise API
  slug: dinari-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-openapi-original.yml
consequence_counts:
  physical: 11
  read: 40
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dinari Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/order_requests/eip155
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/order_requests/eip155/permit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/order_requests/eip155/permit_transaction
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/order_requests/limit_buy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/order_requests/limit_sell
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/order_requests/market_buy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/order_requests/market_sell
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/orders/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/token_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/accounts/{account_id}/withdrawal_requests
operation_count: 61
overview: 'Dinari exposes 61 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read, 10 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dinari
provider_slug: dinari
slug: dinari-agentic-access
source_filename: dinari-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/dinari-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 61\n  by_action_class:\n    connected: 40\n    acting: 21\n  by_consequence:\n    read: 40\n    write: 10\n    physical: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/market_data/alloys/\n  method: get\n  operationId: getAlloys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/alloys/{alloy_id}/current_price\n  method: get\n  operationId: getAlloyCurrentPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/alloys/{alloy_id}/historical_prices/\n  method: get\n  operationId: getAlloyPriceChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/stocks/\n  method: get\n  operationId: getStocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/stocks/{stock_id}/current_price\n  method: get\n  operationId: getStockCurrentPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/stocks/{stock_id}/current_quote\n  method: get\n  operationId: getStockCurrentQuotesRouteV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/stocks/{stock_id}/historical_prices/\n  method: get\n  operationId: getStockPriceChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/stocks/splits\n  method: get\n  operationId: getStockSplits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/stocks/{stock_id}/splits\n  method: get\n  operationId: getStockSplitsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/stocks/{stock_id}/news\n  method: get\n  operationId: getStockNewsByStockId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/stocks/{stock_id}/dividends\n  method: get\n  operationId: getStockDividendsByStockId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market_data/market_hours/\n  method: get\n  operationId: getMarketHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/entities/\n  method: get\n  operationId: getEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/entities/\n  method: post\n  operationId: createEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/entities/me\n  method: get\n  operationId: getCurrentEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/entities/{entity_id}\n  method: get\n  operationId: getEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/entities/{entity_id}\n  method: patch\n  operationId: updateEntityById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/entities/{entity_id}/accounts\n  method: get\n  operationId:\
  \ getEntityAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/entities/{entity_id}/accounts\n  method: post\n  operationId: createEntityAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/entities/{entity_id}/kyc\n  method: get\n  operationId: getEntityKyc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/entities/{entity_id}/kyc\n  method: post\n  operationId: createEntityKyc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/entities/{entity_id}/kyc/{kyc_id}/document\n  method: get\n  operationId: getEntityKycDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/entities/{entity_id}/kyc/{kyc_id}/document\n  method: post\n  operationId: createEntityKycDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/entities/{entity_id}/kyc/url\n  method: post\n  operationId: createManagedEntityKycEmbed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/orders/\n  method: get\n  operationId: getEntityOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/deactivate\n  method: post\n  operationId: createAccountDeactivation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v2/accounts/{account_id}/portfolio\n  method: get\n  operationId: getAccountPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/cash\n  method: get\n  operationId: getAccountCash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/interest_payments\n  method: get\n  operationId: getAccountInterestPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/dividend_payments\n  method: get\n  operationId: getAccountDividendPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v2/accounts/{account_id}/faucet\n  method: post\n  operationId: createAccountFaucet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/activities/brokerage\n  method: get\n  operationId: getBrokerageAccountActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/wallet\n  method: get\n  operationId: getWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/wallet/external/nonce\n  method: get\n  operationId: getAccountWalletConnectionNonce\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/wallet/external\n  method: post\n  operationId: createAccountWalletConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/wallet/internal\n  method: post\n  operationId: createAccountWalletInternalConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/orders\n  method: get\n\
  \  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/orders/{order_id}\n  method: get\n  operationId: getOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/orders/{order_id}/cancel\n  method: post\n  operationId: createOrderCancellation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/orders/cancel\n  method: post\n  operationId: createBatchOrderCancellation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/order_requests\n  method: get\n  operationId: getListOrderRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/order_requests/{order_request_id}\n  method: get\n  operationId: getOrderRequestById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/order_requests/eip155/permit\n  method: post\n  operationId: createEIP155OrderRequestPermit\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/order_requests/eip155\n  method: post\n  operationId: createEIP155OrderRequestPermitTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/order_requests/eip155/permit_transaction\n  method: post\n  operationId: createEip155PermitTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/order_fulfillments\n  method: get\n  operationId: getAccountAllOrderFulfillments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/orders/{order_id}/fulfillments\n  method: get\n  operationId: getAccountOrderFulfillments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/order_fulfillments/{order_fulfillment_id}\n  method: get\n  operationId: getAccountOrderFulfillmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/order_requests/market_buy\n  method: post\n  operationId: createMarketBuyManagedOrderRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/order_requests/market_sell\n  method: post\n  operationId: createMarketSellManagedOrderRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v2/accounts/{account_id}/order_requests/limit_buy\n  method: post\n  operationId: createLimitBuyManagedOrderRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/order_requests/limit_sell\n  method: post\n  operationId: createLimitSellManagedOrderRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/token_transfers\n  method: get\n  operationId:\
  \ getTokenTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/token_transfers\n  method: post\n  operationId: createTokenTransfers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/token_transfers/{transfer_id}\n  method: get\n  operationId: getTokenTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/withdrawal_requests\n  method: get\n  operationId: getAccountWithdrawalRequests\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/withdrawal_requests\n  method: post\n  operationId: createAccountWithdrawalRequests\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/accounts/{account_id}/withdrawal_requests/{withdrawal_request_id}\n  method: get\n  operationId: getAccountWithdrawalRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/withdrawals\n  method: get\n  operationId: getAccountWithdrawals\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{account_id}/withdrawals/{withdrawal_id}\n  method: get\n  operationId: getAccountWithdrawal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/agentic-access/dinari-agentic-access.yml
summary_line: 61 operations · 21 acting
tags:
- Company
- Tokenized Securities
- Stocks
- ETFs
- Brokerage
- Market Data
- Blockchain
- Stablecoin
- Fintech
- KYC
- Orders
- Wallets
---
