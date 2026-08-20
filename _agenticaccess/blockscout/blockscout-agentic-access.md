---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 56
api_specs:
- filename: blockscout-addresses-api-openapi.yml
  format: yaml
  label: Blockscout Addresses API
  slug: blockscout-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-addresses-api-openapi.yml
- filename: blockscout-blocks-api-openapi.yml
  format: yaml
  label: Blockscout Blocks API
  slug: blockscout-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-blocks-api-openapi.yml
- filename: blockscout-celestiaservice-api-openapi.yml
  format: yaml
  label: Blockscout CelestiaService API
  slug: blockscout-celestiaservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-celestiaservice-api-openapi.yml
- filename: blockscout-config-api-openapi.yml
  format: yaml
  label: Blockscout Config API
  slug: blockscout-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-config-api-openapi.yml
- filename: blockscout-internal-transactions-api-openapi.yml
  format: yaml
  label: Blockscout Internal Transactions API
  slug: blockscout-internal-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-internal-transactions-api-openapi.yml
- filename: blockscout-main-page-api-openapi.yml
  format: yaml
  label: Blockscout Main Page API
  slug: blockscout-main-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-main-page-api-openapi.yml
- filename: blockscout-proxy-api-openapi.yml
  format: yaml
  label: Blockscout Proxy API
  slug: blockscout-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-proxy-api-openapi.yml
- filename: blockscout-search-api-openapi.yml
  format: yaml
  label: Blockscout Search API
  slug: blockscout-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-search-api-openapi.yml
- filename: blockscout-smart-contracts-api-openapi.yml
  format: yaml
  label: Blockscout Smart Contracts API
  slug: blockscout-smart-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-smart-contracts-api-openapi.yml
- filename: blockscout-stats-api-openapi.yml
  format: yaml
  label: Blockscout Stats API
  slug: blockscout-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-stats-api-openapi.yml
- filename: blockscout-token-transfers-api-openapi.yml
  format: yaml
  label: Blockscout Token Transfers API
  slug: blockscout-token-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-token-transfers-api-openapi.yml
- filename: blockscout-tokens-api-openapi.yml
  format: yaml
  label: Blockscout Tokens API
  slug: blockscout-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-tokens-api-openapi.yml
- filename: blockscout-transactions-api-openapi.yml
  format: yaml
  label: Blockscout Transactions API
  slug: blockscout-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-transactions-api-openapi.yml
- filename: blockscout-withdrawals-api-openapi.yml
  format: yaml
  label: Blockscout Withdrawals API
  slug: blockscout-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/openapi/blockscout-withdrawals-api-openapi.yml
consequence_counts:
  read: 56
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blockscout Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 57
overview: 'Blockscout exposes 57 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 56 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blockscout
provider_slug: blockscout
slug: blockscout-agentic-access
source_filename: blockscout-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/blockscout-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 56\n    acting: 1\n  by_consequence:\n    read: 56\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/check-redirect\n  method: get\n  operationId: search redirect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId:\
  \ get_txs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks\n  method: get\n  operationId: get_blocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token-transfers\n  method: get\n  operationId: get_token_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal-transactions\n  method: get\n  operationId: get_internal_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main-page/transactions\n  method: get\n  operationId: get_main_page_txs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /main-page/blocks\n  method: get\n  operationId: get_main_page_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /main-page/indexing-status\n  method: get\n  operationId: get_indexing_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: get_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/charts/transactions\n  method: get\n  operationId: get_txs_chart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/charts/market\n  method: get\n  operationId: get_market_chart\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_hash}\n  method: get\n  operationId: get_tx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_hash}/token-transfers\n  method: get\n  operationId: get_transaction_token_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_hash}/internal-transactions\n  method: get\n  operationId: get_transaction_internal_txs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_hash}/logs\n  method: get\n  operationId: get_transaction_logs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_hash}/raw-trace\n  method: get\n  operationId: get_transaction_raw_trace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_hash}/state-changes\n  method: get\n  operationId: get_transaction_state_changes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_hash}/summary\n  method: get\n  operationId: get_transaction_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks/{block_number_or_hash}\n  method: get\n  operationId: get_block\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks/{block_number_or_hash}/transactions\n  method: get\n  operationId: get_block_txs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks/{block_number_or_hash}/withdrawals\n  method: get\n  operationId: get_block_withdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses\n  method: get\n  operationId: get_addresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}\n  method: get\n  operationId: get_address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/counters\n  method: get\n  operationId: get_address_counters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/transactions\n  method: get\n  operationId: get_address_txs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/token-transfers\n  method: get\n  operationId: get_address_token_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/internal-transactions\n  method: get\n  operationId: get_address_internal_txs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/logs\n  method: get\n  operationId: get_address_logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/blocks-validated\n  method: get\n  operationId: get_address_blocks_validated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/token-balances\n  method: get\n  operationId: get_address_token_balances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/tokens\n  method: get\n  operationId: get_address_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/coin-balance-history\n  method: get\n  operationId: get_address_coin_balance_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/coin-balance-history-by-day\n  method: get\n  operationId: get_address_coin_balance_history_by_day\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/withdrawals\n  method: get\n  operationId: get_address_withdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/nft\n  method: get\n  operationId: get_address_nft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_hash}/nft/collections\n  method: get\n  operationId: get_address_nft_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens\n  method: get\n  operationId: get_tokens_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{address_hash}\n  method: get\n  operationId: get_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{address_hash}/transfers\n  method: get\n  operationId: get_token_token_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /tokens/{address_hash}/holders\n  method: get\n  operationId: get_token_holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{address_hash}/counters\n  method: get\n  operationId: get_token_counters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{address_hash}/instances\n  method: get\n  operationId: get_nft_instances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{address_hash}/instances/{id}\n  method: get\n  operationId: get_nft_instance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{address_hash}/instances/{id}/transfers\n\
  \  method: get\n  operationId: get_nft_instance_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{address_hash}/instances/{id}/holders\n  method: get\n  operationId: get_token_instance_holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{address_hash}/instances/{id}/transfers-count\n  method: get\n  operationId: get_nft_instance_transfers_count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{address_hash}/instances/{id}/refetch-metadata\n  method: patch\n  operationId: refetch_token_instance_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smart-contracts\n  method: get\n  operationId: get_smart_contracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smart-contracts/counters\n  method: get\n  operationId: get_smart_contracts_counters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smart-contracts/{address_hash}\n  method: get\n  operationId: get_smart_contract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/json-rpc-url\n  method: get\n  operationId: get_json_rpc_url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals\n  method: get\n  operationId: get_withdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proxy/account-abstraction/status\n  method: get\n  operationId: get_account_abstraction_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/celestia/blob\n  method: get\n  operationId: CelestiaService_GetBlob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/celestia/l2BatchMetadata\n  method: get\n  operationId: CelestiaService_GetL2BatchMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /health\n  method: get\n  operationId: Health_Check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/agentic-access/blockscout-agentic-access.yml
summary_line: 57 operations · 1 acting
tags:
- Web3
- Explorer
- Open-Source
- EVM
- Multi-Chain
- GraphQL
- REST
- Etherscan-Compatible
---
