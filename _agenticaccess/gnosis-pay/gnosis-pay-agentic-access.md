---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 22
api_specs:
- filename: gnosis-pay-auth-api-openapi.yml
  format: yaml
  label: Gnosis Pay Auth API
  slug: gnosis-pay-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-auth-api-openapi.yml
- filename: gnosis-pay-cards-api-openapi.yml
  format: yaml
  label: Gnosis Pay Cards API
  slug: gnosis-pay-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-cards-api-openapi.yml
- filename: gnosis-pay-health-api-openapi.yml
  format: yaml
  label: Gnosis Pay Health API
  slug: gnosis-pay-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-health-api-openapi.yml
- filename: gnosis-pay-kyc-api-openapi.yml
  format: yaml
  label: Gnosis Pay KYC API
  slug: gnosis-pay-kyc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-kyc-api-openapi.yml
- filename: gnosis-pay-pci-api-openapi.yml
  format: yaml
  label: Gnosis Pay PCI API
  slug: gnosis-pay-pci-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-pci-api-openapi.yml
- filename: gnosis-pay-phone-api-openapi.yml
  format: yaml
  label: Gnosis Pay Phone API
  slug: gnosis-pay-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-phone-api-openapi.yml
- filename: gnosis-pay-source-of-funds-api-openapi.yml
  format: yaml
  label: Gnosis Pay Source of Funds API
  slug: gnosis-pay-source-of-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-source-of-funds-api-openapi.yml
- filename: gnosis-pay-terms-api-openapi.yml
  format: yaml
  label: Gnosis Pay Terms API
  slug: gnosis-pay-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-terms-api-openapi.yml
- filename: gnosis-pay-user-account-api-openapi.yml
  format: yaml
  label: Gnosis Pay User Account API
  slug: gnosis-pay-user-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-user-account-api-openapi.yml
- filename: gnosis-pay-user-api-openapi.yml
  format: yaml
  label: Gnosis Pay User API
  slug: gnosis-pay-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-user-api-openapi.yml
- filename: gnosis-pay-user-movements-api-openapi.yml
  format: yaml
  label: Gnosis Pay User Movements API
  slug: gnosis-pay-user-movements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-user-movements-api-openapi.yml
- filename: gnosis-pay-3-ds-api-openapi.yml
  format: yaml
  label: Gnosis Pay 3 DS API
  slug: gnosis-pay-3-ds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-3-ds-api-openapi.yml
consequence_counts:
  physical: 1
  read: 22
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gnosis Pay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /user/withdrawal
operation_count: 44
overview: 'Gnosis Pay exposes 44 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 21 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gnosis Pay
provider_slug: gnosis-pay
slug: gnosis-pay-agentic-access
source_filename: gnosis-pay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/gnosis-pay-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 22\n    acting: 22\n  by_consequence:\n    read: 22\n    write: 21\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/siwe/{address}\n  method: get\n  operationId: Auth_getSiweMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/siwe\n  method: post\n  operationId: Auth_verifySiwe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-verification\n  method: post\n  operationId: EmailVerification_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/refresh\n  method: post\n  operationId: AuthSession_refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/logout\n  method: post\n  operationId: AuthSession_logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: post\n  operationId: User_registerUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: get\n  operationId: User_getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/onboarding\n  method: get\n  operationId: User_getUserOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /terms\n  method: get\n  operationId:\
  \ Terms_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/terms\n  method: post\n  operationId: UserTerms_acceptUserTerms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/terms\n  method: get\n  operationId: UserTerms_getUserTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /source-of-funds\n  method: get\n  operationId: SourceOfFunds_getQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /source-of-funds\n  method:\
  \ post\n  operationId: SourceOfFunds_submitAnswers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phone\n  method: get\n  operationId: Phone_getPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phone\n  method: post\n  operationId: Phone_createPhone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phone\n  method: patch\n  operationId: Phone_updatePhone\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phone/verification\n  method: post\n  operationId: Phone_requestVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/account\n  method: post\n  operationId: User_createUserAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/account\n  method: get\n  operationId: User_getUserAccount\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/account/limit\n  method: get\n  operationId: User_getUserAccountLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/account/limit\n  method: put\n  operationId: User_setUserAccountLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/virtual\n  method: post\n  operationId: Cards_createVirtualCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards\n  method: get\n  operationId: Cards_listCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardId}/limit\n  method: get\n  operationId: Cards_getCardLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardId}/limit\n  method: put\n  operationId: Cards_setCardLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/block\n  method: post\n  operationId: Cards_blockCard\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/unblock\n  method: post\n  operationId: Cards_unblockCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/cancel\n  method: post\n  operationId: Cards_cancelCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/balances/v2\n  method: get\n\
  \  operationId: User_getUserBalancesV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/deposits\n  method: get\n  operationId: User_getUserDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/statement\n  method: get\n  operationId: User_getUserStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/withdrawal\n  method: post\n  operationId: User_createUserWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /user/withdrawals\n  method: get\n  operationId: User_getUserWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kyc/import-partner-applicant\n  method: post\n  operationId: KYC_importPartnerApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pci/cards/{cardId}/challenge\n  method: get\n  operationId: PCI_getCardChallenge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pci/cards/{cardId}/details\n  method: get\n  operationId: PCI_getCardDetails\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pci/cards/{cardId}/pin\n  method: get\n  operationId: PCI_getCardPin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pci/cards/{cardId}/pin\n  method: post\n  operationId: PCI_setCardPin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pci/public-key\n  method: get\n  operationId: PCI_getPublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3ds/challenges\n  method: get\n  operationId: ThreeDS_list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3ds/challenges/{challengeId}\n  method: get\n  operationId: ThreeDS_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /3ds/challenges/{challengeId}/decision\n  method: post\n  operationId: ThreeDS_decide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /3ds/challenges/{challengeId}/decision-challenge\n  method: post\n  operationId: ThreeDS_createDecisionChallenge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: Health_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/gnosis-pay/agentic-access/gnosis-pay-agentic-access.yml
summary_line: 44 operations · 22 acting
tags:
- Company
- Payments
- Cryptocurrency
- Stablecoins
---
