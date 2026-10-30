---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 25
api_specs:
- filename: snaptrade-account-information-api-openapi.yml
  format: yaml
  label: SnapTrade Account Information API
  slug: snaptrade-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snaptrade/refs/heads/main/openapi/snaptrade-account-information-api-openapi.yml
- filename: snaptrade-api-status-api-openapi.yml
  format: yaml
  label: SnapTrade API Status API
  slug: snaptrade-api-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snaptrade/refs/heads/main/openapi/snaptrade-api-status-api-openapi.yml
- filename: snaptrade-authentication-api-openapi.yml
  format: yaml
  label: SnapTrade Authentication API
  slug: snaptrade-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snaptrade/refs/heads/main/openapi/snaptrade-authentication-api-openapi.yml
- filename: snaptrade-connections-api-openapi.yml
  format: yaml
  label: SnapTrade Connections API
  slug: snaptrade-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snaptrade/refs/heads/main/openapi/snaptrade-connections-api-openapi.yml
- filename: snaptrade-management-api-openapi.yml
  format: yaml
  label: SnapTrade Management API
  slug: snaptrade-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snaptrade/refs/heads/main/openapi/snaptrade-management-api-openapi.yml
- filename: snaptrade-reference-data-api-openapi.yml
  format: yaml
  label: SnapTrade Reference Data API
  slug: snaptrade-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snaptrade/refs/heads/main/openapi/snaptrade-reference-data-api-openapi.yml
- filename: snaptrade-trading-api-openapi.yml
  format: yaml
  label: SnapTrade Trading API
  slug: snaptrade-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snaptrade/refs/heads/main/openapi/snaptrade-trading-api-openapi.yml
consequence_counts:
  physical: 12
  read: 25
  safety-critical: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Snaptrade Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /authorizations/{authorizationId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /snapTrade/resetUserSecret
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/trading/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/trading/complex
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/trading/crypto
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/trading/crypto/preview
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/trading/options
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/trading/replace
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /snapTrade/deleteUser
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /snapTrade/login
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /snapTrade/registerUser
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trade/impact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trade/place
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trade/{tradeId}
operation_count: 42
overview: 'SnapTrade exposes 42 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 3 write, 12 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SnapTrade
provider_slug: snaptrade
slug: snaptrade-agentic-access
source_filename: snaptrade-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/snaptrade-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 25\n    acting: 17\n  by_consequence:\n    read: 25\n    physical: 12\n    safety-critical: 2\n    write: 3\n  human_in_the_loop_required: 2\noperations:\n- path: /\n  method: get\n  operationId: ApiStatus_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snapTrade/listUsers\n  method: get\n  operationId: Authentication_listSnapTradeUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /snapTrade/registerUser\n  method: post\n  operationId: Authentication_registerSnapTradeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /snapTrade/deleteUser\n  method: delete\n  operationId: Authentication_deleteSnapTradeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /snapTrade/login\n  method: post\n  operationId: Authentication_loginSnapTradeUser\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /snapTrade/resetUserSecret\n  method: post\n  operationId: Authentication_resetSnapTradeUserSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /snapTrade/partners\n  method: get\n  operationId: ReferenceData_getPartnerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/stats\n  method:\
  \ get\n  operationId: Management_getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snapTrade/stats\n  method: get\n  operationId: Management_getStatsLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/all\n  method: get\n  operationId: AccountInformation_listAllUserAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/details\n  method: get\n  operationId: AccountInformation_getAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/balances\n  method: get\n  operationId: AccountInformation_getUserAccountBalance\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/positions/all\n  method: get\n  operationId: AccountInformation_getAllAccountPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/orders\n  method: get\n  operationId: AccountInformation_getUserAccountOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/balanceHistory\n  method: get\n  operationId: AccountInformation_getAccountBalanceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/recentOrders\n  method: get\n  operationId:\
  \ AccountInformation_getUserAccountRecentOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/activities\n  method: get\n  operationId: AccountInformation_getAccountActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/quotes\n  method: get\n  operationId: Trading_getUserAccountQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/symbols\n  method: post\n  operationId: ReferenceData_symbolSearchUserAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations\n  method: get\n  operationId:\
  \ Connections_listBrokerageAuthorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/{authorizationId}\n  method: get\n  operationId: Connections_detailBrokerageAuthorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connection/{connectionId}\n  method: delete\n  operationId: Connections_deleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorizations/{authorizationId}/refresh\n  method: post\n  operationId: Connections_refreshBrokerageAuthorization\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorizations/{authorizationId}/transactions/sync\n  method: post\n  operationId: Connections_syncBrokerageAuthorizationTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorizations/{authorizationId}/disable\n  method: post\n  operationId: Connections_disableBrokerageAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /connections/{connectionId}/accounts\n  method: get\n  operationId: Connections_listConnectionAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brokerages/{slug}/instruments\n  method: get\n  operationId: ReferenceData_listAllBrokerageInstruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /symbols\n  method: post\n  operationId: ReferenceData_getSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /symbols/{query}\n  method: get\n  operationId: ReferenceData_getSymbolsByTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /trade/place\n  method: post\n  operationId: Trading_placeForceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/trading/complex\n  method: post\n  operationId: Trading_placeComplexOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/trading/replace\n  method: post\n  operationId: Trading_replaceOrder\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trade/impact\n  method: post\n  operationId: Trading_getOrderImpact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trade/{tradeId}\n  method: post\n  operationId: Trading_placeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/orders/details\n  method: post\n  operationId: AccountInformation_getUserAccountOrderDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/trading/crypto\n  method: post\n  operationId: Trading_placeCryptoOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/trading/cancel\n  method: post\n  operationId: Trading_cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/trading/crypto/preview\n  method: post\n  operationId: Trading_previewCryptoOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/trading/instruments/cryptocurrencyPairs\n  method: get\n  operationId: Trading_searchCryptocurrencyPairInstruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /accounts/{accountId}/trading/instruments/cryptocurrencyPairs/{instrumentSymbol}/quote\n  method: get\n  operationId: Trading_getCryptocurrencyPairQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/trading/options/impact\n  method: post\n  operationId: Trading_getOptionImpact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/trading/options\n  method: post\n  operationId: Trading_placeMlegOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snaptrade/refs/heads/main/agentic-access/snaptrade-agentic-access.yml
summary_line: 42 operations · 17 acting · 2 human-in-the-loop
tags:
- Company
- Fintech
- Brokerage
- Trading
---
