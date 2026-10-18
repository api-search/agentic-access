---
acting_count: 34
action_class_counts:
  acting: 34
  connected: 46
api_specs:
- filename: latoken-account-api-openapi.yml
  format: yaml
  label: LATOKEN Account API
  slug: latoken-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-account-api-openapi.yml
- filename: latoken-appealcontroller-api-openapi.yml
  format: yaml
  label: LATOKEN Appeal Controller API
  slug: latoken-appealcontroller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-appealcontroller-api-openapi.yml
- filename: latoken-bulkorder-api-openapi.yml
  format: yaml
  label: LATOKEN Bulk Order API
  slug: latoken-bulkorder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-bulkorder-api-openapi.yml
- filename: latoken-chart-api-openapi.yml
  format: yaml
  label: LATOKEN Chart API
  slug: latoken-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-chart-api-openapi.yml
- filename: latoken-chatcontroller-api-openapi.yml
  format: yaml
  label: LATOKEN Chat Controller API
  slug: latoken-chatcontroller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-chatcontroller-api-openapi.yml
- filename: latoken-currency-api-openapi.yml
  format: yaml
  label: LATOKEN Currency API
  slug: latoken-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-currency-api-openapi.yml
- filename: latoken-offercontroller-api-openapi.yml
  format: yaml
  label: LATOKEN Offer Controller API
  slug: latoken-offercontroller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-offercontroller-api-openapi.yml
- filename: latoken-order-api-openapi.yml
  format: yaml
  label: LATOKEN Order API
  slug: latoken-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-order-api-openapi.yml
- filename: latoken-ordercontroller-api-openapi.yml
  format: yaml
  label: LATOKEN Order Controller API
  slug: latoken-ordercontroller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-ordercontroller-api-openapi.yml
- filename: latoken-pair-api-openapi.yml
  format: yaml
  label: LATOKEN Pair API
  slug: latoken-pair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-pair-api-openapi.yml
- filename: latoken-paymentmethodcontroller-api-openapi.yml
  format: yaml
  label: LATOKEN Payment Method Controller API
  slug: latoken-paymentmethodcontroller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-paymentmethodcontroller-api-openapi.yml
- filename: latoken-spot-api-openapi.yml
  format: yaml
  label: LATOKEN Spot API
  slug: latoken-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-spot-api-openapi.yml
- filename: latoken-stoporder-api-openapi.yml
  format: yaml
  label: LATOKEN Stop Order API
  slug: latoken-stoporder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-stoporder-api-openapi.yml
- filename: latoken-ticker-api-openapi.yml
  format: yaml
  label: LATOKEN Ticker API
  slug: latoken-ticker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-ticker-api-openapi.yml
- filename: latoken-time-api-openapi.yml
  format: yaml
  label: LATOKEN Time API
  slug: latoken-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-time-api-openapi.yml
- filename: latoken-trade-api-openapi.yml
  format: yaml
  label: LATOKEN Trade API
  slug: latoken-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-trade-api-openapi.yml
- filename: latoken-transaction-api-openapi.yml
  format: yaml
  label: LATOKEN Transaction API
  slug: latoken-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-transaction-api-openapi.yml
- filename: latoken-transfer-api-openapi.yml
  format: yaml
  label: LATOKEN Transfer API
  slug: latoken-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-transfer-api-openapi.yml
- filename: latoken-usercontroller-api-openapi.yml
  format: yaml
  label: LATOKEN User Controller API
  slug: latoken-usercontroller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-usercontroller-api-openapi.yml
- filename: latoken-orderbook-api-openapi.yml
  format: yaml
  label: LATOKEN Orderbook API
  slug: latoken-orderbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/openapi/latoken-orderbook-api-openapi.yml
consequence_counts:
  physical: 16
  read: 46
  safety-critical: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 18
kind: agentic-access
layout: agentic-access
method: generated
name: Latoken Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/offer
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/offer/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/offer/update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/order
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/order/appeal
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/order/appeal/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/order/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/order/chat/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/order/complete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/order/confirm
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/paymentMethods
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/paymentMethods/remove
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/paymentMethods/update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/p2p/user/register
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/auth/stopOrder/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/auth/stopOrder/cancelAll
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/auth/stopOrder/cancelAll/{currency}/{quote}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/auth/stopOrder/place
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/auth/order/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/auth/order/cancelAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/auth/order/cancelAll/{currency}/{quote}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/auth/order/cancelBulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/auth/order/place
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/auth/order/placeBulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/auth/spot/deposit
operation_count: 80
overview: 'LATOKEN exposes 80 API operations that an AI agent could call, of which 34 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read, 16 physical, and 18 safety-critical.


  18 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LATOKEN
provider_slug: latoken
slug: latoken-agentic-access
source_filename: latoken-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/latoken-openapi.yml, openapi/latoken-p2p-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 80\n  by_action_class:\n    connected: 46\n    acting: 34\n  by_consequence:\n    read: 46\n    physical: 16\n    safety-critical: 18\n  human_in_the_loop_required: 18\noperations:\n- path: /v2/auth/account\n  method: get\n  operationId: getBalancesByUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/account/currency/{currency}/{type}\n  method: get\n  operationId: getBalancesByCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/account/filtered\n  method: get\n  operationId: getBalancesByUserCurrenciesAndTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/order\n  method: get\n  operationId: getMyOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/order/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/order/cancelAll\n  method: post\n  operationId: cancelAllOrders\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/order/cancelAll/{currency}/{quote}\n  method: post\n  operationId: cancelAllOrdersByPair\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/order/getOrder/{id}\n  method: get\n  operationId: getOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/auth/order/pair/{currency}/{quote}\n  method: get\n  operationId: getMyOrdersByPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/order/pair/{currency}/{quote}/active\n  method: get\n  operationId: getMyActiveOrdersByPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/order/active\n  method: get\n  operationId: getMyActiveOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/order/place\n  method: post\n  operationId: placeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/spot/deposit\n  method: post\n  operationId: depositSpotAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/spot/withdraw\n  method: post\n  operationId: withdrawSpotAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/trade\n  method: get\n\
  \  operationId: getTradesByTrader\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/trade/pair/{currency}/{quote}\n  method: get\n  operationId: getTradesByAssetAndTrader\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/trade/fee/{currency}/{quote}\n  method: get\n  operationId: getAuthFeeByPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/transaction\n  method: get\n  operationId: getUserTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/transaction/bindings\n  method: get\n  operationId: getCurrenciesBindings\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/transaction/bindings/{currency}\n  method: get\n  operationId: getCurrencyBindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/transaction/depositAddress\n  method: post\n  operationId: generateDepositAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/transaction/withdraw\n  method: post\n  operationId: withdrawMoney\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/transaction/withdraw/cancel\n  method: post\n  operationId: cancelWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/transaction/withdraw/confirm\n  method: post\n  operationId: confirmWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/transaction/withdraw/resendCode\n  method: post\n  operationId: resendVerificationCode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/transaction/{id}\n  method: get\n  operationId: getTransactionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/transfer\n  method: get\n  operationId: getUsersTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/transfer/email\n\
  \  method: post\n  operationId: transferByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/transfer/id\n  method: post\n  operationId: transferById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/transfer/phone\n  method: post\n  operationId: transferByPhone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/book/{currency}/{quote}\n  method: get\n  operationId: getOrderBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/chart/week\n  method: get\n  operationId: getAllWeeklyCharts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/chart/week/{currency}/{quote}\n  method: get\n  operationId: getWeeklyCharts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/currency\n  method: get\n  operationId: getActiveCurrencies\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/currency/available\n  method: get\n  operationId: getAvailableCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/currency/quotes\n  method: get\n  operationId: getQuoteCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/currency/{currency}\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/pair\n  method: get\n  operationId: getActivePairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/pair/available\n\
  \  method: get\n  operationId: getAvailablePairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/stopOrder\n  method: get\n  operationId: getMyStopOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/stopOrder/cancel\n  method: post\n  operationId: cancelStopOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/auth/stopOrder/cancelAll\n  method: post\n  operationId: cancelAllStopOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/auth/stopOrder/cancelAll/{currency}/{quote}\n  method: post\n  operationId: cancelAllStopOrdersByPair\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/auth/stopOrder/getOrder/{id}\n  method: get\n  operationId: getStopOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/stopOrder/pair/{currency}/{quote}\n  method: get\n  operationId: getMyStopOrdersByPair\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/stopOrder/pair/{currency}/{quote}/active\n  method: get\n  operationId: getMyActiveStopOrdersByPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/stopOrder/place\n  method: post\n  operationId: placeStopOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/auth/order/placeBulk\n  method: post\n  operationId: placeBulkOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/order/cancelBulk\n  method: post\n  operationId: cancelBulkOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ticker\n  method: get\n  operationId: getAllTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ticker/{base}/{quote}\n  method: get\n  operationId: getTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/time\n  method: get\n  operationId: currentTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trade/history/{currency}/{quote}\n  method: get\n  operationId: getTradesByPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trade/fee/{currency}/{quote}\n  method: get\n  operationId: getFeeByPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trade/feeLevels\n  method: get\n  operationId: getFeeLevels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transaction/bindings\n  method: get\n  operationId:\
  \ getBindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /p2p/offers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /p2p/config\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /p2p/offers/rates\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/p2p/user/register\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/user\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/p2p/paymentMethods\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/paymentMethods\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/p2p/paymentMethods/update\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/paymentMethods/remove\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/paymentMethods/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/p2p/offer\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/merchant/offers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/p2p/offer/update\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/offer/delete\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /auth/p2p/order\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/order/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/p2p/orders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/p2p/merchant/orders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/p2p/order/confirm\n  method:\
  \ post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/order/complete\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/order/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /auth/p2p/order/appeal\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/order/appeal/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/p2p/order/chat/{id}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/latoken/refs/heads/main/agentic-access/latoken-agentic-access.yml
summary_line: 80 operations · 34 acting · 18 human-in-the-loop
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- P2P
- WebSocket
---
