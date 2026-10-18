---
acting_count: 88
action_class_counts:
  acting: 88
  connected: 43
api_specs:
- filename: pliant-account-entries-api-openapi.yml
  format: yaml
  label: Pliant Account Entries API
  slug: pliant-account-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-account-entries-api-openapi.yml
- filename: pliant-accounting-projects-api-openapi.yml
  format: yaml
  label: Pliant Accounting Projects API
  slug: pliant-accounting-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-accounting-projects-api-openapi.yml
- filename: pliant-accounting-teams-api-openapi.yml
  format: yaml
  label: Pliant Accounting Teams API
  slug: pliant-accounting-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-accounting-teams-api-openapi.yml
- filename: pliant-accounting-transactions-api-openapi.yml
  format: yaml
  label: Pliant Accounting Transactions API
  slug: pliant-accounting-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-accounting-transactions-api-openapi.yml
- filename: pliant-callbacks-api-openapi.yml
  format: yaml
  label: Pliant Callbacks API
  slug: pliant-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-callbacks-api-openapi.yml
- filename: pliant-card-accounts-api-openapi.yml
  format: yaml
  label: Pliant Card Accounts API
  slug: pliant-card-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-card-accounts-api-openapi.yml
- filename: pliant-card-controls-api-openapi.yml
  format: yaml
  label: Pliant Card Controls API
  slug: pliant-card-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-card-controls-api-openapi.yml
- filename: pliant-card-copilots-api-openapi.yml
  format: yaml
  label: Pliant Card Copilots API
  slug: pliant-card-copilots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-card-copilots-api-openapi.yml
- filename: pliant-card-sensitive-data-api-openapi.yml
  format: yaml
  label: Pliant Card Sensitive Data API
  slug: pliant-card-sensitive-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-card-sensitive-data-api-openapi.yml
- filename: pliant-cardholders-api-openapi.yml
  format: yaml
  label: Pliant Cardholders API
  slug: pliant-cardholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-cardholders-api-openapi.yml
- filename: pliant-cards-api-openapi.yml
  format: yaml
  label: Pliant Cards API
  slug: pliant-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-cards-api-openapi.yml
- filename: pliant-custom-fields-api-openapi.yml
  format: yaml
  label: Pliant Custom Fields API
  slug: pliant-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-custom-fields-api-openapi.yml
- filename: pliant-organizations-api-openapi.yml
  format: yaml
  label: Pliant Organizations API
  slug: pliant-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-organizations-api-openapi.yml
- filename: pliant-payments-api-openapi.yml
  format: yaml
  label: Pliant Payments API
  slug: pliant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-payments-api-openapi.yml
- filename: pliant-receipt-automatching-api-openapi.yml
  format: yaml
  label: Pliant Receipt Automatching API
  slug: pliant-receipt-automatching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-receipt-automatching-api-openapi.yml
- filename: pliant-receipts-api-openapi.yml
  format: yaml
  label: Pliant Receipts API
  slug: pliant-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-receipts-api-openapi.yml
- filename: pliant-statements-api-openapi.yml
  format: yaml
  label: Pliant Statements API
  slug: pliant-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-statements-api-openapi.yml
- filename: pliant-test-data-generator-sandbox-only-api-openapi.yml
  format: yaml
  label: Pliant Test Data Generator (Sandbox-only) API
  slug: pliant-test-data-generator-sandbox-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-test-data-generator-sandbox-only-api-openapi.yml
- filename: pliant-transactions-api-openapi.yml
  format: yaml
  label: Pliant Transactions API
  slug: pliant-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/openapi/pliant-transactions-api-openapi.yml
consequence_counts:
  physical: 5
  read: 43
  safety-critical: 2
  write: 81
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Pliant Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /cards/{cardId}/card-controls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cards/{cardId}/terminate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /callbacks/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /card-accounts/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/subscription
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payments/subscription
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /test-data-generator/organizations/prefund
operation_count: 131
overview: 'Pliant exposes 131 API operations that an AI agent could call, of which 88 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 43 read, 81 write, 5 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pliant
provider_slug: pliant
slug: pliant-agentic-access
source_filename: pliant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/pliant-customer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 131\n  by_action_class:\n    connected: 43\n    acting: 88\n  by_consequence:\n    read: 43\n    write: 81\n    physical: 5\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /account-entries\n  method: get\n  operationId: get-account-entries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-entries/subscription\n  method: post\n  operationId: create-account-entry-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-entries/subscription\n  method: delete\n  operationId: remove-account-entry-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/projects\n  method: get\n  operationId: get-projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/projects\n  method: post\n  operationId: create-project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/projects/subscription\n  method: post\n  operationId: create-accounting-project-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/projects/subscription\n  method: delete\n  operationId: remove-accounting-project-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/projects/team/assign\n  method: post\n  operationId: assign-project-team\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/projects/team/unassign\n  method: post\n  operationId: unassign-project-team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/projects/{projectId}\n  method: put\n  operationId: update-project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /accounting/projects/{projectId}\n  method: delete\n  operationId: delete-project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/teams\n  method: get\n  operationId: get-teams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/teams\n  method: post\n  operationId: create-team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/teams/subscription\n  method:\
  \ post\n  operationId: create-accounting-team-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/teams/subscription\n  method: delete\n  operationId: remove-accounting-team-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/teams/{teamId}\n  method: put\n  operationId: update-team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/teams/{teamId}\n  method: delete\n  operationId: delete-team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/teams/{teamId}/cardholder/assign\n  method: post\n  operationId: assign-to-team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/teams/{teamId}/cardholder/unassign\n  method: post\n  operationId: unassign-from-team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/teams/{teamId}/deactivate\n  method: post\n  operationId: deactivate-team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/transactions\n  method: post\n  operationId: get-accounting-transactions-batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/transactions/subscription\n  method: post\n  operationId: create-accounting-transaction-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/transactions/subscription\n  method: delete\n  operationId: remove-accounting-transaction-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/transactions/{accountingTransactionId}/custom-fields\n  method: patch\n  operationId: update-custom-fields-on-accounting-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /callbacks\n  method: get\n  operationId: search-callbacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /callbacks/resend\n  method: post\n  operationId: resend-callbacks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /callbacks/{callbackId}\n  method: get\n  operationId: get-callback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-accounts\n  method: get\n  operationId: get-card-accounts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-accounts\n  method: post\n  operationId: create-card-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-accounts/available-currencies\n  method: get\n  operationId: get-card-accounts-available-currencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-accounts/subscription\n  method: post\n  operationId: create-card-account-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-accounts/subscription\n  method: delete\n  operationId: remove-card-account-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-accounts/transfer\n  method: post\n  operationId: create-card-account-transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-accounts/{cardAccountId}\n  method: get\n  operationId: get-card-account-details\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-accounts/{cardAccountId}\n  method: patch\n  operationId: update-card-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-accounts/{cardAccountId}/deactivate\n  method: post\n  operationId: deactivate-card-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-details/widget/{cardId}/otp\n  method: get\n  operationId: get-otp-for-pci-widget\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-details/{cardId}\n  method: get\n  operationId: card-pan-and-cvv-pci-vault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardholders\n  method: get\n  operationId: list-cardholders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardholders/invite\n  method: post\n  operationId: invite-cardholders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardholders/register\n  method: post\n  operationId: register-cardholders\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardholders/subscription\n  method: post\n  operationId: create-cardholder-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardholders/subscription\n  method: delete\n  operationId: remove-cardholder-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /cardholders/{cardholderId}\n  method: get\n  operationId: get-cardholder-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardholders/{cardholderId}\n  method: patch\n  operationId: update-cardholders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardholders/{cardholderId}\n  method: delete\n  operationId: deactivate-cardholder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /cards\n  method: get\n  operationId: get-cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards\n  method: post\n  operationId: issue-card-with-cardholder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/available-cards\n  method: get\n  operationId: get-available-cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/copilots/subscription\n  method: post\n  operationId: create-card-copilot-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/copilots/subscription\n  method: delete\n  operationId: remove-card-copilot-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/details\n  method: post\n  operationId: get-multiple-card-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/instant\n  method: post\n  operationId: issue-card-with-cardholder-instant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/instant-pci\n  method: post\n  operationId: issue-card-with-cardholder-instant-with-pci\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/limits/{cardId}\n  method: put\n  operationId: update-card-limit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/load\n  method: post\n  operationId: load-cards-batch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/subscription\n  method: post\n  operationId: create-card-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/subscription\n  method: delete\n  operationId: remove-cards-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}\n  method: get\n  operationId: get-single-card-details\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardId}\n  method: patch\n  operationId: update-card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/activate\n  method: post\n  operationId: activate-physical-card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/card-controls\n  method: put\n  operationId: update-card-controls-by-card\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cards/{cardId}/card-controls\n  method: get\n  operationId: get-card-controls-by-card\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardId}/copilots\n  method: put\n  operationId: update-card-copilots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/copilots/claim\n  method: put\n  operationId: claim-card-as-copilot\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/custom-fields\n  method: patch\n  operationId: update-custom-fields-on-card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/label\n  method: patch\n  operationId: update-card-label\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/lock\n\
  \  method: post\n  operationId: lock-card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/pin\n  method: get\n  operationId: get-card-pin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardId}/replace\n  method: post\n  operationId: replace-card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/terminate\n  method: post\n  operationId: terminate-card\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cards/{cardId}/tokenized-pan\n  method: post\n  operationId: card-pan-tokenized-from-pci-proxy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardId}/unlock\n  method: post\n  operationId: unlock-card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardId}/validity-period\n  method: put\n  operationId: update-card-validity-period\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardholderId}\n  method: post\n  operationId: issue-card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardholderId}/instant\n  method: post\n  operationId: issue-card-instant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardholderId}/instant-pci\n\
  \  method: post\n  operationId: issue-card-instant-with-pci\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations\n  method: get\n  operationId: list-organizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}\n  method: get\n  operationId: get-organization-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: get-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /payments/subscription\n  method: post\n  operationId: create-payment-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/subscription\n  method: delete\n  operationId: remove-payment-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}\n  method: get\n  operationId: get-payments-detail\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receipts\n  method: get\n  operationId: get-receipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receipts\n  method: post\n  operationId: upload-receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipts/automatching\n  method: post\n  operationId: upload-receipt-to-automatcher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /receipts/automatching/metadata\n  method: post\n  operationId: metadata-receipt-to-automatcher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipts/automatching/subscription\n  method: post\n  operationId: create-receipt-automatching-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipts/automatching/subscription\n  method: delete\n  operationId: remove-receipt-automatching-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipts/automatching/{automatchingTaskId}\n  method: get\n  operationId: get-receipt-automatcher-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receipts/subscription\n  method: post\n  operationId: create-receipt-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipts/subscription\n  method: delete\n  operationId: remove-receipt-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipts/{receiptId}\n  method: get\n  operationId: get-receipt-detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receipts/{receiptId}\n  method: delete\n  operationId: delete-receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipts/{receiptId}/original\n  method: get\n  operationId: receipt-original\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receipts/{receiptId}/pdf\n\
  \  method: get\n  operationId: receipt-as-pdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receipts/{receiptId}/thumbnail\n  method: get\n  operationId: receipt-thumbnail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements\n  method: get\n  operationId: get-statements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements/csv\n  method: get\n  operationId: get-statement-csv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statements/subscription\n  method: post\n  operationId: create-statement-subscription\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statements/subscription\n  method: delete\n  operationId: remove-statement-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statements/{statementId}\n  method: get\n  operationId: get-statement-detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (41 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/agentic-access/pliant-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/agentic-access/pliant-agentic-access.yml
summary_line: 131 operations · 88 acting · 2 human-in-the-loop
tags:
- Company
- Payments
- Corporate Cards
- Card Issuing
- Spend Management
- Expense Management
- Fintech
- Cards-as-a-Service
- Banking as a Service
- Travel
- Accounting
---
