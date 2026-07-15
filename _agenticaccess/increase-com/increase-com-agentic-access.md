---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 46
api_specs:
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Accounts API
  slug: increase-com-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Account Numbers API
  slug: increase-com-account-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Cards API
  slug: increase-com-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Card Payments API
  slug: increase-com-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase ACH Transfers API
  slug: increase-com-ach-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Wire Transfers API
  slug: increase-com-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Real-Time Payments API
  slug: increase-com-real-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Checks API
  slug: increase-com-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Transactions API
  slug: increase-com-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Entities API
  slug: increase-com-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Events and Webhooks API
  slug: increase-com-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Bookkeeping API
  slug: increase-com-bookkeeping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Card Profiles and Digital Wallets API
  slug: increase-com-card-profiles-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Lockboxes API
  slug: increase-com-lockboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Simulations API
  slug: increase-com-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
consequence_counts:
  physical: 16
  read: 46
  safety-critical: 1
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Increase Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /check_transfers/{check_transfer_id}/stop_payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach_prenotifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach_transfers/{ach_transfer_id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach_transfers/{ach_transfer_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /card_disputes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check_deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inbound_ach_transfers/{inbound_ach_transfer_id}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /real_time_decisions/{real_time_decision_id}/action
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /real_time_payments_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /simulations/inbound_ach_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /simulations/inbound_wire_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wire_drawdown_requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wire_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wire_transfers/{wire_transfer_id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wire_transfers/{wire_transfer_id}/cancel
operation_count: 84
overview: 'Increase exposes 84 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read, 21 write, 16 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Increase
provider_slug: increase-com
slug: increase-com-agentic-access
source_filename: increase-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/increase-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 84\n  by_action_class:\n    connected: 46\n    acting: 38\n  by_consequence:\n    read: 46\n    write: 21\n    physical: 16\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}\n  method: get\n  operationId: retrieveAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}\n  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/balance\n  method: get\n  operationId: retrieveAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/close\n  method: post\n\
  \  operationId: closeAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_numbers\n  method: get\n  operationId: listAccountNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_numbers\n  method: post\n  operationId: createAccountNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_numbers/{account_number_id}\n  method: get\n  operationId: retrieveAccountNumber\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_numbers/{account_number_id}\n  method: patch\n  operationId: updateAccountNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external_accounts\n  method: get\n  operationId: listExternalAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external_accounts\n  method: post\n  operationId: createExternalAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external_accounts/{external_account_id}\n  method: get\n  operationId: retrieveExternalAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external_accounts/{external_account_id}\n  method: patch\n  operationId: updateExternalAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /routing_numbers\n  method: get\n  operationId: listRoutingNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards\n  method: get\n  operationId: listCards\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}\n  method: get\n  operationId: retrieveCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{card_id}\n  method: patch\n  operationId: updateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /cards/{card_id}/details\n  method: get\n  operationId: retrieveCardDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_payments\n  method: get\n  operationId: listCardPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_payments/{card_payment_id}\n  method: get\n  operationId: retrieveCardPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_disputes\n  method: get\n  operationId: listCardDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_disputes\n  method: post\n  operationId: createCardDispute\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /real_time_decisions/{real_time_decision_id}\n  method: get\n  operationId: retrieveRealTimeDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /real_time_decisions/{real_time_decision_id}/action\n  method: post\n  operationId: actionRealTimeDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /ach_transfers\n  method: get\n  operationId: listACHTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach_transfers\n  method: post\n  operationId: createACHTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach_transfers/{ach_transfer_id}\n  method: get\n  operationId: retrieveACHTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach_transfers/{ach_transfer_id}/approve\n  method: post\n  operationId: approveACHTransfer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach_transfers/{ach_transfer_id}/cancel\n  method: post\n  operationId: cancelACHTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inbound_ach_transfers/{inbound_ach_transfer_id}/decline\n  method: post\n  operationId: declineInboundACHTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach_prenotifications\n  method: post\n  operationId: createACHPrenotification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wire_transfers\n  method: get\n  operationId: listWireTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wire_transfers\n  method: post\n  operationId: createWireTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wire_transfers/{wire_transfer_id}\n  method: get\n  operationId: retrieveWireTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wire_transfers/{wire_transfer_id}/approve\n  method: post\n  operationId: approveWireTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wire_transfers/{wire_transfer_id}/cancel\n  method: post\n\
  \  operationId: cancelWireTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wire_drawdown_requests\n  method: post\n  operationId: createWireDrawdownRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /real_time_payments_transfers\n  method: get\n  operationId: listRealTimePaymentsTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /real_time_payments_transfers\n  method: post\n  operationId: createRealTimePaymentsTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /real_time_payments_transfers/{real_time_payments_transfer_id}\n  method: get\n  operationId: retrieveRealTimePaymentsTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbound_real_time_payments_transfers/{inbound_real_time_payments_transfer_id}\n  method: get\n  operationId: retrieveInboundRealTimePaymentsTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_transfers\n  method: get\n  operationId: listCheckTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_transfers\n  method: post\n  operationId: createCheckTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check_transfers/{check_transfer_id}\n  method: get\n  operationId: retrieveCheckTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_transfers/{check_transfer_id}/stop_payment\n \
  \ method: post\n  operationId: stopPaymentCheckTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /check_deposits\n  method: get\n  operationId: listCheckDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_deposits\n  method: post\n  operationId: createCheckDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_id}\n  method: get\n  operationId: retrieveTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pending_transactions\n  method: get\n  operationId: listPendingTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /declined_transactions/{declined_transaction_id}\n  method: get\n  operationId: retrieveDeclinedTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities\n  method: get\n  operationId: listEntities\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities\n  method: post\n  operationId: createEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entities/{entity_id}\n  method: get\n  operationId: retrieveEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/{entity_id}/archive\n  method: post\n  operationId: archiveEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entity_supplemental_documents\n  method: post\n  operationId: createSupplementalDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}\n  method: get\n  operationId: retrieveEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_subscriptions\n  method: get\n  operationId: listEventSubscriptions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_subscriptions\n  method: post\n  operationId: createEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event_subscriptions/{event_subscription_id}\n  method: get\n  operationId: retrieveEventSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_subscriptions/{event_subscription_id}\n  method: patch\n  operationId: updateEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookkeeping_accounts\n  method: get\n  operationId: listBookkeepingAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookkeeping_accounts\n  method: post\n  operationId: createBookkeepingAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookkeeping_accounts/{bookkeeping_account_id}\n  method: patch\n  operationId: updateBookkeepingAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookkeeping_accounts/{bookkeeping_account_id}/balance\n  method: get\n  operationId: retrieveBookkeepingBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookkeeping_entry_sets\n  method: get\n  operationId: listBookkeepingEntrySets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookkeeping_entry_sets\n  method: post\n  operationId: createBookkeepingEntrySet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookkeeping_entries/{bookkeeping_entry_id}\n\
  \  method: get\n  operationId: retrieveBookkeepingEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital_card_profiles\n  method: get\n  operationId: listDigitalCardProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital_card_profiles\n  method: post\n  operationId: createDigitalCardProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /physical_card_profiles\n  method: get\n  operationId: listPhysicalCardProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /digital_wallet_tokens\n  method: get\n  operationId: listDigitalWalletTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital_wallet_tokens/{digital_wallet_token_id}\n  method: get\n  operationId: retrieveDigitalWalletToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lockboxes\n  method: get\n  operationId: listLockboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lockboxes\n  method: post\n  operationId: createLockbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lockboxes/{lockbox_id}\n  method: get\n  operationId: retrieveLockbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lockboxes/{lockbox_id}\n  method: patch\n  operationId: updateLockbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inbound_mail_items/{inbound_mail_item_id}\n  method: get\n  operationId: retrieveInboundMailItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /simulations/inbound_ach_transfers\n  method: post\n  operationId: simulateInboundACHTransfer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /simulations/card_authorizations\n  method: post\n  operationId: simulateCardAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /simulations/inbound_wire_transfers\n  method: post\n  operationId: simulateInboundWireTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/agentic-access/increase-com-agentic-access.yml
summary_line: 84 operations · 38 acting · 1 human-in-the-loop
tags:
- Payments
- Banking
- Financial Infrastructure
- ACH
- Wire Transfers
- Real-Time Payments
- Cards
- Fintech
---
