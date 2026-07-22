---
acting_count: 109
action_class_counts:
  acting: 109
  connected: 92
api_specs:
- filename: ripple-labs-rlusd-openapi-original.yml
  format: yaml
  label: Ripple Mint API (RLUSD Stablecoin)
  slug: ripple-mint-api-rlusd-stablecoin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-rlusd-openapi-original.yml
- filename: ripple-labs-ripplenet-openapi-original.yml
  format: yaml
  label: RippleNet Server API
  slug: ripplenet-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-ripplenet-openapi-original.yml
- filename: ripple-labs-report-service-openapi-original.yml
  format: yaml
  label: Report Service API
  slug: report-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-report-service-openapi-original.yml
- filename: ripple-labs-smart-liquidation-openapi-original.yml
  format: yaml
  label: Smart Liquidation API
  slug: smart-liquidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-smart-liquidation-openapi-original.yml
- filename: ripple-labs-palisade-wallet-openapi-original.yml
  format: yaml
  label: Palisade Wallet-as-a-Service API
  slug: palisade-wallet-as-a-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-palisade-wallet-openapi-original.yml
consequence_counts:
  physical: 42
  read: 92
  write: 67
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ripple Labs Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /config/payments/payment_expiries
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /config/payments/payment_expiries/{payment_expiry_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /config/payments/payment_expiries/{payment_expiry_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /config/payments/quote_expiries
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /config/payments/quote_expiries/{quote_expiry_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /config/payout_methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /config/payout_methods/{payout_method_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /config/payout_methods/{payout_method_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange_transfers/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange_transfers/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange_transfers/{id}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{payment_id}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{payment_id}/fail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{payment_id}/finalize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payments/{payment_id}/labels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payments/{payment_id}/labels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{payment_id}/lock
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{payment_id}/reject
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{payment_id}/retry_accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{payment_id}/settle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{payment_id}/sub_state
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /quote_collections/return
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /quote_collections/reversal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request_for_payment
operation_count: 201
overview: 'Ripple Labs exposes 201 API operations that an AI agent could call, of which 109 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 92 read, 67 write, and 42 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ripple Labs
provider_slug: ripple-labs
slug: ripple-labs-agentic-access
source_filename: ripple-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/ripple-labs-palisade-wallet-openapi-original.yml, openapi/ripple-labs-report-service-openapi-original.yml,\n  openapi/ripple-labs-ripplenet-openapi-original.yml, openapi/ripple-labs-rlusd-openapi-original.yml,\n  openapi/ripple-labs-smart-liquidation-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 201\n  by_action_class:\n    connected: 92\n    acting: 109\n  by_consequence:\n    read: 92\n    write: 67\n    physical: 42\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/addresses\n  method: get\n  operationId: CounterpartyService_ListGlobalAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/addresses:list\n  method: post\n  operationId: CounterpartyService_ListGlobalAddresses2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/balances\n  method: get\n  operationId: BalanceService_GetOrgBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/counterparties\n  method: get\n  operationId: CounterpartyService_ListCounterparties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/counterparties\n  method: post\n  operationId: CounterpartyService_CreateCounterparty\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/counterparties/{counterpartyId}/addresses\n  method: get\n  operationId: CounterpartyService_ListAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/counterparties/{counterpartyId}/addresses\n  method: post\n  operationId: CounterpartyService_CreateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/counterparties/{counterpartyId}/addresses/{addressId}\n  method: get\n\
  \  operationId: CounterpartyService_GetAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/counterparties/{counterpartyId}/addresses/{addressId}\n  method: delete\n  operationId: CounterpartyService_DeleteAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/counterparties/{counterpartyId}/addresses:list\n  method: post\n  operationId: CounterpartyService_ListAddresses2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v2/counterparties/{id}\n  method: get\n  operationId: CounterpartyService_GetCounterparty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/counterparties/{id}\n  method: delete\n  operationId: CounterpartyService_DeleteCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/counterparties/{id}\n  method: put\n  operationId: CounterpartyService_UpdateCounterparty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/counterparties:list\n  method: post\n  operationId: CounterpartyService_ListCounterparties2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/credentials/oauth/token\n  method: post\n  operationId: CredentialService_ExchangeCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/policy-rules/limits\n  method: get\n  operationId: PolicyService_ListGlobalWalletLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v2/policy-rules/limits:list\n  method: post\n  operationId: PolicyService_ListGlobalWalletLimits2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tags\n  method: get\n  operationId: VaultService_ListGlobalTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transactions\n  method: get\n  operationId: TransactionsService_ListTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transactions/sweep/{sweepId}\n  method: get\n  operationId: TransactionsService_ListSweepInstanceTransactions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transactions/sweep/{sweepId}:list\n  method: post\n  operationId: TransactionsService_ListSweepInstanceTransactions2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transactions/transfer/estimate-fee\n  method: post\n  operationId: TransactionsService_EstimateTransferFee\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/transactions:list\n  method: post\n  operationId: TransactionsService_ListTransactions2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults\n  method: get\n  operationId: VaultService_ListVaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults\n  method: post\n  operationId: VaultService_CreateVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/tags\n  method: get\n  operationId:\
  \ VaultService_ListGlobalVaultTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{id}\n  method: get\n  operationId: VaultService_GetVault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{id}\n  method: put\n  operationId: VaultService_UpdateVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/balances\n  method: get\n  operationId: BalanceService_GetVaultBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/vaults/{vaultId}/tags\n  method: get\n  operationId: VaultService_ListVaultTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/tags\n  method: delete\n  operationId: VaultService_DeleteVaultTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/tags\n  method: post\n  operationId: VaultService_AddVaultTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets\n\
  \  method: get\n  operationId: VaultService_ListVaultWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets\n  method: post\n  operationId: VaultService_CreateWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/tags\n  method: get\n  operationId: VaultService_ListWalletTagsInVault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets/{walletId}\n  method: get\n  operationId: VaultService_GetWallet\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets/{walletId}\n  method: delete\n  operationId: VaultService_DeleteWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}\n  method: put\n  operationId: VaultService_UpdateWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/balances\n  method: get\n  operationId: BalanceService_GetWalletBalances\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/balances/sync\n  method: post\n  operationId: BalanceService_SyncWalletBalances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/limits\n  method: get\n  operationId: PolicyService_ListWalletLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/limits\n  method: put\n  operationId: PolicyService_CreateWalletLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/limits/{id}\n  method: get\n  operationId: PolicyService_GetWalletLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/limits/{id}\n  method: delete\n  operationId: PolicyService_DeleteWalletLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/policy-rules/limits:list\n  method: post\n  operationId: PolicyService_ListWalletLimits2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/sequence\n  method: get\n  operationId: VaultService_GetWalletSequence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/settings\n  method: put\n  operationId: VaultService_UpdateWalletSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/tags\n \
  \ method: get\n  operationId: VaultService_ListWalletTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/tags\n  method: delete\n  operationId: VaultService_DeleteWalletTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/tags\n  method: post\n  operationId: VaultService_AddWalletTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions\n\
  \  method: get\n  operationId: TransactionsService_ListWalletTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/raw\n  method: post\n  operationId: TransactionsService_RawTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/sign-plaintext\n  method: post\n  operationId: TransactionsService_SignPlaintext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/transfer\n  method: post\n  operationId: TransactionsService_TransferTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/account-set\n  method: post\n  operationId: TransactionsService_SubmitAccountSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/amm-create\n\
  \  method: post\n  operationId: TransactionsService_SubmitAMMCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/amm-deposit\n  method: post\n  operationId: TransactionsService_SubmitAMMDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/amm-withdraw\n  method: post\n  operationId: TransactionsService_SubmitAMMWithdraw\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/clawback\n  method: post\n  operationId: TransactionsService_SubmitClawback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/offer-cancel\n  method: post\n  operationId: TransactionsService_SubmitOfferCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/offer-create\n  method: post\n  operationId: TransactionsService_SubmitOfferCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/signer-list-set\n  method: post\n  operationId: TransactionsService_SubmitSignerListSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v2/vaults/{vaultId}/wallets/{walletId}/transactions/xrp/trust-set\n  method: post\n  operationId: TransactionsService_SubmitTrustSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/{transactionId}\n  method: get\n  operationId: TransactionsService_GetTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/{transactionId}/freeze\n  method: put\n  operationId: TransactionsService_FreezeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions/{transactionId}/unfreeze\n  method: put\n  operationId: TransactionsService_UnfreezeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets/{walletId}/transactions:list\n  method: post\n  operationId: TransactionsService_ListWalletTransactions2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults/{vaultId}/wallets:list\n\
  \  method: post\n  operationId: VaultService_ListVaultWallets2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vaults:list\n  method: post\n  operationId: VaultService_ListVaults2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/wallets\n  method: get\n  operationId: VaultService_ListGlobalWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wallets/{id}\n  method: get\n  operationId: VaultService_GetWalletByID\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wallets:list\n  method: post\n  operationId: VaultService_ListGlobalWallets2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks\n  method: get\n  operationId: WebhookService_ListWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks\n  method: post\n  operationId: WebhookService_CreateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{id}\n  method: get\n  operationId: WebhookService_GetWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{id}\n  method: delete\n  operationId: WebhookService_DeleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{webhookId}/subscriptions\n  method: get\n  operationId: WebhookService_ListSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{webhookId}/subscriptions\n  method:\
  \ post\n  operationId: WebhookService_CreateSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{webhookId}/subscriptions/{subscriptionId}\n  method: get\n  operationId: WebhookService_GetSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{webhookId}/subscriptions/{subscriptionId}\n  method: delete\n  operationId: WebhookService_DeleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /v2/webhooks/{webhookId}/subscriptions:list\n  method: post\n  operationId: WebhookService_ListSubscriptions2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks:list\n  method: post\n  operationId: WebhookService_ListWebhooks2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/workflows/sweep/{id}/trigger\n  method: post\n  operationId: SweepService_TriggerSweepConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reports\n  method: get\n  operationId: getReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports\n  method: post\n  operationId: postReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reports/{report-id}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/{report-id}\n  method: delete\n  operationId:\
  \ deleteReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reports/download/{report-id}\n  method: get\n  operationId: getReportDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit\n  method: get\n  operationId: getAudits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit/payment/{id}\n  method: get\n  operationId: getEventTrailForPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_lookups\n  method: get\n\
  \  operationId: getAccountLookupByStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_lookups/request\n  method: post\n  operationId: initiateAccountLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_lookups/response\n  method: post\n  operationId: completeAccountLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_lookups/{account_lookup_id}\n  method: get\n  operationId: getAccountLookupById\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/fees\n  method: get\n  operationId: getFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/fees\n  method: post\n  operationId: createFee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config/fees/{id}\n  method: get\n  operationId: getFeeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/fees/{id}\n  method: put\n  operationId: updateFee\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config/fees/{id}\n  method: delete\n  operationId: deleteFee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config/payments/payment_expiries/{payment_expiry_id}\n  method: get\n  operationId: getPaymentExpiryById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/payment\n\n# --- truncated at 32 KB (62 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/agentic-access/ripple-labs-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/agentic-access/ripple-labs-agentic-access.yml
summary_line: 201 operations · 109 acting
tags:
- Company
- Financial Services
- Payments
- Cross-Border Payments
- Blockchain
- Cryptocurrency
- Stablecoin
- Digital Assets
- Custody
- Wallet
- Fintech
---
