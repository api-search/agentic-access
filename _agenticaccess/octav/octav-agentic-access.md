---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 24
api_specs:
- filename: octav-airdrops-api-openapi.yml
  format: yaml
  label: Octav Airdrops API
  slug: octav-airdrops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-airdrops-api-openapi.yml
- filename: octav-approvals-api-openapi.yml
  format: yaml
  label: Octav Approvals API
  slug: octav-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-approvals-api-openapi.yml
- filename: octav-beacon-validators-api-openapi.yml
  format: yaml
  label: Octav Beacon Validators API
  slug: octav-beacon-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-beacon-validators-api-openapi.yml
- filename: octav-chains-api-openapi.yml
  format: yaml
  label: Octav Chains API
  slug: octav-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-chains-api-openapi.yml
- filename: octav-contract-protocol-api-openapi.yml
  format: yaml
  label: Octav Contract Protocol API
  slug: octav-contract-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-contract-protocol-api-openapi.yml
- filename: octav-credits-api-openapi.yml
  format: yaml
  label: Octav Credits API
  slug: octav-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-credits-api-openapi.yml
- filename: octav-nav-api-openapi.yml
  format: yaml
  label: Octav Nav API
  slug: octav-nav-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-nav-api-openapi.yml
- filename: octav-portfolio-api-openapi.yml
  format: yaml
  label: Octav Portfolio API
  slug: octav-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-portfolio-api-openapi.yml
- filename: octav-status-api-openapi.yml
  format: yaml
  label: Octav Status API
  slug: octav-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-status-api-openapi.yml
- filename: octav-sync-api-openapi.yml
  format: yaml
  label: Octav Sync API
  slug: octav-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-sync-api-openapi.yml
- filename: octav-tokens-api-openapi.yml
  format: yaml
  label: Octav Tokens API
  slug: octav-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-tokens-api-openapi.yml
- filename: octav-transactions-api-openapi.yml
  format: yaml
  label: Octav Transactions API
  slug: octav-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-transactions-api-openapi.yml
- filename: octav-virtual-users-api-openapi.yml
  format: yaml
  label: Octav Virtual Users API
  slug: octav-virtual-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-virtual-users-api-openapi.yml
- filename: octav-wallet-api-openapi.yml
  format: yaml
  label: Octav Wallet API
  slug: octav-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-wallet-api-openapi.yml
consequence_counts:
  read: 24
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Octav Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Octav exposes 25 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Octav
provider_slug: octav
slug: octav-agentic-access
source_filename: octav-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/octav-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 24\n    acting: 1\n  by_consequence:\n    read: 24\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /portfolio\n  method: get\n  operationId: getPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/at-block\n  method: get\n  operationId: getPortfolioAtBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /virtual-users\n  method:\
  \ get\n  operationId: listVirtualUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /virtual-users/portfolio\n  method: get\n  operationId: getVirtualUsersPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nav\n  method: get\n  operationId: getNav\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet\n  method: get\n  operationId: getWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /approvals/{chain}\n  method: get\n  operationId: getApprovals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token-overview\n  method: get\n  operationId: getTokenOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airdrop\n  method: get\n  operationId: getAirdrop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical\n  method: get\n  operationId: getHistoricalPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sync-transactions\n  method: post\n  operationId: syncWallet\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chains\n  method: get\n  operationId: getChains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chains/{chainKey}/protocols\n  method: get\n  operationId: getProtocols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contract-protocol\n  method: get\n  operationId: getContractProtocol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beacon/validators/details/index/{index}\n  method: get\n  operationId: getValidatorDetailsByIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beacon/validators/details/pubkey/{pubkey}\n  method: get\n  operationId: getValidatorDetailsByPubkey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beacon/validators/rewards/index/{index}\n  method: get\n  operationId: getValidatorRewardsByIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beacon/validators/rewards/pubkey/{pubkey}\n  method: get\n  operationId: getValidatorRewardsByPubkey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beacon/validators/withdrawals/index/{index}\n  method: get\n  operationId: getValidatorWithdrawalsByIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beacon/validators/withdrawals/pubkey/{pubkey}\n  method: get\n  operationId: getValidatorWithdrawalsByPubkey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beacon/validators/deposits/index/{index}\n  method: get\n  operationId: getValidatorDepositsByIndex\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beacon/validators/deposits/pubkey/{pubkey}\n  method: get\n  operationId: getValidatorDepositsByPubkey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/agentic-access/octav-agentic-access.yml
summary_line: 25 operations · 1 acting
tags:
- Company
- Cryptocurrency
- Blockchain
- Portfolio
- DeFi
- Analytics
- Web3
- Financial Data
- Wallets
---
