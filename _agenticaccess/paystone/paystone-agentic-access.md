---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 27
api_specs:
- filename: paystone-balance-portal-api-openapi.yml
  format: yaml
  label: Paystone Balance Portal API
  slug: paystone-balance-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-balance-portal-api-openapi.yml
- filename: paystone-client-management-api-openapi.yml
  format: yaml
  label: Paystone Client Management API
  slug: paystone-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-client-management-api-openapi.yml
- filename: paystone-contact-api-openapi.yml
  format: yaml
  label: Paystone Contact API
  slug: paystone-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-contact-api-openapi.yml
- filename: paystone-gift-account-type-api-openapi.yml
  format: yaml
  label: Paystone Gift Account Type API
  slug: paystone-gift-account-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-gift-account-type-api-openapi.yml
- filename: paystone-item-api-openapi.yml
  format: yaml
  label: Paystone Item API
  slug: paystone-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-item-api-openapi.yml
- filename: paystone-loyalty-account-type-api-openapi.yml
  format: yaml
  label: Paystone Loyalty Account Type API
  slug: paystone-loyalty-account-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-loyalty-account-type-api-openapi.yml
- filename: paystone-loyalty-transaction-api-openapi.yml
  format: yaml
  label: Paystone Loyalty Transaction API
  slug: paystone-loyalty-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-loyalty-transaction-api-openapi.yml
- filename: paystone-member-portal-api-openapi.yml
  format: yaml
  label: Paystone Member Portal API
  slug: paystone-member-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-member-portal-api-openapi.yml
- filename: paystone-merchant-management-api-openapi.yml
  format: yaml
  label: Paystone Merchant Management API
  slug: paystone-merchant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-merchant-management-api-openapi.yml
- filename: paystone-prepaid-transaction-api-openapi.yml
  format: yaml
  label: Paystone Prepaid Transaction API
  slug: paystone-prepaid-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-prepaid-transaction-api-openapi.yml
- filename: paystone-promo-account-type-api-openapi.yml
  format: yaml
  label: Paystone Promo Account Type API
  slug: paystone-promo-account-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-promo-account-type-api-openapi.yml
- filename: paystone-reward-api-openapi.yml
  format: yaml
  label: Paystone Reward API
  slug: paystone-reward-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-reward-api-openapi.yml
- filename: paystone-user-management-api-openapi.yml
  format: yaml
  label: Paystone User Management API
  slug: paystone-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-user-management-api-openapi.yml
- filename: paystone-webhook-management-api-openapi.yml
  format: yaml
  label: Paystone Webhook Management API
  slug: paystone-webhook-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-webhook-management-api-openapi.yml
consequence_counts:
  read: 27
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Paystone Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 38
overview: 'Paystone exposes 38 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paystone
provider_slug: paystone
slug: paystone-agentic-access
source_filename: paystone-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/paystone-datacandy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 27\n    acting: 11\n  by_consequence:\n    read: 27\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/clients/{accessKey}/portals/balance\n  method: get\n  operationId: api_v1clients_accessKeyportalsbalance_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients\n  method: get\n  operationId: api_v1clients_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients\n  method: post\n  operationId: api_v1clients_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/clients/{id}\n  method: get\n  operationId: api_v1clients_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{id}\n  method: patch\n  operationId: api_v1clients_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/clients/{id}/complete\n\
  \  method: post\n  operationId: api_v1clients_idcomplete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: get\n  operationId: api_contacts_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}\n  method: get\n  operationId: api_contacts_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/account-types/gift\n  method: get\n  operationId: api_v1clients_accessKeyaccount-typesgift_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/account-types/gift/{id}\n  method: get\n  operationId: api_v1clients_accessKeyaccount-typesgift_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /items/{id}\n  method: get\n  operationId: api_items_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/account-types/loyalty\n  method: get\n  operationId: api_v1clients_accessKeyaccount-typesloyalty_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/account-types/loyalty/{id}\n  method: get\n  operationId: api_v1clients_accessKeyaccount-typesloyalty_id_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty-transactions\n  method: get\n  operationId: api_loyalty-transactions_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty-transactions/{id}\n  method: get\n  operationId: api_loyalty-transactions_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/portals/member\n  method: get\n  operationId: api_v1clients_accessKeyportalsmember_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants\n  method: get\n  operationId: api_merchants_get_collection\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{id}\n  method: get\n  operationId: api_merchants_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/merchants\n  method: get\n  operationId: api_v1clients_accessKeymerchants_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/merchants\n  method: post\n  operationId: api_v1clients_accessKeymerchants_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/clients/{accessKey}/merchants/by-external-reference/{externalReference}\n  method: get\n  operationId: api_v1clients_accessKeymerchantsby-external-reference_externalReference_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/merchants/by-external-reference/{externalReference}\n  method: patch\n  operationId: api_v1clients_accessKeymerchantsby-external-reference_externalReference_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/clients/{accessKey}/merchants/{id}\n  method: get\n  operationId: api_v1clients_accessKeymerchants_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/merchants/{id}\n  method: patch\n  operationId: api_v1clients_accessKeymerchants_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prepaid-transactions\n  method: get\n  operationId: api_prepaid-transactions_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prepaid-transactions/{id}\n  method: get\n  operationId: api_prepaid-transactions_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/account-types/promo\n\
  \  method: get\n  operationId: api_v1clients_accessKeyaccount-typespromo_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/account-types/promo/{id}\n  method: get\n  operationId: api_v1clients_accessKeyaccount-typespromo_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rewards/{id}\n  method: get\n  operationId: api_rewards_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/users\n  method: get\n  operationId: api_v1clients_accessKeyusers_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v1/clients/{accessKey}/users\n  method: post\n  operationId: api_v1clients_accessKeyusers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/clients/{accessKey}/users/{username}\n  method: get\n  operationId: api_v1clients_accessKeyusers_username_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{accessKey}/users/{username}\n  method: patch\n  operationId: api_v1clients_accessKeyusers_username_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: api_webhooks_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: api_webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  operationId: api_webhooks_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: put\n  operationId: api_webhooks_id_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: patch\n  operationId: api_webhooks_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/agentic-access/paystone-agentic-access.yml
summary_line: 38 operations · 11 acting
tags:
- Payments
- Canada
- Payment Processing
- Acquiring
- Gift Cards
- Loyalty
- Subscription
- Billing
- Merchant Services
---
