---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 26
api_specs:
- filename: mesh-connect-assets-api-openapi.yml
  format: yaml
  label: Mesh Connect Assets API
  slug: mesh-connect-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-assets-api-openapi.yml
- filename: mesh-connect-auth-token-api-openapi.yml
  format: yaml
  label: Mesh Connect Auth token API
  slug: mesh-connect-auth-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-auth-token-api-openapi.yml
- filename: mesh-connect-balance-api-openapi.yml
  format: yaml
  label: Mesh Connect Balance API
  slug: mesh-connect-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-balance-api-openapi.yml
- filename: mesh-connect-brokeraccountdetail-api-openapi.yml
  format: yaml
  label: Mesh Connect BrokerAccountDetail API
  slug: mesh-connect-brokeraccountdetail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-brokeraccountdetail-api-openapi.yml
- filename: mesh-connect-main-clients-api-openapi.yml
  format: yaml
  label: Mesh Connect Main Clients API
  slug: mesh-connect-main-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-main-clients-api-openapi.yml
- filename: mesh-connect-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Connect Managed Account Authentication API
  slug: mesh-connect-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-managed-account-authentication-api-openapi.yml
- filename: mesh-connect-managed-transfers-api-openapi.yml
  format: yaml
  label: Mesh Connect Managed Transfers API
  slug: mesh-connect-managed-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-managed-transfers-api-openapi.yml
- filename: mesh-connect-portfolio-api-openapi.yml
  format: yaml
  label: Mesh Connect Portfolio API
  slug: mesh-connect-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-portfolio-api-openapi.yml
- filename: mesh-connect-registered-clients-api-openapi.yml
  format: yaml
  label: Mesh Connect Registered Clients API
  slug: mesh-connect-registered-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-registered-clients-api-openapi.yml
- filename: mesh-connect-self-managed-account-authentication-api-openapi.yml
  format: yaml
  label: Mesh Connect Self Managed Account Authentication API
  slug: mesh-connect-self-managed-account-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-self-managed-account-authentication-api-openapi.yml
- filename: mesh-connect-transactions-api-openapi.yml
  format: yaml
  label: Mesh Connect Transactions API
  slug: mesh-connect-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-transactions-api-openapi.yml
- filename: mesh-connect-transfers-api-openapi.yml
  format: yaml
  label: Mesh Connect Transfers API
  slug: mesh-connect-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-transfers-api-openapi.yml
consequence_counts:
  physical: 12
  read: 26
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mesh Connect Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transactions/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transactions/preview/{side}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transactions/{side}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers/address/get
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers/details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers/managed/address/get
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers/managed/configure
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers/managed/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers/managed/preview
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers/managed/quote
operation_count: 50
overview: 'Mesh Connect exposes 50 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 12 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mesh Connect
provider_slug: mesh-connect
slug: mesh-connect-agentic-access
source_filename: mesh-connect-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/mesh-connect-assets-api-openapi.yml, openapi/mesh-connect-auth-token-api-openapi.yml,\n  openapi/mesh-connect-balance-api-openapi.yml, openapi/mesh-connect-brokeraccountdetail-api-openapi.yml,\n  openapi/mesh-connect-main-clients-api-openapi.yml, openapi/mesh-connect-managed-account-authentication-api-openapi.yml,\n  openapi/mesh-connect-managed-transfers-api-openapi.yml, openapi/mesh-connect-portfolio-api-openapi.yml,\n  openapi/mesh-connect-registered-clients-api-openapi.yml, openapi/mesh-connect-self-managed-account-authentication-api-openapi.yml,\n  openapi/mesh-connect-transactions-api-openapi.yml, openapi/mesh-connect-transfers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n\
  \  operations: 50\n  by_action_class:\n    connected: 26\n    acting: 24\n  by_consequence:\n    read: 26\n    write: 12\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/assets/{assetType}\n  method: get\n  operationId: getApiV1AssetsByAssetType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/assets/equity/{symbol}/price\n  method: get\n  operationId: getApiV1AssetsEquityBySymbolPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/v1/Token\n  method: post\n  operationId: postAdminApiV1Token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/balance/get\n  method: post\n  operationId: postApiV1BalanceGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/balance/portfolio\n  method: get\n  operationId: getApiV1BalancePortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/verify\n  method: post\n  operationId: postApiV1AccountVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/v1/Client/callbackUrls\n  method: get\n  operationId: getAdminApiV1ClientCallbackUrls\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/v1/Client/callbackUrls\n  method: post\n  operationId: postAdminApiV1ClientCallbackUrls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cataloglink\n  method: get\n  operationId: getApiV1Cataloglink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cataloglink\n  method: post\n  operationId: postApiV1Cataloglink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/linktoken\n  method:\
  \ post\n  operationId: postApiV1Linktoken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/token/refresh\n  method: post\n  operationId: postApiV1TokenRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account\n  method: delete\n  operationId: deleteApiV1Account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /api/v1/status\n  method: get\n  operationId: getApiV1Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/integrations\n  method: get\n  operationId: getApiV1Integrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transfers/managed/networks\n  method: get\n  operationId: getApiV1TransfersManagedNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transfers/managed/integrations\n  method: get\n  operationId: getApiV1TransfersManagedIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/transfers/managed/tokens\n  method: get\n  operationId: getApiV1TransfersManagedTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transfers/managed/verify\n  method: get\n  operationId: getApiV1TransfersManagedVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transfers/managed/configure\n  method: post\n  operationId: postApiV1TransfersManagedConfigure\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transfers/managed/preview\n  method: post\n\
  \  operationId: postApiV1TransfersManagedPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transfers/managed/execute\n  method: post\n  operationId: postApiV1TransfersManagedExecute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transfers/managed/address/get\n  method: post\n  operationId: postApiV1TransfersManagedAddressGet\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transfers/managed/quote\n  method: post\n  operationId: postApiV1TransfersManagedQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transfers/managed/mesh\n  method: get\n  operationId: getApiV1TransfersManagedMesh\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/holdings/get\n  method: post\n \
  \ operationId: postApiV1HoldingsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/holdings/value\n  method: post\n  operationId: postApiV1HoldingsValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/holdings/portfolio\n  method: get\n  operationId: getApiV1HoldingsPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/v1/SubClient\n  method: get\n  operationId: getAdminApiV1SubClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/v1/SubClient\n  method: post\n  operationId: postAdminApiV1SubClient\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/v1/SubClient/{id}\n  method: get\n  operationId: getAdminApiV1SubClientById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/v1/SubClient/{id}\n  method: put\n  operationId: putAdminApiV1SubClientById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/v1/SubClient/{id}\n  method: delete\n  operationId: deleteAdminApiV1SubClientById\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/v1/SubClient/{id}/logo\n  method: post\n  operationId: postAdminApiV1SubClientByIdLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/v1/SubClient/{id}/logo\n  method: delete\n  operationId: deleteAdminApiV1SubClientByIdLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/authenticationSchemes\n  method: get\n  operationId: getApiV1AuthenticationSchemes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/authenticate\n  method: post\n  operationId: postApiV1Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/authenticate/{brokerType}\n  method: get\n  operationId: getApiV1AuthenticateByBrokerType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/list\n  method: post\n  operationId: postApiV1TransactionsList\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/details\n  method: post\n  operationId: postApiV1TransactionsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/featureList\n  method: post\n  operationId: postApiV1TransactionsFeatureList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/preview/{side}\n  method: post\n  operationId: postApiV1TransactionsPreviewBySide\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions/{side}\n  method: post\n  operationId: postApiV1TransactionsBySide\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions/cancel\n  method: post\n  operationId: postApiV1TransactionsCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions/symbolinfo\n  method: post\n  operationId: postApiV1TransactionsSymbolinfo\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transfers/list\n  method: post\n  operationId: postApiV1TransfersList\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transfers/details\n  method: post\n  operationId: postApiV1TransfersDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transfers\n\
  \  method: post\n  operationId: postApiV1Transfers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transfers/address/get\n  method: post\n  operationId: postApiV1TransfersAddressGet\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transfers/symbol/details\n  method: post\n  operationId: postApiV1TransfersSymbolDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/agentic-access/mesh-connect-agentic-access.yml
summary_line: 50 operations · 24 acting
tags:
- Company
- Crypto Infrastructure
- Crypto Payments
- Digital Assets
- Wallets
- Exchange
- Embedded Finance
- Stablecoins
- Payments
---
