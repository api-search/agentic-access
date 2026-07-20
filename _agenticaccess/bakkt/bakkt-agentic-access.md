---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 24
api_specs:
- filename: bakkt-crypto-openapi.yml
  format: yaml
  label: Bakkt Crypto Solutions API
  slug: bakkt-crypto-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-crypto-openapi.yml
consequence_counts:
  physical: 11
  read: 24
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bakkt Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/accounts/kycTransferRecovery/{clientAccountId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/allocation/trade/batch/allocate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/allocation/trade/batch/close
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/allocation/trade/batch/open
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/orders/{clientOrderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/transfers/deposit/coin/receiveAddress
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/transfers/verifyWalletAddress
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/transfers/withdraw/coin
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apex-crypto/api/v2/transfers/withdraw/coin/estimate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/transfer
operation_count: 54
overview: 'Bakkt exposes 54 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 19 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bakkt
provider_slug: bakkt
slug: bakkt-agentic-access
source_filename: bakkt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/bakkt-crypto-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    acting: 30\n    connected: 24\n  by_consequence:\n    write: 19\n    read: 24\n    physical: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/plaidAccount/link\n  method: post\n  operationId: addBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/bankAccount\n\
  \  method: post\n  operationId: addManualBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/currency/batch/allocate\n  method: post\n  operationId: allocationCurrencyBatchAllocateCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/currency/batch/allocate/{clientTransactionId}\n  method: get\n  operationId: allocationCurrencyBatchAllocateGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/allocation/currency/batch/close\n  method: post\n  operationId: allocationCurrencyBatchClose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/currency/batch/{batchTransactionId}\n  method: get\n  operationId: allocationCurrencyBatchGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/allocation/currency/batch/open\n  method: post\n  operationId: allocationCurrencyBatchOpen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/fiat/batch/allocate\n  method: post\n  operationId: allocationFiatBatchAllocateCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/fiat/batch/allocate/{clientTransactionId}\n  method: get\n  operationId: allocationFiatBatchAllocateGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/allocation/fiat/batch/close\n  method: post\n  operationId: allocationFiatBatchClose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/fiat/batch/{batchTransactionId}\n  method: get\n  operationId: allocationFiatBatchGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/allocation/fiat/batch/open\n  method: post\n  operationId: allocationFiatBatchOpen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/gift\n  method: post\n  operationId: allocationGiftCreate\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/gift/{clientTransactionId}\n  method: get\n  operationId: allocationGiftGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/allocation/trade/batch/allocate\n  method: post\n  operationId: allocationTradeBatchAllocateCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/trade/batch/allocate/{clientTransactionId}\n\
  \  method: get\n  operationId: allocationTradeBatchAllocateGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/allocation/trade/batch/close\n  method: post\n  operationId: allocationTradeBatchClose\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/allocation/trade/batch/{batchTransactionId}\n  method: get\n  operationId: allocationTradeBatchGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/orders/{clientOrderId}/cancel\n  method:\
  \ post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/documents/{clientDocumentId}\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/v1/oauth2/token\n\
  \  method: post\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/wire-instructions\n  method: get\n  operationId: generateWireInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/accounts/{clientAccountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/accounts/{clientAccountId}/status\n  method: get\n  operationId: getAccountStatus\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/status\n  method: get\n  operationId: getApiStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/fiatAccount/balance\n  method: get\n  operationId: getFiatAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/instruments\n  method: get\n  operationId: getInstruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/jurisdictions\n  method: get\n  operationId: getJurisdictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/jurisdictions/all\n  method: get\n  operationId: getJurisdictionsAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/kyc/documentVerificationDetails\n  method: get\n  operationId: getKycDocumentVerificationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/orders/{clientOrderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/positions/{account}\n  method: get\n  operationId: getPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/transfers/withdraw/coin/{clientTransactionId}\n  method: get\n  operationId: getWithdraw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/v1/heartbeat\n  method: post\n  operationId: heartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/accounts/kycTransferRecovery/{clientAccountId}\n\
  \  method: post\n  operationId: kycTransferRecovery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/bankAccountLinking/ach\n  method: post\n  operationId: linkBankAccountAchAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/transfers/vaspLookup/{receivingWallet}\n  method: get\n  operationId: lookupVasp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/allocation/trade/batch/open\n  method: post\n  operationId: openBatchTradeAllocation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/transfers/deposit/coin/receiveAddress\n  method: post\n  operationId: postReceiveAddress\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/transfers/withdraw/coin\n  method: post\n  operationId: postWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/transfers/withdraw/coin/estimate\n  method: post\n  operationId: postWithdrawFee\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/fiatAccount/unlink\n  method: post\n  operationId: removeFiatAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/documents/{clientAccountId}/accountDocumentMetadata\n  method: get\n  operationId: retrieveAccountDocumentMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/documents/{clientDocumentId}/metadata\n  method: get\n  operationId: retrieveDocumentMetadata\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apex-crypto/api/v2/orders\n  method: post\n  operationId: submitOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/transfer\n  method: post\n  operationId: transferFiatCurrency\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /apex-crypto/api/v2/accounts/triggerKYBScreening/{clientAccountId}\n  method: post\n  operationId: triggerKYBScreening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/v1/partner/{partnerId}/party/{partnerPartyRef}/bankAccountLinking/unlink\n  method: post\n  operationId: unlinkBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/accounts/settlementMethod/update\n  method: post\n  operationId: updateAccountSettlement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apex-crypto/api/v2/transfers/verifyWalletAddress\n  method: post\n  operationId: verifyWalletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/agentic-access/bakkt-agentic-access.yml
summary_line: 54 operations · 30 acting
tags:
- Company
- Crypto Web3
- Cryptocurrency
- Digital Assets
- Trading
- Payments
- Fiat On-Ramp
- Custody
- Webhooks
- FIX Protocol
---
