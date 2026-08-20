---
acting_count: 39
action_class_counts:
  acting: 39
  connected: 32
api_specs:
- filename: due-account-api-openapi.yml
  format: yaml
  label: Due Account API
  slug: due-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-account-api-openapi.yml
- filename: due-account-wallets-api-openapi.yml
  format: yaml
  label: Due Account Wallets API
  slug: due-account-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-account-wallets-api-openapi.yml
- filename: due-blockchain-transfers-api-openapi.yml
  format: yaml
  label: Due Blockchain Transfers API
  slug: due-blockchain-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-blockchain-transfers-api-openapi.yml
- filename: due-channels-api-openapi.yml
  format: yaml
  label: Due Channels API
  slug: due-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-channels-api-openapi.yml
- filename: due-financial-institutions-api-openapi.yml
  format: yaml
  label: Due Financial Institutions API
  slug: due-financial-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-financial-institutions-api-openapi.yml
- filename: due-kyc-api-openapi.yml
  format: yaml
  label: Due KYC API
  slug: due-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-kyc-api-openapi.yml
- filename: due-markets-api-openapi.yml
  format: yaml
  label: Due Markets API
  slug: due-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-markets-api-openapi.yml
- filename: due-quote-api-openapi.yml
  format: yaml
  label: Due Quote API
  slug: due-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-quote-api-openapi.yml
- filename: due-recipients-api-openapi.yml
  format: yaml
  label: Due Recipients API
  slug: due-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-recipients-api-openapi.yml
- filename: due-simulate-pay-in-api-openapi.yml
  format: yaml
  label: Due Simulate pay-in API
  slug: due-simulate-pay-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-simulate-pay-in-api-openapi.yml
- filename: due-tos-api-openapi.yml
  format: yaml
  label: Due TOS API
  slug: due-tos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-tos-api-openapi.yml
- filename: due-transfers-api-openapi.yml
  format: yaml
  label: Due Transfers API
  slug: due-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-transfers-api-openapi.yml
- filename: due-usage-api-openapi.yml
  format: yaml
  label: Due Usage API
  slug: due-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-usage-api-openapi.yml
- filename: due-vaults-api-openapi.yml
  format: yaml
  label: Due Vaults API
  slug: due-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-vaults-api-openapi.yml
- filename: due-virtual-accounts-api-openapi.yml
  format: yaml
  label: Due Virtual Accounts API
  slug: due-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-virtual-accounts-api-openapi.yml
- filename: due-wallets-api-openapi.yml
  format: yaml
  label: Due Wallets API
  slug: due-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-wallets-api-openapi.yml
- filename: due-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Due Webhook Endpoints API
  slug: due-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-webhook-endpoints-api-openapi.yml
- filename: due-webhooks-api-openapi.yml
  format: yaml
  label: Due Webhooks API
  slug: due-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-webhooks-api-openapi.yml
consequence_counts:
  physical: 7
  read: 32
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Due Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfer_intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfer_intents/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfers/estimate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfers/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfers/{id}/funding_address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfers/{id}/transfer_intent
operation_count: 71
overview: 'Due exposes 71 API operations that an AI agent could call, of which 39 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 32 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Due
provider_slug: due
slug: due-agentic-access
source_filename: due-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/due-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 71\n  by_action_class:\n    acting: 39\n    connected: 32\n  by_consequence:\n    write: 32\n    read: 32\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /quote\n  method: post\n  operationId: CreateQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipients/{id}\n  method: delete\n  operationId: delete_v1-recipients-id\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipients/{id}\n  method: get\n  operationId: get_v1-recipients-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook_endpoints/{id}\n  method: delete\n  operationId: delete_v1-webhook-endpoints-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_endpoints/{webhookId}\n  method: delete\n  operationId: delete_v1-webhook-endpoints-webhookid\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_endpoints/{webhookId}\n  method: post\n  operationId: post_v1-webhook-endpoints-webhookid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account_categories/\n  method: get\n  operationId: get_v1-account-categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountId}\n  method: get\n  operationId: get_v1-accounts-accountid\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/\n  method: get\n  operationId: get_v1-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/channels\n  method: get\n  operationId: get_v1-channels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/financial_institutions/{country2}/{schema}\n  method: get\n  operationId: get_v1-financial-institutions-country2-schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/financial_institutions/{id}\n  method: get\n  operationId: get_v1-financial-institutions-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kyc/endorsements/{code}\n  method: get\n  operationId: get_v1-kyc-endorsements-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kyc/endorsements/{code}\n  method: post\n  operationId: post_v1-kyc-endorsements-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/endorsements\n  method: get\n  operationId: get_v1-kyc-endorsements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kyc/submissions/{submissionId}\n  method: get\n  operationId: get_v1-kyc-submissions-submissionid\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kyc/submissions\n  method: get\n  operationId: get_v1-kyc-submissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kyc\n  method: get\n  operationId: get_v1-kyc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kyc\n  method: post\n  operationId: post_v1-kyc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipients\n  method: get\n  operationId: get_v1-recipients\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipients\n  method: post\n  operationId: post_v1-recipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/token_transfers/{address}/{id}\n  method: get\n  operationId: get_v1-token-transfers-address-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/token_transfers/{address}\n  method: get\n  operationId: get_v1-token-transfers-address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tos/{token}\n\
  \  method: get\n  operationId: get_v1-tos-token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tos/{token}\n  method: post\n  operationId: post_v1-tos-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transfer_intents/{id}\n  method: get\n  operationId: get_v1-transfer-intents-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transfers/{id}\n  method: get\n  operationId: get_v1-transfers-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/transfers\n  method: get\n  operationId: get_v1-transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transfers\n  method: post\n  operationId: post_v1-transfers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: get_v1-usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/credentials\n  method: get\n  operationId: get_v1-vaults-credentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/credentials\n  method: post\n  operationId: post_v1-vaults-credentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/virtual_accounts/{key}\n  method: get\n  operationId: get_v1-virtual-accounts-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/virtual_accounts/{key}\n  method: post\n  operationId: post_v1-virtual-accounts-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/virtual_accounts/list\n  method: get\n  operationId: get_v1-virtual-accounts-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/virtual_accounts\n  method: get\n  operationId: get_v1-virtual-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/virtual_accounts\n  method: post\n  operationId: post_v1-virtual-accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/wallets\n  method: get\n  operationId: get_v1-wallets-1\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets\n  method: post\n  operationId: post_v1-wallets-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/wallets/{walletId}/balance\n  method: get\n  operationId: get_v1-wallets-walletid-balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook_endpoints/{webhookId}/events/\n  method: get\n  operationId: get_v1-webhook-endpoints-webhookid-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook_endpoints\n\
  \  method: get\n  operationId: get_v1-webhook-endpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook_endpoints\n  method: post\n  operationId: post_v1-webhook-endpoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_endpoints/events\n  method: get\n  operationId: get_v1-webhook-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{base}/{quote}\n  method: get\n  operationId: GetMarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /markets/{base}/{quote}/history\n  method: get\n  operationId: GetMarketHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets\n  method: get\n  operationId: GetMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dev/payin\n  method: post\n  operationId: post_dev-payin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts\n  method: post\n  operationId: post_v1-accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/session\n  method: post\n  operationId: post_v1-kyc-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/sessions\n  method: post\n  operationId: post_v1-kyc-sessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/sharing/sumsub\n  method: post\n  operationId: post_v1-kyc-sharing-sumsub\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/submissions/documents/{token}\n  method: post\n  operationId: post_v1-kyc-submissions-documents-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/submissions/{submissionId}/applicants\n  method: post\n  operationId: post_v1-kyc-submissions-submissionid-applicants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /v1/kyc/submissions/{submissionId}/complete\n  method: post\n  operationId: post_v1-kyc-submissions-submissionid-complete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/submissions/{submissionId}/documents\n  method: post\n  operationId: post_v1-kyc-submissions-submissionid-documents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/submissions/{submissionId}/info\n  method: post\n  operationId: post_v1-kyc-submissions-submissionid-info\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/submissions/{submissionId}/questionnaires\n  method: post\n  operationId: post_v1-kyc-submissions-submissionid-questionnaires\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/submissions/{submissionId}/relations\n  method: post\n  operationId: post_v1-kyc-submissions-submissionid-relations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transfer_intents/submit\n  method: post\n  operationId: post_v1-transfer-intents-submit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transfer_intents\n  method: post\n  operationId: post_v1-transfer-intents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transfers/estimate\n  method: post\n  operationId: post_v1-transfers-estimate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transfers/{id}/funding_address\n  method: post\n  operationId: post_v1-transfers-id-funding-address\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transfers/{id}/transfer_intent\n  method: post\n  operationId: post_v1-transfers-id-transfer-intent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transfers/quote\n  method: post\n  operationId: post_v1-transfers-quote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vaults/credentials/approve\n  method: post\n  operationId: post_v1-vaults-credentials-approve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/vaults/credentials/deactivate\n  method: post\n  operationId: post_v1-vaults-credentials-deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vaults/credentials/init\n  method: post\n  operationId: post_v1-vaults-credentials-init\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vaults/sign\n  method: post\n  operationId: post_v1-vaults-sign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vaults\n  method: post\n  operationId: post_v1-vaults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_endpoints/{webhookId}/events/{eventId}/retry\n  method: post\n  operationId: post_v1-webhook-endpoints-webhookid-events-eventid-retry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/agentic-access/due-agentic-access.yml
summary_line: 71 operations · 39 acting
tags:
- Payments
- Cross-Border Payments
- Stablecoins
- Fintech
- Virtual Accounts
- Foreign Exchange
- KYC
- Wallets
---
