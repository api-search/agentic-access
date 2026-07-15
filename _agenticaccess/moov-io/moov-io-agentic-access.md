---
acting_count: 39
action_class_counts:
  acting: 39
  connected: 46
api_specs:
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Accounts API
  slug: moov-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Representatives API
  slug: moov-io-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Capabilities API
  slug: moov-io-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Underwriting API
  slug: moov-io-underwriting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Bank Accounts API
  slug: moov-io-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Cards API
  slug: moov-io-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Wallets API
  slug: moov-io-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Payment Methods API
  slug: moov-io-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Transfers API
  slug: moov-io-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Refunds API
  slug: moov-io-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Sweeps API
  slug: moov-io-sweeps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Disputes API
  slug: moov-io-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Card Issuing API
  slug: moov-io-card-issuing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
- filename: moov-io-openapi.yml
  format: yaml
  label: Moov Institutions API
  slug: moov-io-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/openapi/moov-io-openapi.yml
consequence_counts:
  physical: 10
  read: 46
  safety-critical: 2
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Moov Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /accounts/{accountID}/capabilities/{capabilityID}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /accounts/{accountID}/cards/{cardID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountID}/bank-accounts/{bankAccountID}/micro-deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountID}/bank-accounts/{bankAccountID}/micro-deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountID}/transfer-config
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountID}/transfer-config
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountID}/transfer-options
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountID}/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /accounts/{accountID}/transfers/{transferID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountID}/transfers/{transferID}/cancellations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountID}/transfers/{transferID}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountID}/transfers/{transferID}/reversals
operation_count: 85
overview: 'Moov exposes 85 API operations that an AI agent could call, of which 39 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read, 27 write, 10 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Moov
provider_slug: moov-io
slug: moov-io-agentic-access
source_filename: moov-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/moov-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 85\n  by_action_class:\n    acting: 39\n    connected: 46\n  by_consequence:\n    write: 27\n    read: 46\n    safety-critical: 2\n    physical: 10\n  human_in_the_loop_required: 2\noperations:\n- path: /accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}\n  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}\n  method: delete\n  operationId: disconnectAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/connected-accounts\n  method: get\n  operationId: listConnectedAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tos-token\n  method: get\n  operationId: getTermsOfServiceToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/representatives\n  method: post\n  operationId: createRepresentative\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/representatives\n  method: get\n  operationId: listRepresentatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/representatives/{representativeID}\n  method: get\n  operationId: getRepresentative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/representatives/{representativeID}\n  method: patch\n  operationId: updateRepresentative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/representatives/{representativeID}\n  method: delete\n  operationId: deleteRepresentative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/capabilities\n  method: post\n  operationId: requestCapabilities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/capabilities\n  method:\
  \ get\n  operationId: listCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/capabilities/{capabilityID}\n  method: get\n  operationId: getCapability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/capabilities/{capabilityID}\n  method: delete\n  operationId: disableCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /accounts/{accountID}/underwriting\n  method: get\n  operationId: getUnderwriting\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/underwriting\n  method: put\n  operationId: upsertUnderwriting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/bank-accounts\n  method: post\n  operationId: linkBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/bank-accounts\n  method: get\n  operationId: listBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/bank-accounts/{bankAccountID}\n  method: get\n  operationId: getBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/bank-accounts/{bankAccountID}\n  method: delete\n  operationId: deleteBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/bank-accounts/{bankAccountID}/verify\n  method: post\n  operationId: initiateBankAccountVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/bank-accounts/{bankAccountID}/verify\n  method: put\n  operationId: completeBankAccountVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/bank-accounts/{bankAccountID}/verify\n  method: get\n  operationId: getBankAccountVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/bank-accounts/{bankAccountID}/micro-deposits\n  method: post\n  operationId: initiateMicroDeposits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/bank-accounts/{bankAccountID}/micro-deposits\n  method: put\n  operationId: completeMicroDeposits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/cards\n  method: post\n  operationId: linkCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/cards\n  method: get\n  operationId: listCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/cards/{cardID}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/cards/{cardID}\n  method: patch\n  operationId: updateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/cards/{cardID}\n  method: delete\n  operationId: disableCard\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /accounts/{accountID}/wallets\n  method: post\n  operationId: createWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/wallets\n  method: get\n  operationId: listWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/wallets/{walletID}\n  method: get\n  operationId: getWallet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/wallets/{walletID}\n  method: patch\n  operationId: updateWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/wallets/{walletID}/transactions\n  method: get\n  operationId: listWalletTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/wallets/{walletID}/transactions/{transactionID}\n  method: get\n  operationId: getWalletTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /accounts/{accountID}/adjustments\n  method: get\n  operationId: listAdjustments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/adjustments/{adjustmentID}\n  method: get\n  operationId: getAdjustment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/payment-methods\n  method: get\n  operationId: listPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/payment-methods/{paymentMethodID}\n  method: get\n  operationId: getPaymentMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /accounts/{accountID}/transfers\n  method: post\n  operationId: createTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/transfers\n  method: get\n  operationId: listTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transfers/{transferID}\n  method: get\n  operationId: getTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transfers/{transferID}\n  method: patch\n  operationId: updateTransferMetadata\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/transfer-options\n  method: post\n  operationId: createTransferOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/transfer-config\n  method: post\n  operationId: createTransferConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/transfer-config\n  method: get\n  operationId: getTransferConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transfer-config\n  method: put\n  operationId: updateTransferConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/transfers/{transferID}/cancellations\n  method: post\n  operationId: cancelTransfer\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/transfers/{transferID}/cancellations/{cancellationID}\n  method: get\n  operationId: getCancellation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transfers/{transferID}/refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /accounts/{accountID}/transfers/{transferID}/refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transfers/{transferID}/refunds/{refundID}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/transfers/{transferID}/reversals\n  method: post\n  operationId: createReversal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/sweep-configs\n\
  \  method: post\n  operationId: createSweepConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/sweep-configs\n  method: get\n  operationId: listSweepConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/sweep-configs/{sweepConfigID}\n  method: get\n  operationId: getSweepConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/sweep-configs/{sweepConfigID}\n  method: patch\n  operationId: updateSweepConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/wallets/{walletID}/sweeps\n  method: get\n  operationId: listSweeps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/wallets/{walletID}/sweeps/{sweepID}\n  method: get\n  operationId: getSweep\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/disputes\n  method: get\n  operationId: listDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/disputes/{disputeID}\n  method: get\n\
  \  operationId: getDispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/disputes/{disputeID}/accept\n  method: post\n  operationId: acceptDispute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/disputes/{disputeID}/evidence-file\n  method: post\n  operationId: uploadDisputeEvidenceFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/disputes/{disputeID}/evidence-text\n\
  \  method: post\n  operationId: uploadDisputeEvidenceText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/disputes/{disputeID}/evidence/submit\n  method: post\n  operationId: submitDisputeEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/disputes/{disputeID}/evidence\n  method: get\n  operationId: listDisputeEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /accounts/{accountID}/disputes/{disputeID}/evidence/{evidenceID}\n  method: get\n  operationId: getDisputeEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountID}/disputes/{disputeID}/evidence/{evidenceID}\n  method: patch\n  operationId: updateDisputeEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/disputes/{disputeID}/evidence/{evidenceID}\n  method: delete\n  operationId: deleteDisputeEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountID}/disputes/{disputeID}/evidence/{evidenceID}/data\n  method: get\n  operationId: getDisputeEvidenceData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuing/{accountID}/cards\n  method: post\n  operationId: createIssuedCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issuing/{accountID}/cards\n  method: get\n  operationId: listIssuedCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuing/{accountID}/cards/{issuedCardID}\n \
  \ method: get\n  operationId: getIssuedCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuing/{accountID}/cards/{issuedCardID}\n  method: patch\n  operationId: updateIssuedCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issuing/{accountID}/cards/{issuedCardID}/details\n  method: get\n  operationId: getIssuedCardDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuing/{accountID}/authorizations\n  method: get\n  operationId: listAuthorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuing/{accountID}/authorizations/{authorizationID}\n  method: get\n  operationId: getAuthorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuing/{accountID}/authorizations/{authorizationID}/events\n  method: get\n  operationId: listAuthorizationEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuing/{accountID}/card-transactions\n  method: get\n  operationId: listCardTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuing/{accountID}/card-transactions/{cardTransactionID}\n  method: get\n  operationId: getCardTransaction\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /institutions\n  method: get\n  operationId: getInstitutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moov-io/refs/heads/main/agentic-access/moov-io-agentic-access.yml
summary_line: 85 operations · 39 acting · 2 human-in-the-loop
tags:
- Payments
- Money Movement
- Fintech
- ACH
- RTP
- Cards
- Wallets
- Embedded Finance
---
