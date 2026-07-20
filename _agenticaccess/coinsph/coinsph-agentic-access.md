---
acting_count: 63
action_class_counts:
  acting: 63
  connected: 50
api_specs:
- filename: coinsph-account-openapi.json
  format: json
  label: Coins.ph Coins Pro — Account
  slug: coinsph-coins-pro-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-account-openapi.json
- filename: coinsph-account-validation-openapi.json
  format: json
  label: Coins.ph Account Validation
  slug: coinsph-account-validation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-account-validation-openapi.json
- filename: coinsph-convert-openapi.json
  format: json
  label: Coins.ph Coins Pro — Convert
  slug: coinsph-coins-pro-convert
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-convert-openapi.json
- filename: coinsph-listenkey-openapi.json
  format: json
  label: Coins.ph Coins Pro — User Data Stream
  slug: coinsph-coins-pro-user-data-stream
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-listenkey-openapi.json
- filename: coinsph-markets-openapi.json
  format: json
  label: Coins.ph Coins Pro — Market Data
  slug: coinsph-coins-pro-market-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-markets-openapi.json
- filename: coinsph-payment-openapi.json
  format: json
  label: Coins.ph Payment / Partner Integration
  slug: coinsph-payment-partner-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-payment-openapi.json
- filename: coinsph-ramp-openapi.json
  format: json
  label: Coins.ph ON/OFF Ramp
  slug: coinsph-onoff-ramp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-ramp-openapi.json
- filename: coinsph-spot-openapi.json
  format: json
  label: Coins.ph Coins Pro — Spot Trading
  slug: coinsph-coins-pro-spot-trading
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-spot-openapi.json
- filename: coinsph-sub-account-openapi.json
  format: json
  label: Coins.ph Coins Pro — Sub-Account
  slug: coinsph-coins-pro-sub-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-sub-account-openapi.json
- filename: coinsph-system-openapi.json
  format: json
  label: Coins.ph Coins Pro — System
  slug: coinsph-coins-pro-system
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-system-openapi.json
- filename: coinsph-wallet-openapi.json
  format: json
  label: Coins.ph Coins Pro — Wallet
  slug: coinsph-coins-pro-wallet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-wallet-openapi.json
consequence_counts:
  physical: 33
  read: 50
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coinsph Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/convert/v1/accept-quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/convert/v1/get-quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/convert/v1/get-supported-trading-pairs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/convert/v1/query-order-history
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/fiat/v1/auto-debit/token-apply
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/fiat/v1/auto-debit/token-pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/fiat/v1/auto-debit/token-query
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/fiat/v1/auto-debit/token-remove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/fiat/v1/checkout/create-checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/fiat/v1/checkout/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/fiat/v1/refund/pay-in-refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/fiat/v2/history
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/otc-trade/v1/accept-rfq
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/otc-trade/v1/create-rfq
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/otc-trade/v1/get-supported-trading-pairs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/otc-trade/v1/manual-settle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/ramp/callback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/ramp/v1/orderDetail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/ramp/v1/paymentConfigurations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/transfer/v3/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/transfer/v4/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /openapi/v1/openOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /openapi/v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/v1/order/cancelReplace
operation_count: 113
overview: 'Coins.ph exposes 113 API operations that an AI agent could call, of which 63 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 50 read, 30 write, and 33 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Coins.ph
provider_slug: coinsph
slug: coinsph-agentic-access
source_filename: coinsph-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/coinsph-account-openapi.json, openapi/coinsph-account-validation-openapi.json,\n  openapi/coinsph-convert-openapi.json, openapi/coinsph-listenkey-openapi.json, openapi/coinsph-markets-openapi.json,\n  openapi/coinsph-payment-openapi.json, openapi/coinsph-ramp-openapi.json, openapi/coinsph-spot-openapi.json,\n  openapi/coinsph-sub-account-openapi.json, openapi/coinsph-system-openapi.json, openapi/coinsph-wallet-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 113\n  by_action_class:\n    connected: 50\n    acting: 63\n  by_consequence:\n    read: 50\n    write: 30\n    physical: 33\n  human_in_the_loop_required: 0\noperations:\n- path: /openapi/account/v3/crypto-accounts\n\
  \  method: get\n  operationId: query_crypto_account_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/account\n  method: get\n  operationId: get_account_information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/fiat/v1/account-validation/create\n  method: post\n  operationId: createAccountValidation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/account-validation/status-check\n  method: get\n  operationId: getAccountValidationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/convert/v1/get-supported-trading-pairs\n  method: post\n  operationId: convert_get_supported_trading_pairs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/convert/v1/get-quote\n  method: post\n  operationId: convert_get_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/convert/v1/accept-quote\n\
  \  method: post\n  operationId: convert_accept_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/convert/v1/query-order-history\n  method: post\n  operationId: convert_query_order_history\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/userDataStream\n  method: post\n  operationId: create_listen_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/userDataStream\n  method: put\n  operationId: keepalive_listen_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/userDataStream\n  method: delete\n  operationId: close_listen_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/pairs\n  method: get\n  operationId: get_cryptoasset_trading_pairs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/quote/v1/depth\n  method: get\n  operationId: get_order_book\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/quote/v1/klines\n  method: get\n  operationId: get_kline_candlestick_data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/quote/v1/ticker/24hr\n  method: get\n  operationId: get_24hr_ticker_price_change_statistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/quote/v1/ticker/price\n  method: get\n  operationId: get_latest_price_for_symbol\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/quote/v1/ticker/bookTicker\n  method: get\n  operationId: get_best_price_quantity_on_order_book\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/quote/v1/trades\n  method: get\n  operationId: get_recent_trades_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/quote/v1/avgPrice\n  method: get\n  operationId: get_current_average_price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/fiat/v1/generate_qr_code\n  method: post\n  operationId: generateDynamicQRPH\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/cancel_qr_code\n  method: post\n  operationId: cancelDynamicQRPH\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/generate/static/qr_code\n  method: post\n  operationId: generateStaticQRPH\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/update/qr_code\n\
  \  method: post\n  operationId: updateStaticQRPH\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/get_qr_code/static/list\n  method: get\n  operationId: getStaticQRPHList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/fiat/v1/get_qr_code\n  method: get\n  operationId: getQRPHStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/wallet/v1/deposit/address\n  method: get\n  operationId: getCryptoDepositAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/fiat/v1/checkout/create-checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/checkout/status-check\n  method: get\n  operationId: getCheckoutStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/fiat/v1/checkout/refund\n  method: post\n  operationId: checkoutRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/checkout/refund/status-check\n  method: get\n  operationId: checkoutRefundStatusCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/fiat/v1/auto-debit/token-apply\n  method: post\n  operationId: tokenApply\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/auto-debit/token-query\n  method: post\n  operationId: tokenQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/auto-debit/token-remove\n  method: post\n  operationId: removePaymentToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/auto-debit/token-pay\n  method: post\n  operationId: payWithToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/support-channel\n  method: post\n  operationId: getSupportChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/decode/kyb_qr_code\n  method: post\n  operationId: decodeQRPH\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/cash-out\n  method: post\n  operationId: initiateCashOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/wallet/v1/withdraw/apply\n  method: post\n  operationId: cryptoApplyWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/refund/pay-in-refund\n  method: post\n  operationId: cashInRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /openapi/fiat/refund/account\n  method: get\n  operationId: getPayerAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/fiat/v1/apply/merchant_bill\n  method: post\n  operationId: applyForReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/download/merchant_bill\n  method: get\n  operationId: retrieveReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/convert/v1/get-supported-trading-pairs\n  method: post\n  operationId: getSupportedConvertTradingPairs\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/convert/v1/get-quote\n  method: post\n  operationId: convertFetchQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/convert/v1/accept-quote\n  method: post\n  operationId: convertAcceptQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /openapi/otc-trade/v1/get-supported-trading-pairs\n  method: post\n  operationId: getOTCSupportedTradingPairs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/otc-trade/v1/create-rfq\n  method: post\n  operationId: createRFQ\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/otc-trade/v1/accept-rfq\n  method: post\n  operationId: acceptRFQ\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/otc-trade/v1/manual-settle\n  method: post\n  operationId: manualSettle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/fiat/v1/details\n  method: get\n  operationId: getOrderDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/fiat/v2/history\n  method: post\n  operationId:\
  \ getFiatOrderHistoryV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/account\n  method: get\n  operationId: getAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/transfer/v3/transfers\n  method: post\n  operationId: p2pTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /openapi/v1/user/ip\n  method: get\n  operationId: getUserIP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/virtual-account/create\n  method: post\n  operationId: createVirtualAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/virtual-account/update\n  method: post\n  operationId: updateVirtualAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/virtual-account/details\n\
  \  method: post\n  operationId: getVirtualAccountDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/virtual-account/list\n  method: post\n  operationId: listVirtualAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/virtual-account/reactivate\n  method: post\n  operationId: reactivateVirtualAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/virtual-account/deactivate\n  method: post\n  operationId: deactivateVirtualAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/virtual-account/order/list\n  method: post\n  operationId: listVirtualAccountTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/virtual-account/check-network\n  method: post\n  operationId: checkVirtualAccountNetwork\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/scan-to-pay/payment-preview\n  method: post\n  operationId: paymentQRCodeDecode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/scan-to-pay/payment-execution\n  method: post\n  operationId: executeScanToPayPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/scan-to-pay/get-payment-result\n  method: get\n  operationId: getScanToPayPaymentResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/account/create-account\n  method: post\n  operationId: createKycAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/account/get-create-account-request\n  method: get\n  operationId: getCreateAccountRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /openapi/ramp/v1/paymentConfigurations\n  method: post\n  operationId: getRampPaymentConfigurations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/ramp/v1/trialPrice\n  method: post\n  operationId: getRampTrialPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/ramp/v1/confirmOnChainFunding\n  method: post\n  operationId: confirmOnChainFunding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/ramp/v1/orderDetail\n  method: post\n  operationId: getRampOrderDetail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/ramp/callback\n  method: post\n  operationId: rampOrderStatusCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /openapi/ramp/outbound/initOnChainFund\n  method: post\n  operationId: initOnChainFund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/exchangeInfo\n  method: get\n  operationId: get_exchange_info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/order/test\n  method: post\n  operationId: test_new_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/order\n  method: post\n  operationId: create_new_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/order\n  method: get\n  operationId: query_order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/order\n  method: delete\n  operationId: cancel_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/openOrders\n  method: get\n  operationId: get_open_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/openOrders\n  method: delete\n  operationId: cancel_all_open_orders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/order/cancelReplace\n  method: post\n  operationId: cancel_replace_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/historyOrders\n  method: get\n  operationId: get_history_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/getHistoryOrdersByUpdateTime\n  method: get\n  operationId: get_history_orders_by_update_time\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/myTrades\n  method: get\n  operationId: get_my_trades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/asset/transaction/history\n  method: get\n  operationId: get_transaction_history\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/asset/tradeFee\n  method: get\n  operationId: get_trade_fee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/sub-account/create\n  method: post\n  operationId: create_virtual_sub_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/sub-account/list\n  method: get\n  operationId: query_sub_account_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/sub-account/asset\n  method: get\n  operationId:\
  \ query_sub_account_assets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/fund-collect/collect-from-sub-account\n  method: post\n  operationId: collect_sub_account_assets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/fund-collect/get-fund-record\n  method: get\n  operationId: retrieve_asset_collection_records\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/sub-account/apikey/ip-restriction\n  method: get\n  operationId: get_sub_account_ip_restriction\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/sub-account/apikey/add-ip-restriction\n  method: post\n  operationId: add_sub_account_ip_restriction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/sub-account/apikey/delete-ip-restriction\n  method: post\n  operationId: delete_sub_account_ip_restriction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/sub-account/transfer/sub-history\n  method: get\n  operationId: get_sub_account_transfer_history\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/sub-account/transfer/sub-to-master\n  method: post\n  operationId: post_sub_account_transfer_to_master\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/sub-account/transfer/universal-transfer\n  method: post\n  operationId: post_sub_account_universal_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v\n\n# --- truncated at 32 KB (35 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/agentic-access/coinsph-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/agentic-access/coinsph-agentic-access.yml
summary_line: 113 operations · 63 acting
tags:
- Company
- Crypto
- Cryptocurrency Exchange
- Payments
- Fintech
- Wallet
- Philippines
- Trading
---
