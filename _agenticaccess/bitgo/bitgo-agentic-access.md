---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Wallets API
  slug: bitgo-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Addresses API
  slug: bitgo-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Transactions & Transfers API
  slug: bitgo-transactions-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Keychains & Keys API
  slug: bitgo-keychains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Webhooks API
  slug: bitgo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Wallet Policies API
  slug: bitgo-wallet-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Staking API
  slug: bitgo-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Trading & Settlement (Go Network) API
  slug: bitgo-trading-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Express API
  slug: bitgo-express-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Enterprise & Users API
  slug: bitgo-enterprise-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bitgo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{coin}/wallet/{walletId}/sendcoins
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{coin}/wallet/{walletId}/sendmany
operation_count: 19
overview: 'BitGo exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BitGo
provider_slug: bitgo
slug: bitgo-agentic-access
source_filename: bitgo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bitgo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 11\n    acting: 8\n  by_consequence:\n    read: 11\n    write: 6\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /{coin}/wallet\n  method: get\n  operationId: listWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{coin}/wallet\n  method: post\n  operationId: generateWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{coin}/wallet/{walletId}\n  method: get\n  operationId: getWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{coin}/wallet/{walletId}/address\n  method: get\n  operationId: listWalletAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{coin}/wallet/{walletId}/address\n  method: post\n  operationId: createWalletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{coin}/wallet/{walletId}/sendcoins\n  method: post\n  operationId:\
  \ sendCoins\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{coin}/wallet/{walletId}/sendmany\n  method: post\n  operationId: sendMany\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{coin}/wallet/{walletId}/transfer\n  method: get\n  operationId: listTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /{coin}/wallet/{walletId}/transfer/{transferId}\n  method: get\n  operationId: getTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{coin}/key\n  method: get\n  operationId: listKeychains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{coin}/key\n  method: post\n  operationId: createKeychain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{coin}/wallet/{walletId}/webhooks\n  method: get\n  operationId: listWalletWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /{coin}/wallet/{walletId}/webhooks\n  method: post\n  operationId: addWalletWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{coin}/wallet/{walletId}/policy\n  method: put\n  operationId: updateWalletPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{coin}/wallet/{walletId}/staking/requests\n  method: post\n  operationId: createStakingRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{coin}/wallet/{walletId}/staking/requests\n  method: get\n  operationId: listStakingRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trading/settlements\n  method: get\n  operationId: listSettlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enterprise\n  method: get\n  operationId: listEnterprises\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/agentic-access/bitgo-agentic-access.yml
summary_line: 19 operations · 8 acting
tags:
- Digital Assets
- Custody
- Wallets
- Blockchain
- Crypto
- Staking
- Settlement
---
