---
acting_count: 39
action_class_counts:
  acting: 39
  connected: 13
api_specs:
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Payouts API
  slug: chimoney-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Wallets API
  slug: chimoney-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Multicurrency Wallets API
  slug: chimoney-multicurrency-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Sub-Accounts API
  slug: chimoney-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Redeem API
  slug: chimoney-redeem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Info API
  slug: chimoney-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Accounts API
  slug: chimoney-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
- filename: chimoney-openapi.yml
  format: yaml
  label: Chimoney Payments API
  slug: chimoney-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/openapi/chimoney-openapi.yml
consequence_counts:
  physical: 19
  read: 13
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chimoney Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/accounts/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/multicurrency-wallets/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/multicurrency-wallets/transfer/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payment/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payment/simulate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payment/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/airtime
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/bank
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/bills/ca
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/chimoney
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/gift-card
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/initiate-chimoney
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/interac
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/interledger-wallet-address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/mobile-money
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/process
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/payouts/wallet
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.2/wallets/transfer
operation_count: 52
overview: 'Chimoney exposes 52 API operations that an AI agent could call, of which 39 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 20 write, and 19 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chimoney
provider_slug: chimoney
slug: chimoney-agentic-access
source_filename: chimoney-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chimoney-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    acting: 39\n    connected: 13\n  by_consequence:\n    physical: 19\n    write: 20\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /v0.2/payouts/bank\n  method: post\n  operationId: post_v0.2_payouts_bank\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/mobile-money\n\
  \  method: post\n  operationId: post_v0.2_payouts_mobile-money\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/airtime\n  method: post\n  operationId: post_v0.2_payouts_airtime\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/gift-card\n  method: post\n  operationId: post_v0.2_payouts_gift-card\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/chimoney\n  method: post\n  operationId: post_v0.2_payouts_chimoney\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/wallet\n  method: post\n  operationId: post_v0.2_payouts_wallet\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/interledger-wallet-address\n  method: post\n  operationId: post_v0.2_payouts_interledger-wallet-address\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/interac\n  method: post\n  operationId: post_v0.2_payouts_interac\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/bills/ca\n  method: post\n\
  \  operationId: post_v0.2_payouts_bills_ca\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/initiate-chimoney\n  method: post\n  operationId: post_v0.2_payouts_initiate-chimoney\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/process\n  method: post\n  operationId: post_v0.2_payouts_process\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payouts/status\n  method: post\n  operationId: post_v0.2_payouts_status\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/wallets/list\n  method: post\n  operationId: post_v0.2_wallets_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v0.2/wallets/lookup\n  method: post\n  operationId: post_v0.2_wallets_lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/wallets/transfer\n  method: post\n  operationId: post_v0.2_wallets_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/multicurrency-wallets/create\n  method: post\n  operationId: post_v0.2_multicurrency-wallets_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/multicurrency-wallets/get\n  method: get\n  operationId: get_v0.2_multicurrency-wallets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/multicurrency-wallets/list\n  method: get\n  operationId: get_v0.2_multicurrency-wallets_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/multicurrency-wallets/update\n  method: post\n  operationId: post_v0.2_multicurrency-wallets_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/multicurrency-wallets/transfer\n  method: post\n  operationId: post_v0.2_multicurrency-wallets_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/multicurrency-wallets/transfer/quote\n  method: post\n  operationId: post_v0.2_multicurrency-wallets_transfer_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/sub-account/create\n\
  \  method: post\n  operationId: post_v0.2_sub-account_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/sub-account/get\n  method: get\n  operationId: get_v0.2_sub-account_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/sub-account/list\n  method: get\n  operationId: get_v0.2_sub-account_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/sub-account/update\n  method: post\n  operationId: post_v0.2_sub-account_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/sub-account/delete\n  method: delete\n  operationId: delete_v0.2_sub-account_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/sub-account/community/create\n  method: post\n  operationId: post_v0.2_sub-account_community_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/sub-account/community/members\n  method:\
  \ get\n  operationId: get_v0.2_sub-account_community_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/redeem/any\n  method: post\n  operationId: post_v0.2_redeem_any\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/redeem/chimoney\n  method: post\n  operationId: post_v0.2_redeem_chimoney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/redeem/airtime\n  method: post\n  operationId: post_v0.2_redeem_airtime\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/redeem/gift-card\n  method: post\n  operationId: post_v0.2_redeem_gift-card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/redeem/mobile-money\n  method: post\n  operationId: post_v0.2_redeem_mobile-money\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v0.2/info/assets\n  method: get\n  operationId: get_v0.2_info_assets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/info/country-banks\n  method: get\n  operationId: get_v0.2_info_country-banks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/info/bank-branches\n  method: get\n  operationId: get_v0.2_info_bank-branches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/info/airtime-countries\n  method: get\n  operationId: get_v0.2_info_airtime-countries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/info/mobile-money-codes\n\
  \  method: get\n  operationId: get_v0.2_info_mobile-money-codes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/info/exchange-rates\n  method: get\n  operationId: get_v0.2_info_exchange-rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/info/local-amount-in-usd\n  method: get\n  operationId: get_v0.2_info_local-amount-in-usd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/info/usd-amount-in-local\n  method: get\n  operationId: get_v0.2_info_usd-amount-in-local\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.2/info/verify-bank-account-number\n\
  \  method: post\n  operationId: post_v0.2_info_verify-bank-account-number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/accounts/transactions\n  method: post\n  operationId: post_v0.2_accounts_transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/accounts/transaction\n  method: post\n  operationId: post_v0.2_accounts_transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/accounts/issue-id-transactions\n  method: post\n  operationId: post_v0.2_accounts_issue-id-transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/accounts/public-profile\n  method: post\n  operationId: post_v0.2_accounts_public-profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/accounts/transfer\n  method: post\n  operationId: post_v0.2_accounts_transfer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/accounts/delete-unpaid-transaction\n  method: delete\n  operationId: delete_v0.2_accounts_delete-unpaid-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/accounts/issue-wallet-address\n  method: post\n  operationId: post_v0.2_accounts_issue-wallet-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payment/initiate\n  method: post\n  operationId: post_v0.2_payment_initiate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payment/verify\n  method: post\n  operationId: post_v0.2_payment_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/payment/simulate\n  method: post\n  operationId: post_v0.2_payment_simulate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chimoney/refs/heads/main/agentic-access/chimoney-agentic-access.yml
summary_line: 52 operations · 39 acting
tags:
- Payouts
- Disbursements
- Payments
- Africa
- Global Payouts
- Wallets
- Multicurrency
- Gift Cards
- Mobile Money
- Fintech
---
