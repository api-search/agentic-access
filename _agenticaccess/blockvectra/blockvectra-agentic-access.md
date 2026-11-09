---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 42
api_specs:
- filename: blockvectra-account-api-openapi.yml
  format: yaml
  label: BlockVectra Account API
  slug: blockvectra-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-account-api-openapi.yml
- filename: blockvectra-addresses-api-openapi.yml
  format: yaml
  label: BlockVectra Addresses API
  slug: blockvectra-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-addresses-api-openapi.yml
- filename: blockvectra-auth-api-openapi.yml
  format: yaml
  label: BlockVectra Auth API
  slug: blockvectra-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-auth-api-openapi.yml
- filename: blockvectra-billing-api-openapi.yml
  format: yaml
  label: BlockVectra Billing API
  slug: blockvectra-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-billing-api-openapi.yml
- filename: blockvectra-chain-api-openapi.yml
  format: yaml
  label: BlockVectra Chain API
  slug: blockvectra-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-chain-api-openapi.yml
- filename: blockvectra-chains-api-openapi.yml
  format: yaml
  label: BlockVectra Chains API
  slug: blockvectra-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-chains-api-openapi.yml
- filename: blockvectra-dex-api-openapi.yml
  format: yaml
  label: BlockVectra DEX API
  slug: blockvectra-dex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-dex-api-openapi.yml
- filename: blockvectra-faucet-api-openapi.yml
  format: yaml
  label: BlockVectra Faucet API
  slug: blockvectra-faucet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-faucet-api-openapi.yml
- filename: blockvectra-json-rpc-api-openapi.yml
  format: yaml
  label: BlockVectra JSON RPC API
  slug: blockvectra-json-rpc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-json-rpc-api-openapi.yml
- filename: blockvectra-keys-api-openapi.yml
  format: yaml
  label: BlockVectra Keys API
  slug: blockvectra-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-keys-api-openapi.yml
- filename: blockvectra-me-api-openapi.yml
  format: yaml
  label: BlockVectra Me API
  slug: blockvectra-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-me-api-openapi.yml
- filename: blockvectra-nfts-api-openapi.yml
  format: yaml
  label: BlockVectra NFTs API
  slug: blockvectra-nfts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-nfts-api-openapi.yml
- filename: blockvectra-status-api-openapi.yml
  format: yaml
  label: BlockVectra Status API
  slug: blockvectra-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-status-api-openapi.yml
- filename: blockvectra-stocks-api-openapi.yml
  format: yaml
  label: BlockVectra Stocks API
  slug: blockvectra-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-stocks-api-openapi.yml
- filename: blockvectra-subscriptions-api-openapi.yml
  format: yaml
  label: BlockVectra Subscriptions API
  slug: blockvectra-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-subscriptions-api-openapi.yml
- filename: blockvectra-tokens-api-openapi.yml
  format: yaml
  label: BlockVectra Tokens API
  slug: blockvectra-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-tokens-api-openapi.yml
- filename: blockvectra-traces-api-openapi.yml
  format: yaml
  label: BlockVectra Traces API
  slug: blockvectra-traces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-traces-api-openapi.yml
- filename: blockvectra-top-up-api-openapi.yml
  format: yaml
  label: BlockVectra Top Up API
  slug: blockvectra-top-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockvectra/openapi/blockvectra-top-up-api-openapi.yml
consequence_counts:
  read: 42
  safety-critical: 3
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Blockvectra Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /keys/{key_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /push/subscriptions/{subscription_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resets/use
operation_count: 66
overview: 'BlockVectra exposes 66 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 42 read, 21 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BlockVectra
provider_slug: blockvectra
slug: blockvectra-agentic-access
source_filename: blockvectra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/console.yaml, openapi/data.yaml, openapi/json-rpc.yaml, openapi/push.yaml, openapi/topup.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 66\n  by_action_class:\n    connected: 42\n    acting: 24\n  by_consequence:\n    read: 42\n    write: 21\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /auth/siwe/challenge\n  method: post\n  operationId: siweChallenge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/siwe/login\n  method: post\n  operationId: siweLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: patch\n  operationId: updateUsername\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /me/identities/siwe\n  method: post\n  operationId: linkSiwe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/identities/oauth\n  method: post\n  operationId: linkOauth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/identities/{identity_id}\n  method: delete\n  operationId: unlinkIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/{key_id}\n  method: get\n  operationId: getKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /keys/{key_id}\n  method: patch\n  operationId: renameKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/{key_id}/rotate\n  method: post\n  operationId: rotateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/{key_id}/revoke\n  method: post\n  operationId: revokeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /plans\n  method: get\n  operationId: getPlans\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charges\n  method: get\n  operationId: listCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topups\n  method: get\n  operationId: listTopups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resets\n  method: get\n  operationId: getResets\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resets/use\n  method: post\n  operationId: useReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chains\n  method: get\n  operationId: getChains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/status/freshness\n  method: get\n  operationId: getStatusFreshness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/blocks/{number}\n  method:\
  \ get\n  operationId: getBlockByNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/blocks/hash/{hash}\n  method: get\n  operationId: getBlockByHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/blocks/{number}/transactions\n  method: get\n  operationId: getBlockTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/transactions/{hash}\n  method: get\n  operationId: getTransactionByHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/addresses/{address}/transactions\n  method: get\n  operationId: getAddressTransactions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/addresses/{address}/transfers\n  method: get\n  operationId: getAddressTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/tokens/{token}/transfers\n  method: get\n  operationId: getTokenTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/addresses/{address}/balances\n  method: get\n  operationId: getAddressBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/tokens/{token}/holders\n  method: get\n  operationId: getTokenHolders\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/tokens/{token}\n  method: get\n  operationId: getTokenMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/tokens:batch\n  method: post\n  operationId: postTokensBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{chain}/nfts/{contract}/{token_id}\n  method: get\n  operationId: getNftByContractAndTokenId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/nfts\n  method: get\n  operationId: getNftsByOwner\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/dex/swaps\n  method: get\n  operationId: getDexSwaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/dex/prices\n  method: get\n  operationId: getDexPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/stocks\n  method: get\n  operationId: getStocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/stocks/{token}\n  method: get\n  operationId: getStockByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /{chain}/blocks/{number}/traces\n  method: get\n  operationId: getBlockTraces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/transactions/{hash}/trace\n  method: get\n  operationId: getTransactionTrace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faucet/robinhood_testnet\n  method: post\n  operationId: claimRobinhoodTestnetFaucet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /faucet/robinhood_testnet\n  method: options\n  operationId: preflightRobinhoodTestnetFaucet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chain}/public\n  method: post\n  operationId: rpcPublic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{chain}/public/{apiKey}\n  method: post\n  operationId: rpcPublicWithPathKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{chain}/{apiKey}\n  method: post\n  operationId: rpcWithPathKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{chain}\n  method: post\n  operationId: rpcWithHeaderKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chains\n  method: get\n  operationId: getChains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/chains\n  method: get\n  operationId: listPushChains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/subscriptions/{subscription_id}\n  method: get\n  operationId: getSubscription\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/subscriptions/{subscription_id}\n  method: patch\n  operationId: patchSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/subscriptions/{subscription_id}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /push/subscriptions/{subscription_id}/addresses\n  method:\
  \ get\n  operationId: listSubscriptionAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/subscriptions/{subscription_id}/addresses/add\n  method: post\n  operationId: addSubscriptionAddresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/subscriptions/{subscription_id}/addresses/remove\n  method: post\n  operationId: removeSubscriptionAddresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/subscriptions/{subscription_id}/replay\n\
  \  method: post\n  operationId: replaySubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/subscriptions/{subscription_id}/rotate-secret\n  method: post\n  operationId: rotateSubscriptionSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/subscriptions/{subscription_id}/events\n  method: get\n  operationId: listDeliveredSubscriptionEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topup/status\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topup/deposit-address\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topup/deposits\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/blockvectra/agentic-access/blockvectra-agentic-access.yml
summary_line: 66 operations · 24 acting · 3 human-in-the-loop
tags:
- Blockchain
- Data API
- Multi-Chain
- Cryptocurrency
- Developer Platform
---
