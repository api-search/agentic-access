---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 12
api_specs:
- filename: developer-controlled-wallets.yaml
  format: yaml
  label: Developer-Controlled Wallets
  slug: developer-controlled-wallets
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/developer-controlled-wallets.yaml
- filename: user-controlled-wallets.yaml
  format: yaml
  label: User-Controlled Wallets
  slug: user-controlled-wallets
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/user-controlled-wallets.yaml
- filename: cctp.yaml
  format: yaml
  label: Cross-Chain Transfer Protocol (CCTP)
  slug: cctp
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/cctp.yaml
- filename: gateway.yaml
  format: yaml
  label: Circle Gateway
  slug: gateway
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/gateway.yaml
- filename: smart-contract-platform.yaml
  format: yaml
  label: Smart Contract Platform
  slug: smart-contract-platform
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/smart-contract-platform.yaml
- filename: cpn-ofi.yaml
  format: yaml
  label: Circle Payments Network (CPN)
  slug: cpn
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/cpn-ofi.yaml
- filename: compliance.yaml
  format: yaml
  label: Compliance Engine
  slug: compliance-engine
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/compliance.yaml
- filename: stablefx.yaml
  format: yaml
  label: StableFX
  slug: stablefx
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/stablefx.yaml
- filename: xreserve.yaml
  format: yaml
  label: xReserve
  slug: xreserve
  spec_type: OpenAPI
  url: https://developers.circle.com/openapi/xreserve.yaml
consequence_counts:
  physical: 2
  read: 12
  safety-critical: 3
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Circle Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/w3s/developer/walletSets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/w3s/developer/walletSets/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/w3s/developer/wallets
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/w3s/developer/transactions/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/w3s/transactions/transfer/estimateFee
operation_count: 30
overview: 'Circle exposes 30 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 13 write, 2 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Circle
provider_slug: circle
slug: circle-agentic-access
source_filename: circle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/circle-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 12\n    acting: 18\n  by_consequence:\n    read: 12\n    safety-critical: 3\n    write: 13\n    physical: 2\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/w3s/walletSets\n  method: get\n  operationId: listWalletSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/walletSets/{id}\n  method: get\n  operationId: getWalletSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v1/w3s/developer/walletSets\n  method: post\n  operationId: createWalletSet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/w3s/developer/walletSets/{id}\n  method: put\n  operationId: updateWalletSet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/w3s/developer/wallets\n  method: post\n  operationId: createWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/w3s/wallets\n  method: get\n  operationId: listWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/wallets/{id}\n  method: get\n  operationId: getWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/wallets/{id}\n  method: put\n  operationId: updateWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/w3s/developer/wallets/balances\n  method: get\n  operationId: listDeveloperWalletBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/developer/wallets/derive\n  method: put\n  operationId: deriveWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/wallets/{id}/balances\n  method: get\n  operationId: getWalletBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/wallets/{id}/nfts\n  method: get\n  operationId: getWalletNfts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/developer/wallets/{id}/blockchains/{blockchain}\n  method: put\n  operationId: enableWalletBlockchain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/developer/sign/message\n  method: post\n  operationId: signMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/developer/sign/typedData\n  method: post\n  operationId: signTypedData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/developer/sign/transaction\n  method: post\n  operationId: signTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/developer/sign/delegateAction\n  method: post\n  operationId: signDelegateAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/transactions\n  method: get\n  operationId: listTransactions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/transactions/lowestNonceTransaction\n  method: get\n  operationId: getLowestNonceTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/developer/transactions/feeParameters\n  method: get\n  operationId: getFeeParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/w3s/developer/transactions/transfer\n  method: post\n  operationId: createTransferTransaction\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/transactions/transfer/estimateFee\n  method: post\n  operationId: estimateTransferFee\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/transactions/contractExecution/estimateFee\n  method: post\n  operationId: estimateContractExecutionFee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/transactions/validateAddress\n  method: post\n  operationId: validateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/developer/transactions/contractExecution\n  method: post\n  operationId: createContractExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/developer/transactions/walletUpgrade\n  method: post\n  operationId: createWalletUpgrade\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/developer/transactions/{id}/cancel\n  method: post\n  operationId: cancelTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/w3s/developer/transactions/{id}/accelerate\n  method: post\n  operationId: accelerateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/w3s/tokens/{id}\n  method: get\n  operationId: getToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/agentic-access/circle-agentic-access.yml
summary_line: 30 operations · 18 acting · 3 human-in-the-loop
tags:
- Blockchain
- Compliance
- Cross-Chain
- Currency
- Money
- Payments
- Stablecoin
- Transfers
- USDC
- Wallets
---
