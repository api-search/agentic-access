---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 31
api_specs:
- filename: oanda-pricing-api-openapi.yml
  format: yaml
  label: OANDA Pricing API
  slug: oanda-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oanda/refs/heads/main/openapi/oanda-pricing-api-openapi.yml
- filename: oanda-accounts-api-openapi.yml
  format: yaml
  label: OANDA Accounts API
  slug: oanda-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oanda/refs/heads/main/openapi/oanda-accounts-api-openapi.yml
- filename: oanda-instruments-api-openapi.yml
  format: yaml
  label: OANDA Instruments API
  slug: oanda-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oanda/refs/heads/main/openapi/oanda-instruments-api-openapi.yml
- filename: oanda-pricing-api-openapi.yml
  format: yaml
  label: OANDA Pricing API
  slug: oanda-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oanda/refs/heads/main/openapi/oanda-pricing-api-openapi.yml
- filename: oanda-users-api-openapi.yml
  format: yaml
  label: OANDA Users API
  slug: oanda-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oanda/refs/heads/main/openapi/oanda-users-api-openapi.yml
consequence_counts:
  physical: 7
  read: 31
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Oanda Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountID}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountID}/orders/{orderSpecifier}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountID}/orders/{orderSpecifier}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountID}/orders/{orderSpecifier}/clientExtensions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountID}/trades/{tradeSpecifier}/clientExtensions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountID}/trades/{tradeSpecifier}/close
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountID}/trades/{tradeSpecifier}/orders
operation_count: 40
overview: 'OANDA exposes 40 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 2 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OANDA
provider_slug: oanda
slug: oanda-agentic-access
source_filename: oanda-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/oanda-accounts-api-openapi.yml, openapi/oanda-instruments-api-openapi.yml, openapi/oanda-pricing-api-openapi.yml,\n  openapi/oanda-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 31\n    acting: 9\n  by_consequence:\n    read: 31\n    write: 2\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/{accountID}/positions\n  method: get\n  operationId: listPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/openPositions\n  method: get\n  operationId: listOpenPositions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/positions/{instrument}\n  method: get\n  operationId: getPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/positions/{instrument}/close\n  method: put\n  operationId: closePosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/trades\n  method: get\n  operationId: listTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /accounts/{accountID}/openTrades\n  method: get\n  operationId: listOpenTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/trades/{tradeSpecifier}\n  method: get\n  operationId: getTrade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/trades/{tradeSpecifier}/close\n  method: put\n  operationId: closeTrade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/trades/{tradeSpecifier}/clientExtensions\n  method: put\n  operationId:\
  \ setTradeClientExtensions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/trades/{tradeSpecifier}/orders\n  method: put\n  operationId: setTradeDependentOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /accounts/{accountID}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/summary\n  method: get\n  operationId: getAccountSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/instruments\n  method: get\n  operationId: getAccountInstruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/configuration\n  method: patch\n  operationId: configureAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/changes\n  method: get\n  operationId: getAccountChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transactions/{transactionID}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transactions/idrange\n  method: get\n  operationId: getTransactionRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transactions/sinceid\n  method: get\n  operationId: getTransactionsSinceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transactions/stream\n  method: get\n  operationId: streamTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/pricing\n  method: get\n  operationId: getPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/pricing/stream\n  method: get\n  operationId: streamPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /accounts/{accountID}/instruments/{instrument}/candles\n  method: get\n  operationId: getInstrumentCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/pendingOrders\n  method: get\n  operationId: listPendingOrders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/orders/{orderSpecifier}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/orders/{orderSpecifier}\n  method: put\n  operationId: replaceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/orders/{orderSpecifier}/cancel\n  method: put\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/orders/{orderSpecifier}/clientExtensions\n  method: put\n  operationId: setOrderClientExtensions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instruments/{instrument}/candles\n  method: get\n  operationId: getInstrumentCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/{instrument}/price\n\
  \  method: get\n  operationId: getInstrumentPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/{instrument}/price/range\n  method: get\n  operationId: getInstrumentPriceRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/{instrument}/orderBook\n  method: get\n  operationId: getInstrumentsByInstrumentOrderBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/{instrument}/positionBook\n  method: get\n  operationId: getInstrumentsByInstrumentPositionBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n\
  \  operationId: getBasePrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing/range\n  method: get\n  operationId: getPriceRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userSpecifier}\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userSpecifier}/externalInfo\n  method: get\n  operationId: getExternalUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oanda/refs/heads/main/agentic-access/oanda-agentic-access.yml
summary_line: 40 operations · 9 acting
tags:
- Forex
- FX Trading
- CFD Trading
- Financial-Services
- Trading APIs
---
