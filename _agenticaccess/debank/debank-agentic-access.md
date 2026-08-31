---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 38
api_specs:
- filename: debank-account-api-openapi.yml
  format: yaml
  label: DeBank Account API
  slug: debank-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-account-api-openapi.yml
- filename: debank-app-protocol-api-openapi.yml
  format: yaml
  label: DeBank App Protocol API
  slug: debank-app-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-app-protocol-api-openapi.yml
- filename: debank-chain-api-openapi.yml
  format: yaml
  label: DeBank Chain API
  slug: debank-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-chain-api-openapi.yml
- filename: debank-cloud-api-openapi.yml
  format: yaml
  label: DeBank Cloud API
  slug: debank-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-cloud-api-openapi.yml
- filename: debank-official-api-openapi.yml
  format: yaml
  label: DeBank Official API
  slug: debank-official-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-official-api-openapi.yml
- filename: debank-pool-api-openapi.yml
  format: yaml
  label: DeBank Pool API
  slug: debank-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-pool-api-openapi.yml
- filename: debank-protocol-api-openapi.yml
  format: yaml
  label: DeBank Protocol API
  slug: debank-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-protocol-api-openapi.yml
- filename: debank-token-api-openapi.yml
  format: yaml
  label: DeBank Token API
  slug: debank-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-token-api-openapi.yml
- filename: debank-user-api-openapi.yml
  format: yaml
  label: DeBank User API
  slug: debank-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-user-api-openapi.yml
- filename: debank-wallet-api-openapi.yml
  format: yaml
  label: DeBank Wallet API
  slug: debank-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-wallet-api-openapi.yml
consequence_counts:
  physical: 2
  read: 38
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Debank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/official/group_send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/official/message/send
operation_count: 42
overview: 'DeBank exposes 42 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DeBank
provider_slug: debank
slug: debank-agentic-access
source_filename: debank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/debank-pro-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 38\n    acting: 4\n  by_consequence:\n    read: 38\n    physical: 2\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /cloud/chain/list\n  method: get\n  operationId: get_chain_list_view\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud/collection\n  method: get\n  operationId: get_get_collection_view\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /cloud/contract\n  method: get\n  operationId: get_get_contract_view\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud/protocol/list\n  method: get\n  operationId: get_protocol_list_view\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud/token\n  method: get\n  operationId: get_get_token_view\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/units\n  method: get\n  operationId: get_unit_api_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app_protocol/list\n  method: get\n  operationId: get_app_protocol_list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain\n  method: get\n  operationId: get_chain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chain/list\n  method: get\n  operationId: get_chain_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official/group_send\n  method: post\n  operationId: post_group_send_api_view\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/official/message/send\n\
  \  method: post\n  operationId: post_message_send_api_view\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pool\n  method: get\n  operationId: get_pool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/protocol\n  method: get\n  operationId: get_protocol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/protocol/all_list\n  method: get\n  operationId: get_protocol_all_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/protocol/list\n  method: get\n  operationId: get_protocol_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/token\n  method: get\n  operationId: get_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/token/history_price\n  method: get\n  operationId: get_token_history_price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/token/list_by_ids\n  method: get\n  operationId: get_token_list_by_ids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/token/top_holders\n  method: get\n  operationId: get_token_top_holders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/all_complex_protocol_list\n  method: get\n  operationId: get_user_all_complex_protocol_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/all_history_list\n  method: get\n  operationId: get_user_history_all_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/all_nft_list\n  method: get\n  operationId: get_user_nft_all_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/all_simple_protocol_list\n  method: get\n  operationId: get_user_all_simple_protocol_list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/all_token_list\n  method: get\n  operationId: get_user_token_all_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/chain_balance\n  method: get\n  operationId: get_user_chain_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/chain_net_curve\n  method: get\n  operationId: get_user_chain_net_curve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/complex_app_list\n  method: get\n  operationId: get_user_complex_app_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/complex_protocol_list\n  method: get\n  operationId: get_user_complex_protocol_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/history_list\n  method: get\n  operationId: get_user_history_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/nft_authorized_list\n  method: get\n  operationId: get_user_nft_authorized_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/nft_list\n  method: get\n  operationId: get_user_nft_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/user/protocol\n  method: get\n  operationId: get_user_protocol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/simple_protocol_list\n  method: get\n  operationId: get_user_simple_protocol_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/token\n  method: get\n  operationId: get_user_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/token_authorized_list\n  method: get\n  operationId: get_user_token_authorized_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/token_list\n  method: get\n  operationId: get_user_token_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/total_balance\n  method: get\n  operationId: get_user_total_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/total_net_curve\n  method: get\n  operationId: get_total_chain_net_curve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/used_chain_list\n  method: get\n  operationId: get_user_chain_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallet/explain_tx\n  method: post\n  operationId: post_explain_tx\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/wallet/gas_market\n  method: get\n  operationId: get_gas_market\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallet/pre_exec_tx\n  method: post\n  operationId: post_pre_exec_tx\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/agentic-access/debank-agentic-access.yml
summary_line: 42 operations · 4 acting
tags:
- Web3
- DeFi
- Blockchain
- Crypto
- Portfolio Tracking
- On-Chain Data
- Wallets
- token-data
- NFT
- Ethereum
- Authentication
- Market Data
---
