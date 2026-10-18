---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 27
api_specs:
- filename: bond-cards-api-openapi.yml
  format: yaml
  label: Bond Cards API
  slug: bond-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-cards-api-openapi.yml
- filename: bond-credit-api-openapi.yml
  format: yaml
  label: Bond Credit API
  slug: bond-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-credit-api-openapi.yml
- filename: bond-webhooks-api-openapi.yml
  format: yaml
  label: Bond Webhooks API
  slug: bond-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-webhooks-api-openapi.yml
- filename: bond-accounts-api-openapi.yml
  format: yaml
  label: Bond Accounts API
  slug: bond-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-accounts-api-openapi.yml
- filename: bond-beneficial-owners-address-api-openapi.yml
  format: yaml
  label: Bond Beneficial owners address API
  slug: bond-beneficial-owners-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-beneficial-owners-address-api-openapi.yml
- filename: bond-beneficial-owners-api-openapi.yml
  format: yaml
  label: Bond Beneficial owners API
  slug: bond-beneficial-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-beneficial-owners-api-openapi.yml
- filename: bond-business-address-api-openapi.yml
  format: yaml
  label: Bond Business address API
  slug: bond-business-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-business-address-api-openapi.yml
- filename: bond-businesses-api-openapi.yml
  format: yaml
  label: Bond Businesses API
  slug: bond-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-businesses-api-openapi.yml
- filename: bond-card-restrictions-api-openapi.yml
  format: yaml
  label: Bond Card restrictions API
  slug: bond-card-restrictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-card-restrictions-api-openapi.yml
- filename: bond-cards-api-openapi.yml
  format: yaml
  label: Bond Cards API
  slug: bond-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-cards-api-openapi.yml
- filename: bond-credit-api-openapi.yml
  format: yaml
  label: Bond Credit API
  slug: bond-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-credit-api-openapi.yml
- filename: bond-customers-api-openapi.yml
  format: yaml
  label: Bond Customers API
  slug: bond-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-customers-api-openapi.yml
- filename: bond-kyb-api-openapi.yml
  format: yaml
  label: Bond KYB API
  slug: bond-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-kyb-api-openapi.yml
- filename: bond-kyc-api-openapi.yml
  format: yaml
  label: Bond KYC API
  slug: bond-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-kyc-api-openapi.yml
- filename: bond-simulate-api-openapi.yml
  format: yaml
  label: Bond Simulate API
  slug: bond-simulate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-simulate-api-openapi.yml
- filename: bond-statements-api-openapi.yml
  format: yaml
  label: Bond Statements API
  slug: bond-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-statements-api-openapi.yml
- filename: bond-transactions-api-openapi.yml
  format: yaml
  label: Bond Transactions API
  slug: bond-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-transactions-api-openapi.yml
- filename: bond-transfer-api-openapi.yml
  format: yaml
  label: Bond Transfer API
  slug: bond-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-transfer-api-openapi.yml
- filename: bond-webhooks-api-openapi.yml
  format: yaml
  label: Bond Webhooks API
  slug: bond-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/openapi/bond-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 27
  write: 43
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bond Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers
operation_count: 71
overview: 'Bond exposes 71 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 43 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bond
provider_slug: bond
slug: bond-agentic-access
source_filename: bond-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/bond-accounts-openapi.yml, openapi/bond-business-openapi.yml, openapi/bond-cards-openapi.yml,\n  openapi/bond-credit-openapi.yml, openapi/bond-customer-openapi.yml, openapi/bond-ledger-openapi.yml,\n  openapi/bond-simulation-openapi.yml, openapi/bond-transfers-openapi.yml, openapi/bond-webhooks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 71\n  by_action_class:\n    connected: 27\n    acting: 44\n  by_consequence:\n    read: 27\n    write: 43\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: get-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: post-accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/processor_tokens\n  method: post\n  operationId: post-accounts-ptoken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}\n  method: get\n  operationId: get-accounts-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}\n\
  \  method: patch\n  operationId: patch-accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/close\n  method: post\n  operationId: close-accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/statements\n  method: get\n  operationId: get-statements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/statements/{yyyy}/{mm}\n  method: get\n  operationId:\
  \ get-statements-yyyy-mm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses\n  method: get\n  operationId: get_businesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses\n  method: post\n  operationId: post_businesses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}\n  method: get\n  operationId: get_business\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{business_id}\n  method:\
  \ delete\n  operationId: delete_business\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}\n  method: patch\n  operationId: patch_business\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/addresses\n  method: get\n  operationId: get_business_addresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{business_id}/addresses\n  method: post\n  operationId:\
  \ post_business_addresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/addresses/{address_id}\n  method: get\n  operationId: get_business_address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{business_id}/addresses/{address_id}\n  method: delete\n  operationId: delete_business_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/addresses/{address_id}\n\
  \  method: patch\n  operationId: patch_business_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/beneficial_owners\n  method: get\n  operationId: get_beneficial_owners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{business_id}/beneficial_owners\n  method: post\n  operationId: post_beneficial_owners\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}\n\
  \  method: get\n  operationId: get_beneficial_owner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}\n  method: delete\n  operationId: delete_beneficial_owner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}\n  method: patch\n  operationId: patch_beneficial_owner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}/addresses\n  method: get\n  operationId: get_beneficial_owner_addresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}/addresses\n  method: post\n  operationId: post_beneficial_owner_addresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}/addresses/{address_id}\n  method: get\n  operationId: get_beneficial_owner_address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}/addresses/{address_id}\n  method: delete\n  operationId: delete_beneficial_owner_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}/addresses/{address_id}\n  method: patch\n  operationId: patch_beneficial_owner_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}/verification-kyc\n\
  \  method: get\n  operationId: get_beneficial_owner_kyc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{business_id}/beneficial_owners/{beneficial_owner_id}/verification-kyc\n  method: post\n  operationId: post_beneficial_owner_kyc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businesses/{business_id}/verification-kyb\n  method: get\n  operationId: get_kyb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{business_id}/verification-kyb\n  method: post\n  operationId: post_kyb\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kyb\n  method: post\n  operationId: post_kyb_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kyb/{inquiry_id}/resume\n  method: post\n  operationId: post_kyb_resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards\n  method: post\n  operationId: post_cards\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards\n  method: get\n  operationId: get_cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{card_id}\n  method: get\n  operationId: get_cards_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{card_id}\n  method: patch\n  operationId: patch_cards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /cards/{card_id}/activate\n  method: post\n  operationId: post_cards_activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/close\n  method: post\n  operationId: post_cards_close\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/reissue\n  method: post\n  operationId: post_cards_reissue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/restrictions\n  method: get\n  operationId: get_cards_restrictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{card_id}/restrictions\n  method: post\n  operationId: post_cards_restrictions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/restrictions/{restriction_id}\n  method: get\n  operationId: get_cards_restrictions_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{card_id}/restrictions/{restriction_id}\n\
  \  method: patch\n  operationId: patch_cards_restrictions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/restrictions/{restriction_id}\n  method: delete\n  operationId: delete_cards_restrictions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credit/applications\n  method: post\n  operationId: post-credit-applications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credit/applications\n  method: get\n  operationId: get-credit-applications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit/applications/{application_id}\n  method: get\n  operationId: get-credit-applications-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit/applications/{application_id}\n  method: patch\n  operationId: patch-credit-applications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credit/applications/{application_id}/adverse-actions\n\
  \  method: get\n  operationId: get-adverse-actions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit/applications/{application_id}/submit\n  method: post\n  operationId: credit-applications-submit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: get_customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/\n  method: post\n  operationId: post_customers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}\n  method: get\n  operationId: get_customers_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}\n  method: patch\n  operationId: patch_customers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}\n  method: delete\n  operationId: delete_customers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/inquiries/{inquiry_id}/resume\n  method: post\n  operationId: post_resume_payload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/verification-kyc\n  method: post\n  operationId: post_verification_kyc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/verification-kyc\n  method: get\n  operationId: get_verification_kyc\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: get_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_id}\n  method: get\n  operationId: get_transaction_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /simulate/authorization\n  method: post\n  operationId: post_authorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /simulate/kyc-fail\n  method: post\n  operationId: post_simulate_kyc_fail\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /simulate/kyc-pass\n  method: post\n  operationId: post_simulate_kyc_pass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /simulate/settlement\n  method: post\n  operationId: post_settle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers\n  method: post\n\
  \  operationId: post-transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: post_webhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: get_webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook_id}\n  method: patch\n  operationId: patch_webhooks\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}\n  method: delete\n  operationId: delete_webhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bond/refs/heads/main/agentic-access/bond-agentic-access.yml
summary_line: 71 operations · 44 acting
tags:
- Company
- United States
- Banking as a Service
- Embedded Finance
- Fintech
- Payments
- Card Issuing
- Deposit Accounts
- Money Movement
- ACH
- KYC
- KYB
- Credit
- Open Finance
---
