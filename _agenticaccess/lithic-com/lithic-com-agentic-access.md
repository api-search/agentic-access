---
acting_count: 109
action_class_counts:
  acting: 109
  connected: 106
api_specs:
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Account Holders API
  slug: lithic-com-account-holders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Accounts API
  slug: lithic-com-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Cards API
  slug: lithic-com-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Transactions & Authorizations API
  slug: lithic-com-transactions-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Authorization Rules API
  slug: lithic-com-authorization-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Real-Time Decisioning API
  slug: lithic-com-realtime-decisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Disputes API
  slug: lithic-com-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Events & Webhooks API
  slug: lithic-com-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Financial Accounts & Statements API
  slug: lithic-com-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Balances & Holds API
  slug: lithic-com-balances-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Payments (ACH) API
  slug: lithic-com-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Ledger, Transfers & Settlement API
  slug: lithic-com-ledger-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic External Payments & Bank Accounts API
  slug: lithic-com-external-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Tokenization & Digital Wallets API
  slug: lithic-com-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Fraud & Transaction Monitoring API
  slug: lithic-com-fraud-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
consequence_counts:
  physical: 31
  read: 106
  safety-critical: 1
  write: 77
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Lithic Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/account_holders/{account_holder_token}/entities
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/book_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/book_transfers/{book_transfer_token}/retry
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/book_transfers/{book_transfer_token}/reverse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/card_bulk_orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/card_bulk_orders/{bulk_order_token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/cards/{card_token}/provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/cards/{card_token}/web_provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/disputes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/disputes/{dispute_token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/disputes/{dispute_token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/disputes/{dispute_token}/evidences
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/disputes/{dispute_token}/evidences/{evidence_token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/event_subscriptions/{event_subscription_token}/recover
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/events/{event_token}/event_subscriptions/{event_subscription_token}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/external_bank_accounts/{external_bank_account_token}/micro_deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/external_bank_accounts/{external_bank_account_token}/retry_micro_deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/external_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/external_payments/{external_payment_token}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/external_payments/{external_payment_token}/release
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/external_payments/{external_payment_token}/reverse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/external_payments/{external_payment_token}/settle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/{payment_token}/retry
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/{payment_token}/return
operation_count: 215
overview: 'Lithic exposes 215 API operations that an AI agent could call, of which 109 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 106 read, 77 write, 31 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lithic
provider_slug: lithic-com
slug: lithic-com-agentic-access
source_filename: lithic-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lithic-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 215\n  by_action_class:\n    connected: 106\n    acting: 109\n  by_consequence:\n    read: 106\n    write: 77\n    safety-critical: 1\n    physical: 31\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/account_holders\n  method: get\n  operationId: getAccountHolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account_holders\n  method: post\n  operationId: postAccountHolders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account_holders/{account_holder_token}\n  method: get\n  operationId: getAccountHolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account_holders/{account_holder_token}\n  method: patch\n  operationId: patchAccountHolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account_holders/{account_holder_token}/documents\n  method: get\n  operationId: getAccountHolderDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account_holders/{account_holder_token}/documents\n  method: post\n  operationId: postAccountHolderDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account_holders/{account_holder_token}/documents/{document_token}\n  method: get\n  operationId: getAccountHolderDocumentByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account_holders/{account_holder_token}/entities\n  method: post\n  operationId: postAccountHolderEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/account_holders/{account_holder_token}/entities/{entity_token}\n  method: delete\n  operationId: deleteAccountHolderEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_token}\n  method: get\n  operationId: getAccountByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/accounts/{account_token}\n  method: patch\n  operationId: patchAccountByToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_token}/spend_limits\n  method: get\n  operationId: getAccountSpendLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth_rules\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth_rules\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth_rules/{auth_rule_token}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth_rules/{auth_rule_token}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth_rules/{auth_rule_token}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/auth_rules/{auth_rule_token}/draft\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth_rules/{auth_rule_token}/features\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth_rules/{auth_rule_token}/promote\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth_rules/{auth_rule_token}/versions\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth_rules/{auth_rule_token}/report\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth_rules/{auth_rule_token}/backtests\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth_rules/{auth_rule_token}/backtests\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth_rules/{auth_rule_token}/backtests/{auth_rule_backtest_token}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth_rules/results\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{card_token}/signals\n  method: get\n  operationId: getCardSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_token}/signals\n  method: get\n  operationId: getAccountSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth_stream/secret\n  method: get\n  operationId: getAuthStreamSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/auth_stream/secret/rotate\n  method: post\n  operationId: rotateAuthStreamSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card_programs\n  method: get\n  operationId: getCardPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card_programs/{card_program_token}\n  method: get\n  operationId: getCardProgram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/cards\n  method: get\n  operationId: getCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards\n  method: post\n  operationId: postCards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/search_by_pan\n  method: post\n  operationId: searchCardByPan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{card_token}\n  method: get\n  operationId:\
  \ getCardByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{card_token}\n  method: patch\n  operationId: patchCardByToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{card_token}/balances\n  method: get\n  operationId: getCardBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{card_token}/financial_transactions\n  method: get\n  operationId: getCardFinancialTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/cards/{card_token}/financial_transactions/{financial_transaction_token}\n  method: get\n  operationId: getCardFinancialTransactionByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{card_token}/provision\n  method: post\n  operationId: postCardProvision\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{card_token}/web_provision\n  method: post\n  operationId: postCardWebProvision\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{card_token}/reissue\n  method: post\n  operationId: postCardReissue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{card_token}/renew\n  method: post\n  operationId: postCardRenew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{card_token}/convert_physical\n  method: post\n  operationId: postConvertPhysical\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{card_token}/spend_limits\n  method: get\n  operationId: getCardSpendLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card_authorizations/{event_token}/challenge_response\n  method: post\n  operationId: respondToAuthorizationChallenge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/card_bulk_orders\n  method: get\n  operationId: getCardBulkOrders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card_bulk_orders\n  method: post\n  operationId: postCardBulkOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/card_bulk_orders/{bulk_order_token}\n  method: get\n  operationId: getCardBulkOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card_bulk_orders/{bulk_order_token}\n  method: patch\n  operationId: patchCardBulkOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/digital_card_art\n  method: get\n  operationId: getDigitalCardArt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/digital_card_art/{digital_card_art_token}\n  method: get\n  operationId: getDigitalCardArtByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/disputes\n  method: get\n  operationId: getDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/disputes\n  method: post\n  operationId: postDisputes\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/disputes/{dispute_token}\n  method: delete\n  operationId: deleteDisputeByToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/disputes/{dispute_token}\n  method: get\n  operationId: getDisputeByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/disputes/{dispute_token}\n\
  \  method: patch\n  operationId: updateDisputeByToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/disputes/{dispute_token}/evidences\n  method: get\n  operationId: getDisputeEvidences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/disputes/{dispute_token}/evidences\n  method: post\n  operationId: postEvidenceDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/disputes/{dispute_token}/evidences/{evidence_token}\n  method: delete\n  operationId: deleteDisputeEvidenceByToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/disputes/{dispute_token}/evidences/{evidence_token}\n  method: get\n  operationId: getDisputeEvidenceByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/embed/card\n  method: get\n  operationId: getEmbedCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/fraud/transactions/{transaction_token}\n  method: get\n  operationId: getFraudReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fraud/transactions/{transaction_token}\n  method: post\n  operationId: createUpdateFraudReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{transaction_token}/enhanced_commercial_data\n  method: get\n  operationId: listEnhancedTransactionData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transaction_token}/expire_authorization\n  method: post\n  operationId:\
  \ expireAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{transaction_token}/route\n  method: post\n  operationId: routeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/events/{event_token}/enhanced_commercial_data\n  method: get\n  operationId: getEnhancedTransactionData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/event_subscriptions\n  method: get\n\
  \  operationId: getEventSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/event_subscriptions\n  method: post\n  operationId: createEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/event_subscriptions/{event_subscription_token}\n  method: delete\n  operationId: deleteEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/event_subscriptions/{event_subscription_token}\n\
  \  method: get\n  operationId: getEventSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/event_subscriptions/{event_subscription_token}\n  method: patch\n  operationId: updateEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/event_subscriptions/{event_subscription_token}/attempts\n  method: get\n  operationId: getMessageAttemptsForEventSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/event_subscriptions/{event_subscription_token}/recover\n  method: post\n  operationId: recoverEventSubscription\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/event_subscriptions/{event_subscription_token}/replay_missing\n  method: post\n  operationId: replayMissingEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/event_subscriptions/{event_subscription_token}/secret\n  method: get\n  operationId: getEventSubscriptionSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/event_subscriptions/{event_subscription_token}/secret/rotate\n  method: post\n  operationId: rotateEventSubscriptionSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{event_token}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{event_token}/attempts\n  method: get\n  operationId: getMessageAttemptsForEvent\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{event_token}/event_subscriptions/{event_subscription_token}/resend\n  method: post\n  operationId: resendEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external_bank_accounts\n  method: get\n  operationId: searchExternalBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/external_bank_accounts\n  method: post\n  operationId: createExternalBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external_bank_accounts/{external_bank_account_token}\n  method: get\n  operationId: getExternalBankAccountByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/external_bank_accounts/{external_bank_account_token}\n  method: patch\n  operationId: patchExternalBankAccountByToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external_bank_accounts/{external_bank_account_token}/micro_deposits\n  method: post\n  operationId: verifyExternalBankAccountByMicroDeposits\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external_bank_accounts/{external_bank_account_token}/pause\n  method: post\n  operationId: pauseExternalBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external_bank_accounts/{external_bank_account_token}/retry_micro_deposits\n  method: post\n  operationId: retryMicroDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external_bank_accounts/{external_bank_account_token}/retry_prenote\n  method: post\n  operationId: retryPrenote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external_bank_accounts/{external_bank_account_token}/set_verification_method\n  method: post\n  operationId: setVerificationMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/external_bank_accounts/{external_bank_account_token}/unpause\n  method: post\n  operationId: unpauseExternalBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit_products/{credit_product_token}/extended_credit\n  method: get\n  operationId: getExtendedCredit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credit_products/{credit_product_token}/prime_rates\n  method: get\n  operationId: getPrimeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credit_products/{credit_product_token}/prime_rates\n\
  \  method: post\n  operationId: createPrimeRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/financial_accounts\n  method: get\n  operationId: getFinancialAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/financial_accounts\n  method: post\n  operationId: createFinancialAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/financial_accounts/{financial_account_token}\n  method: get\n  operationId:\
  \ getFinancialAccountByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/financial_accounts/{financial_account_token}\n  method: patch\n  operationId: updateFinancialAccountByToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/financial_accounts/{financial_account_token}/balances\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/financial_accounts/{financial_account_token}/credit_configuration\n  method: get\n  operationId: getAccountCreditConfiguration\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/financial_accounts/{financial_account_token}/credit_configuration\n  method: patch\n  operationId: patchAccountCreditConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/financial_accounts/{financial_account_token}/financial_transactions\n  method: get\n  operationId: getFinancialTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/financial_accounts/{financial_account_token}/financial_transactions/{financial_transaction_token}\n  method: get\n  operationId: getFinancialTransactionByToken\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: r\n\n# --- truncated at 32 KB (65 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/agentic-access/lithic-com-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/agentic-access/lithic-com-agentic-access.yml
summary_line: 215 operations · 109 acting · 1 human-in-the-loop
tags:
- Fintech
- Card Issuing
- Payments
- Issuer Processor
- KYC
- Banking as a Service
---
