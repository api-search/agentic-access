---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 33
api_specs:
- filename: banno-consumer-api-openapi.yml
  format: yaml
  label: Banno Consumer API
  slug: banno-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-consumer-api-openapi.yml
- filename: banno-admin-api-openapi.yml
  format: yaml
  label: Banno Admin API
  slug: banno-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-admin-api-openapi.yml
- filename: banno-plugin-framework-openapi.yml
  format: yaml
  label: Banno Plugin Framework
  slug: banno-plugin-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-plugin-framework-openapi.yml
- filename: banno-authentication-framework-openapi.yml
  format: yaml
  label: Banno Authentication Framework
  slug: banno-authentication-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-authentication-framework-openapi.yml
- filename: jxchange-rest-openapi.yml
  format: yaml
  label: jXchange REST
  slug: jxchange-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/jxchange-rest-openapi.yml
- filename: jack-henry-payments-openapi.yml
  format: yaml
  label: Jack Henry Payments
  slug: jack-henry-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/jack-henry-payments-openapi.yml
- filename: enterprise-event-system-asyncapi.yml
  format: yaml
  label: Enterprise Event System
  slug: enterprise-event-system
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/asyncapi/enterprise-event-system-asyncapi.yml
consequence_counts:
  physical: 12
  read: 33
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jack Henry Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a/consumer/api/v0/users/{userId}/bill-pay/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a/consumer/api/v0/users/{userId}/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a/consumer/api/v0/users/{userId}/wire-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a/consumer/api/v0/users/{userId}/zelle/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/ach/credits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/ach/debits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/bill-pay/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/cards/authorizations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/orchestrator/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/p2p/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/rdc/deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/wires
operation_count: 52
overview: 'Jack Henry & Associates exposes 52 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read, 7 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jack Henry & Associates
provider_slug: jack-henry
slug: jack-henry-agentic-access
source_filename: jack-henry-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/banno-admin-api-openapi.yml, openapi/banno-authentication-framework-openapi.yml,\n  openapi/banno-consumer-api-openapi.yml, openapi/banno-plugin-framework-openapi.yml, openapi/jack-henry-payments-openapi.yml,\n  openapi/jxchange-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 33\n    acting: 19\n  by_consequence:\n    read: 33\n    write: 7\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /a/mobile/api/v0/institutions/{institutionId}/abilities\n  method: get\n  operationId: getInstitutionAbilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /a/mobile/api/v0/institutions/{institutionId}/consumers\n  method: get\n  operationId: listConsumers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/mobile/api/v0/institutions/{institutionId}/consumers/{consumerId}\n  method: get\n  operationId: getConsumer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/mobile/api/v0/institutions/{institutionId}/consumers/{consumerId}/contact-info\n  method: put\n  operationId: updateContactInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a/mobile/api/v0/institutions/{institutionId}/segments\n\
  \  method: get\n  operationId: listSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/mobile/api/v0/institutions/{institutionId}/segments\n  method: post\n  operationId: createSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a/mobile/api/v0/institutions/{institutionId}/ads\n  method: get\n  operationId: listAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/mobile/api/v0/institutions/{institutionId}/ads\n  method: post\n  operationId: createAd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a/mobile/api/v0/institutions/{institutionId}/plugins\n  method: get\n  operationId: listPlugins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/mobile/api/v0/institutions/{institutionId}/plugins/{pluginId}\n  method: put\n  operationId: updatePlugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a/mobile/api/v0/institutions/{institutionId}/reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/mobile/api/v0/institutions/{institutionId}/high-risk-actions\n  method: get\n  operationId: listHighRiskActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/mobile/api/v0/institutions/{institutionId}/history\n  method: get\n  operationId: listHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/mobile/api/v0/institutions/{institutionId}/offline-mode\n  method: put\n  operationId: setOfflineMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /a/oidc/.well-known/openid-configuration\n  method: get\n  operationId: getDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/oidc/.well-known/jwks.json\n  method: get\n  operationId: getJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/oidc/authorize\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/oidc/token\n  method: post\n  operationId: exchangeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /a/oidc/userinfo\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/user.profile.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/accounts.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/accounts.detail.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/accounts/{accountId}/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/transactions.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/transactions.detail.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/transfers\n  method: get\n  operationId: listTransfers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/transfers.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/transfers\n  method: post\n  operationId: createTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://api.banno.com/consumer/auth/transfers.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a/consumer/api/v0/users/{userId}/bill-pay/payees\n  method: get\n  operationId: listPayees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/bill-pay.readonly\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/bill-pay/payments\n  method: post\n  operationId: createBillPayPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://api.banno.com/consumer/auth/bill-pay.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a/consumer/api/v0/users/{userId}/alerts\n  method: get\n  operationId: listAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/alerts.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/cards\n  method: get\n  operationId: listCards\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/cards.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://api.banno.com/consumer/auth/messages.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/users/{userId}/wire-transfers\n  method: post\n  operationId: createWireTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://api.banno.com/consumer/auth/wire-transfers.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /a/consumer/api/v0/users/{userId}/zelle/payments\n  method: post\n  operationId: sendZellePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://api.banno.com/consumer/auth/zelle.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a/consumer/api/v0/institutions/{institutionId}\n  method: get\n  operationId: getInstitution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a/consumer/api/v0/routing-numbers/{routingNumber}\n  method: get\n  operationId: lookupRoutingNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /plugins/api/v0/plugins/{pluginId}/manifest\n  method: get\n  operationId: getPluginManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plugins/api/v0/plugins/{pluginId}/bridge/token\n  method: post\n  operationId: exchangeBridgeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plugins/api/v0/context\n  method: get\n  operationId: getPluginUserContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/v1/ach/credits\n  method: post\n  operationId: originateAchCredit\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/ach/debits\n  method: post\n  operationId: originateAchDebit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/wires\n  method: post\n  operationId: sendWire\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/bill-pay/payments\n  method: post\n  operationId: submitBillPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/rdc/deposits\n  method: post\n  operationId: submitRemoteDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/cards/authorizations\n  method: post\n  operationId:\
  \ authorizeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/p2p/transfers\n  method: post\n  operationId: sendP2P\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/orchestrator/payments\n  method: post\n  operationId: routePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    \
  \  exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jxchange/v1/customers\n  method: get\n  operationId: searchCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jxchange/v1/customers/{customerId}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jxchange/v1/deposit-accounts/{accountNumber}\n  method: get\n  operationId: getDepositAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jxchange/v1/loan-accounts/{accountNumber}\n  method: get\n  operationId: getLoanAccount\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jxchange/v1/accounts/{accountNumber}/transactions\n  method: get\n  operationId: listAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jxchange/v1/general-ledger/{glAccountNumber}\n  method: get\n  operationId: getGlAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/agentic-access/jack-henry-agentic-access.yml
summary_line: 52 operations · 19 acting
tags:
- Financial Services
- Banking
- Core Banking
- Digital Banking
- Payments
- Lending
- Fraud
- Open Banking
- Community Banks
- Credit Unions
- Fintech
- OAuth
- OpenID Connect
---
