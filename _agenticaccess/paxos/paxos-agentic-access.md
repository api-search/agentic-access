---
acting_count: 61
action_class_counts:
  acting: 61
  connected: 64
api_specs:
- filename: paxos-v2-openapi-original.json
  format: json
  label: Paxos API v2
  slug: paxos-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paxos/refs/heads/main/openapi/paxos-v2-openapi-original.json
consequence_counts:
  physical: 20
  read: 64
  safety-critical: 3
  write: 38
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Paxos Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /identity/controls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /identity/controls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /identity/kycrefresh/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /profiles/{profile_id}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /profiles/{profile_id}/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rewards/payout-groups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /rewards/payout-groups/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /rewards/payout-groups/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sandbox/fiat-deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sandbox/profiles/{profile_id}/deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/crypto-deposits/{id}/reject
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/crypto-deposits/{id}/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /transfer/crypto-destination-address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/crypto-withdrawals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/deposit-addresses
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/fees/crypto-withdrawal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/fiat-accounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /transfer/fiat-accounts/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /transfer/fiat-accounts/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/fiat-deposit-instructions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/fiat-withdrawals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/internal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/paxos
operation_count: 125
overview: 'Paxos exposes 125 API operations that an AI agent could call, of which 61 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 64 read, 38 write, 20 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paxos
provider_slug: paxos
slug: paxos-agentic-access
source_filename: paxos-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/paxos-v2-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 125\n  by_action_class:\n    connected: 64\n    acting: 61\n  by_consequence:\n    read: 64\n    write: 38\n    physical: 20\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /profiles\n  method: get\n  operationId: ListProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - funding:read_profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles\n  method: post\n  operationId: CreateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - funding:write_profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile_id}\n  method: get\n  operationId: GetProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - funding:read_profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}\n  method: put\n  operationId: UpdateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - funding:write_profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile_id}/balances\n  method: get\n  operationId: ListProfileBalances\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - funding:read_profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}/balances/{asset}\n  method: get\n  operationId: GetProfileBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - funding:read_profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}/deactivate\n  method: put\n  operationId: DeactivateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - funding:write_profile\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/profiles/{profile_id}/deposit\n  method: post\n  operationId: CreateSandboxDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    scope:\n    - funding:read_profile\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/controls\n  method: get\n  operationId: ListIdentityControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity:read_identity_control\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/controls\n  method: delete\n  operationId: DeleteIdentityControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - identity:write_identity_control\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /identity/controls\n  method: post\n  operationId: CreateIdentityControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - identity:write_identity_control\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /identity/identities\n  method: get\n  operationId: ListIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity:read_identity\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/identities\n  method: post\n  operationId: CreateIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_identity\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/identities/{identity_id}/documents\n  method: get\n  operationId: ListIdentityDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity:read_identity\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/identities/{identity_id}/documents\n  method: put\n  operationId: DocumentUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_identity\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/identities/{id}\n  method: get\n  operationId: GetIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    scope:\n    - identity:read_identity\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/identities/{id}\n  method: put\n  operationId: UpdateIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_identity\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/institution-members\n  method: post\n  operationId: AddInstitutionMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_identity\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/institution-members/{id}\n  method: delete\n  operationId:\
  \ DeleteInstitutionMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_identity\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/accounts\n  method: get\n  operationId: ListAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity:read_account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/accounts\n  method: post\n  operationId: CreateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_account\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /identity/accounts\n  method: put\n  operationId: UpdateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_account\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/accounts/{id}\n  method: get\n  operationId: GetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - identity:read_account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/account-members\n  method: post\n  operationId: AddAccountMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_account\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /identity/account-members/{id}\n  method: delete\n  operationId: DeleteAccountMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_account\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/identities/{identity_id}/kyc-refresh\n  method: post\n  operationId: SandboxStartKycRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_identity\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/identities/{id}/sandbox-status\n  method: put\n  operationId: SandboxSetIdentityStatus\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_identity\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/kycrefresh/force-start\n  method: post\n  operationId: SandboxForceStartKycRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - identity:write_identity\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/kycrefresh/reset\n  method: post\n  operationId: SandboxResetKycRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - identity:write_identity\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /all-markets/prices\n  method: get\n  operationId: ListPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /executions\n  method: get\n  operationId: ListExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:read_order\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuer-quote\n  method: post\n  operationId: CreateIssuerQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - exchange:write_issuer_quote\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /issuer-quote/settlement-availability\n  method: get\n  operationId: GetIssuerQuoteSettlementAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:write_issuer_quote\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issuer-quote/{quote_id}\n  method: post\n  operationId: CreateIssuerQuoteExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - exchange:write_issuer_quote_execution\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issuer-quotes\n  method: get\n  operationId: ListIssuerQuoteExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:read_issuer_quote_execution\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets\n  method: get\n  operationId: ListMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{market}/historical-prices\n  method: get\n  operationId: ListHistoricalPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:historical_prices\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{market}/order-book\n  method: get\n  operationId: GetOrderBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{market}/recent-executions\n  method: get\n  operationId: ListRecentExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /markets/{market}/ticker\n  method: get\n  operationId: GetTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: ListOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:read_order\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}/executions\n  method: get\n  operationId: ListProfileExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:read_order\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}/orders\n  method: get\n  operationId: ListProfileOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:read_order\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}/orders\n  method: post\n  operationId: CreateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - exchange:write_order\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile_id}/orders/{id}\n  method: get\n  operationId: GetOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:read_order\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}/orders/{id}\n  method: delete\n  operationId: CancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - exchange:write_order\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile_id}/quote-executions\n  method: get\n  operationId: ListQuoteExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:read_quote_execution\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}/quote-executions\n  method: post\n  operationId: CreateQuoteExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - exchange:write_quote_execution\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile_id}/quote-executions/{id}\n\
  \  method: get\n  operationId: GetQuoteExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:read_quote_execution\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotes\n  method: get\n  operationId: ListQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exchange:read_quote\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sandbox/fiat-deposits\n  method: post\n  operationId: InitiateSandboxFiatDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_sandbox_fiat_deposit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/crypto-deposits/{id}/reject\n\
  \  method: post\n  operationId: RejectCryptoDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:reject_crypto_deposit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/crypto-deposits/{id}/update\n  method: post\n  operationId: UpdateCryptoDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:update_crypto_deposit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/crypto-destination-address\n  method: put\n  operationId: PutCryptoDestinationAddress\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_crypto_destination_address\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/crypto-destination-addresses\n  method: get\n  operationId: ListCryptoDestinationAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transfer:read_crypto_destination_address\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/crypto-withdrawals\n  method: post\n  operationId: CreateCryptoWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_crypto_withdrawal\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/deposit-addresses\n  method: get\n  operationId: ListDepositAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transfer:read_deposit_address\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/deposit-addresses\n  method: post\n  operationId: CreateDepositAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_deposit_address\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/fees/crypto-withdrawal\n  method: post\n \
  \ operationId: CreateCryptoWithdrawalFee\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - fee:write_crypto_withdrawal_fee\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/fiat-accounts\n  method: get\n  operationId: ListFiatAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transfer:read_fiat_account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/fiat-accounts\n  method: post\n  operationId: CreateFiatAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_fiat_account\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/fiat-accounts/{id}\n  method: get\n  operationId: GetFiatAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transfer:read_fiat_account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/fiat-accounts/{id}\n  method: delete\n  operationId: DeleteFiatAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_fiat_account\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/fiat-accounts/{id}\n  method: put\n  operationId: UpdateFiatAccount\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_fiat_account\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/fiat-deposit-instructions\n  method: get\n  operationId: ListFiatDepositInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transfer:read_fiat_deposit_instructions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/fiat-deposit-instructions\n  method: post\n  operationId: CreateFiatDepositInstructions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_fiat_deposit_instructions\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/fiat-deposit-instructions/{id}\n  method: get\n  operationId: GetFiatDepositInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transfer:read_fiat_deposit_instructions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/fiat-withdrawals\n  method: post\n  operationId: CreateFiatWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_fiat_withdrawal\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/internal\n  method: post\n  operationId:\
  \ CreateInternalTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_internal_transfer\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/limits/utilizations\n  method: get\n  operationId: ListTransferLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transfer:read_transfer_limit\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/paxos\n  method: post\n  operationId: CreatePaxosTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transfer:write_paxos_transfer\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/transfers\n  method: get\n  operationId: ListTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transfer:read_transfer\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/transfers/{id}\n  method: get\n  operationId: GetTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transfer:read_transfer\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travelrule/vasps\n  method: get\n  operationId: ListVasps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travelrule/vasps/{id}\n  method: get\n  operationId: GetVasp\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tax/tax-form-revisions\n  method: get\n  operationId: ListTaxFormRevisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tax:read_tax_form\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tax/tax-forms\n  method: get\n  operationId: ListTaxForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tax:read_tax_form\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversion/stablecoins\n  method: get\n  operationId: ListStablecoinConversions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - conversion:read_conversion_stablecoin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversion/stablecoins\n  method: post\n  operationId: CreateStablecoinConversion\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - conversion:write_conversion_stablecoin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversion/stablecoins/{id}\n  method: get\n  operationId: GetStablecoinConversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - conversion:read_conversion_stablecoin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversion/stablecoins/{id}\n  method: delete\n  operationId: CancelStablecoinConversion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - conversion:write_conversion_stablecoin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /settlement/transactions\n  method: get\n  operationId: ListTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - settlement:read_transaction\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settlement/transactions\n  method: post\n  operationId: CreateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - settlement:write_transaction\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settlement/transactions/{transaction_id}\n  method: get\n  operationId: GetTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - settlement:read_transaction\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /settlement/transactions/{transaction_id}\n  method: delete\n  operationId: CancelTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - settlement:write_transaction\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settlement/transactions/{transaction_id}/affirm\n  method: put\n  operationId: AffirmTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - settlement:write_transaction\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rewards/monitor/address\n  method: get\n  operationId: ListMonitoringAddress\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - rewards:read_monitoring_address\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rewards/monitor/address\n  method: post\n  operationId: CreateMonitoringAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - rewards:write_monitoring_address\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rewards/monitor/address/{id}\n  method: get\n  operationId: GetMonitoringAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - rewards:read_monitoring_address\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rewards/monitor/address/{id}\n  method: put\n  operationId: UpdateMonitoringAddress\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - rewards:write_monitoring_address\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statements\n  method: get\n  operationId: ListStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - statements:read_statement\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements/payments\n  method: get\n  operationId: ListPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - statements:read_payment\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: ListEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n  \
  \  - events:read_event\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n  operationId: GetEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - events:read_event\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-creds/credentials\n  method: get\n  operationId: ListApiCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api_creds:read_credentials\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-creds/credentials/{client_id}\n  method: delete\n  operationId: DeleteApiCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api_creds:delete_credentials\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /orchestration/orchestrations\n  method: get\n  operationId: ListOrchestrations\n  x-agentic-access:\n   \n\n# --- truncated at 32 KB (41 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/paxos/refs/heads/main/agentic-access/paxos-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paxos/refs/heads/main/agentic-access/paxos-agentic-access.yml
summary_line: 125 operations · 61 acting · 3 human-in-the-loop
tags:
- Company
- Stablecoins
- Cryptocurrency
- Payments
- Crypto Brokerage
- Trading
- Custody
- Blockchain
- Financial Services
- Digital Assets
---
