---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 34
api_specs:
- filename: bvnk-address-api-openapi.yml
  format: yaml
  label: BVNK Address API
  slug: bvnk-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-address-api-openapi.yml
- filename: bvnk-asset-pool-api-openapi.yml
  format: yaml
  label: BVNK Asset Pool API
  slug: bvnk-asset-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-asset-pool-api-openapi.yml
- filename: bvnk-channels-api-openapi.yml
  format: yaml
  label: BVNK Channels API
  slug: bvnk-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-channels-api-openapi.yml
- filename: bvnk-currencies-api-openapi.yml
  format: yaml
  label: BVNK Currencies API
  slug: bvnk-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-currencies-api-openapi.yml
- filename: bvnk-export-api-openapi.yml
  format: yaml
  label: BVNK Export API
  slug: bvnk-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-export-api-openapi.yml
- filename: bvnk-fee-api-openapi.yml
  format: yaml
  label: BVNK Fee API
  slug: bvnk-fee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-fee-api-openapi.yml
- filename: bvnk-key-pair-api-openapi.yml
  format: yaml
  label: BVNK Key Pair API
  slug: bvnk-key-pair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-key-pair-api-openapi.yml
- filename: bvnk-merchant-ids-api-openapi.yml
  format: yaml
  label: BVNK Merchant IDs API
  slug: bvnk-merchant-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-merchant-ids-api-openapi.yml
- filename: bvnk-network-api-openapi.yml
  format: yaml
  label: BVNK Network API
  slug: bvnk-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-network-api-openapi.yml
- filename: bvnk-payments-api-openapi.yml
  format: yaml
  label: BVNK Payments API
  slug: bvnk-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-payments-api-openapi.yml
- filename: bvnk-return-api-openapi.yml
  format: yaml
  label: BVNK Return API
  slug: bvnk-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-return-api-openapi.yml
- filename: bvnk-screening-api-openapi.yml
  format: yaml
  label: BVNK Screening API
  slug: bvnk-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-screening-api-openapi.yml
- filename: bvnk-trading-and-conversions-api-openapi.yml
  format: yaml
  label: BVNK Trading and Conversions API
  slug: bvnk-trading-and-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-trading-and-conversions-api-openapi.yml
- filename: bvnk-transaction-api-openapi.yml
  format: yaml
  label: BVNK Transaction API
  slug: bvnk-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-transaction-api-openapi.yml
- filename: bvnk-transaction-request-api-openapi.yml
  format: yaml
  label: BVNK Transaction Request API
  slug: bvnk-transaction-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-transaction-request-api-openapi.yml
- filename: bvnk-wallets-api-openapi.yml
  format: yaml
  label: BVNK Wallets API
  slug: bvnk-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/openapi/bvnk-wallets-api-openapi.yml
consequence_counts:
  physical: 3
  read: 34
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bvnk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/pay/summary
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/pay/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /digital/v1/screenings/action
operation_count: 54
overview: 'BVNK exposes 54 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 17 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BVNK
provider_slug: bvnk
slug: bvnk-agentic-access
source_filename: bvnk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: generated\nsource: openapi/bvnk-api-endpoints-openapi-original.yml, openapi/bvnk-layer1-digital-asset-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    connected: 34\n    acting: 20\n  by_consequence:\n    read: 34\n    write: 17\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/currency/crypto\n  method: get\n  operationId: listCurrenciesCrypto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/currency/fiat\n  method: get\n  operationId: listCurrenciesFiat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/currency/deposit\n  method: get\n  operationId: listCurrenciesDeposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/merchant\n  method: get\n  operationId: merchantIdList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/merchant\n  method: post\n  operationId: merchantIdCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pay/summary\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pay/summary\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - merchant\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pay/{uuid}/summary\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pay/validate\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/channel\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/channel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/channel/{uuid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/channel/payment/{uuid}\n  method: get\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/channel/payment\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wallet\n  method: get\n  operationId: walletList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wallet\n  method: post\n  operationId: walletCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/wallet/{id}\n\
  \  method: get\n  operationId: walletRGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wallet/balances\n  method: get\n  operationId: walletBalanceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/transaction/report\n  method: get\n  operationId: transactionReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quote\n  method: post\n  operationId: quoteCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quote/accept/{uuid}\n  method: put\n  operationId: quoteAccept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quote/{uuid}\n  method: get\n  operationId: quoteRead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quote/{merchantId}\n  method: get\n  operationId: quoteList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - x-example\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/screenings/action\n \
  \ method: put\n  operationId: manuallyActionHeldTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - screenings:edit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/transaction-requests\n  method: get\n  operationId: listTransactionRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/transaction-requests\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - transactions:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/transaction-claims\n  method: post\n  operationId: claimTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - transactions:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/staking-requests\n  method: post\n  operationId: createStakingTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - transactions:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/returns\n  method: post\n  operationId: createReturnTransactionRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - transactions:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/key-pairs\n  method: get\n  operationId: listKeyPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - keypairs:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/key-pairs\n  method: post\n  operationId: createKeyPair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - keypairs:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/fee-estimate\n  method:\
  \ post\n  operationId: estimateTransactionFee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - fee-estimate:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/exports\n  method: get\n  operationId: getExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ${exports.read-scope:exports:view}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/exports\n  method: post\n  operationId: createBalanceExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - exports:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /digital/v1/asset-pools\n  method: get\n  operationId: listAssetPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - asset-pools:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/asset-pools\n  method: post\n  operationId: createAssetPool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - asset-pools:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/addresses\n  method: get\n  operationId: listAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - addresses:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/addresses\n  method: post\n  operationId: createAddress\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - addresses:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/addresses/validate\n  method: post\n  operationId: validateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - addresses:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/asset-pools/{assetPoolId}\n  method: delete\n  operationId: deleteAssetPool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - asset-pools:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/asset-pools/{assetPoolId}\n  method: get\n  operationId: getAssetPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - asset-pools:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/asset-pools/{assetPoolId}\n  method: patch\n  operationId: updateAssetPool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - asset-pools:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/v1/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:view\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/transactions/{transactionId}\n  method: get\n  operationId: getTransactionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/transaction-requests/{requestId}\n  method: get\n  operationId: getTransactionRequestById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/screenings\n  method: get\n  operationId: listScreenings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - screenings:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/networks\n  method: get\n  operationId: getNetworks\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - networks:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/key-pairs/{keyPairId}\n  method: get\n  operationId: getKeyPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - keypairs:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/exports/{id}\n  method: get\n  operationId: getExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ${exports.read-scope:exports:view}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/asset-pools/{assetPoolId}/max-withdrawable-amount\n  method: get\n  operationId: getAssetPoolMaxWithdrawableAmount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - asset-pools:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/asset-pools/{assetPoolId}/balances\n\
  \  method: get\n  operationId: getAssetPoolBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - asset-pools:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/asset-pools/summary\n  method: get\n  operationId: getAssetPoolSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - asset-pools:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/addresses/{addressId}\n  method: get\n  operationId: getAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - addresses:view\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/v1/addresses/{addressId}/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - addresses:view\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bvnk/refs/heads/main/agentic-access/bvnk-agentic-access.yml
summary_line: 54 operations · 20 acting
tags:
- Company
- Payments
- Stablecoins
- Cryptocurrency
- Wallets
- Virtual Accounts
- Cross-Border Payments
- Financial-Services
- Cards
- Digital Assets
- Banking
- Compliance
---
