---
acting_count: 66
action_class_counts:
  acting: 66
  connected: 87
api_specs:
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Connect API
  slug: bud-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud First-Party Ingestion API
  slug: bud-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Customers Platform API
  slug: bud-customers-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Financial Data API
  slug: bud-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Enrichment API
  slug: bud-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Financial Insights API
  slug: bud-financial-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Intelligent Search API
  slug: bud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Affordability and Assess API
  slug: bud-affordability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Customer Characteristics API
  slug: bud-characteristics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Goals and Budgets API
  slug: bud-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Payments API
  slug: bud-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Embedded Widgets API
  slug: bud-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
consequence_counts:
  physical: 10
  read: 87
  safety-critical: 1
  write: 55
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Bud Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/open-banking/account-access-consent/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/authorisation-codes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/scheduled
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/scheduled/bud-pay-url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/scheduled/{payment_id}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/single
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/single/bud-pay-url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/single/{payment_id}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/standing-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/standing-order/bud-pay-url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/standing-order/{payment_id}/confirm
operation_count: 153
overview: 'Bud Financial exposes 153 API operations that an AI agent could call, of which 66 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 87 read, 55 write, 10 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bud Financial
provider_slug: bud-co
slug: bud-co-agentic-access
source_filename: bud-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bud-platform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 153\n  by_action_class:\n    acting: 66\n    connected: 87\n  by_consequence:\n    write: 55\n    read: 87\n    safety-critical: 1\n    physical: 10\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/oauth/token\n  method: post\n  operationId: oauth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/open-banking/providers\n  method: get\n  operationId: open_banking_providers_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/open-banking/authorisation-gateway-url\n  method: post\n  operationId: v2_ob_authorisation_gateway_url_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/open-banking/authorisation-url\n  method: post\n  operationId: open_banking_authorisation_url_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/open-banking/authorisation-url/{task_id}\n  method: get\n\
  \  operationId: open_banking_authorisation_url_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-banking/authorisation-codes\n  method: post\n  operationId: v1_open_banking_authorisation_codes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/open-banking/authorisation-codes\n  method: post\n  operationId: v2_open_banking_authorisation_codes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/open-banking/connect/{connection_task_id}\n\
  \  method: get\n  operationId: open_banking_connect_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-banking/refresh\n  method: post\n  operationId: open_banking_refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/open-banking/refresh/{task_id}\n  method: get\n  operationId: open_banking_refresh_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-banking/v2/refresh\n  method: post\n  operationId: v2_open_banking_refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-banking/v2/refresh/{task_id}\n  method: get\n  operationId: v2_open_banking_refresh_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-banking/account-access-consents\n  method: get\n  operationId: open_banking_connections_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-banking/account-access-consent/revoke\n  method: post\n  operationId: open_banking_account_access_consent_revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/open-banking/account-access-consent/revoke/{task_id}\n  method: get\n  operationId: open_banking_account_access_consent_revoke_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-banking/account-access-consents/{consent_id}/reconfirm\n  method: post\n  operationId: open_banking_consents_reconfirm_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ingest/accounts\n  method: post\n  operationId: v2_ingest_accounts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingestion/v3/accounts/close\n  method: post\n  operationId: v3_ingest_accounts_close_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingestion/v3/accounts/reopen\n  method: post\n  operationId: v3_ingest_accounts_reopen_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ingest/transactions\n  method:\
  \ post\n  operationId: v2_ingest_transactions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingestion/v3/transactions/book\n  method: post\n  operationId: v3_ingest_transactions_book_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingestion/v3/transactions/decline\n  method: post\n  operationId: v3_ingest_transactions_decline_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingestion/v3/tasks/{task_id}\n  method: get\n  operationId: v3_ingest_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/v3/customers\n  method: post\n  operationId: platform_v3_customers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/v3/customers\n  method: get\n  operationId: platform_v3_customers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/v3/customers/batch\n  method: post\n  operationId:\
  \ platform_v3_customers_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/v3/customers/{customer_id}\n  method: delete\n  operationId: platform_v3_customers_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/v3/customers/idempotent-identifier/{customer_idempotent_identifier}\n  method: delete\n  operationId: platform_v3_customers_idempotent_identifier_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/v3/customers/{customer_id}/{task_id}\n  method: get\n  operationId: platform_v3_customers_delete_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: post\n  operationId: customers_create_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customers\n  method: post\n  operationId: customers_create_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}\n  method: delete\n  operationId: customers_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/context\n  method: get\n  operationId: v1_customer_context_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/context\n  method: put\n  operationId: v1_customer_context_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/v2/categories/models\n  method: get\n  operationId: resources_v2_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/v2/categories\n  method: get\n  operationId: resources_v2_categories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregations/v2/totals/categories\n  method: get\n  operationId: v2_category_totals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregations/v2/totals/categories/trends\n  method: get\n  operationId: v2_category_totals_trends_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregations/v2/totals/essential-statistics\n  method: get\n  operationId: aggregations_v2_totals_essential_statistics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/merchants/totals\n  method: get\n  operationId: v2_merchants_totals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v3/accounts\n  method: get\n  operationId: financial_v3_accounts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v3/accounts/{account_id}\n  method: get\n  operationId: financial_v3_accounts_account_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v3/accounts/transaction-dates\n  method: get\n  operationId: financial_v3_accounts_transaction_dates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v3/balances\n  method: get\n  operationId: financial_v3_balances_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v3/accounts/{account_id}/balances\n  method: get\n  operationId: financial_v3_accounts_balances_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v2/transactions\n  method: get\n  operationId: v2_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v2/authorised-payments\n  method: get\n  operationId: financial_v2_authorised_payments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v2/accounts\n  method: get\n  operationId: financial_v2_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v2/accounts/{account_id}\n  method: get\n  operationId: financial_v2_accounts_account_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v2/accounts/{account_id}\n  method: delete\n  operationId: v2_account_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /financial/v2/balances\n  method: get\n  operationId: financial_v2_balances_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial/v2/accounts/{account_id}/balances\n  method: get\n  operationId: financial_v2_accounts_balances_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provider/{provider}\n  method: delete\n  operationId: v1_provider_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /corrections/v2/categories\n  method: post\n  operationId: corrections_v2_categories_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /corrections/v2/merchants\n  method: post\n  operationId: corrections_v2_merchants_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /corrections/v2/merchants/search/{merchant_query}\n  method: get\n  operationId: corrections_v2_merchant_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /corrections/v2/custom-merchants\n  method: post\n  operationId: corrections_v2_custom_merchants_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /corrections/v2/custom-merchants\n  method: get\n  operationId: corrections_v2_custom_merchants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /corrections/v2/categories/similar/{transaction_id}\n  method: get\n  operationId: corrections_v2_similar_categories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /corrections/v2/merchants/similar/{transaction_id}\n  method: get\n  operationId: corrections_v2_similar_merchants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /corrections/v2/merchant-feedback/merchant/{merchant_id}\n  method: post\n  operationId: corrections_v2_merchant_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goals/v1/spending-budgets\n  method: post\n  operationId: goals_v1_spending_budgets_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /goals/v1/spending-budgets\n  method: get\n  operationId: goals_v1_spending_budgets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goals/v1/spending-budgets\n  method: delete\n  operationId: goals_v1_spending_budgets_delete_all\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goals/v1/spending-budgets/{budget_id}\n  method: patch\n  operationId: goals_v1_spending_budgets_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goals/v1/spending-budgets/{budget_id}\n  method: delete\n  operationId: goals_v1_spending_budgets_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goals/v1/spending-budgets/{budget_id}/transactions\n  method: get\n  operationId: goals_v1_spending_budget_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goals/v2/savings/goal\n  method: post\n  operationId: goals_v2_savings_goal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goals/v2/savings/goals\n  method: get\n  operationId: goals_v2_savings_goals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goals/v2/savings/goals/{savings_goal_id}\n  method: get\n  operationId: goals_v2_savings_goal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goals/v2/savings/goals/{savings_goal_id}\n  method: patch\n  operationId: goals_v2_savings_goal_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /goals/v2/savings/goals/{savings_goal_id}\n  method: delete\n  operationId: goals_v2_savings_goal_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/regular-transactions\n  method: get\n  operationId: regular_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/future-transactions\n  method: get\n  operationId: v2_future_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/income\n  method: get\n  operationId: v2_income_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benefits\n  method: get\n  operationId: v1_benefits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benefits/totals\n  method: get\n  operationId: v1_benefits_totals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loans\n  method: get\n  operationId: v1_loans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/debt-collection\n  method: get\n  operationId: v1_debt_collection_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/products\n  method: get\n\
  \  operationId: insights_v2_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions\n  method: get\n  operationId: v1_subscriptions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/beta/transactions\n  method: get\n  operationId: search_beta_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/beta/transactions/{search_id}\n  method: get\n  operationId: search_beta_transactions_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/beta/transactions/{search_id}/insight\n  method: get\n  operationId: search_beta_transactions_insight_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/beta/transactions/{search_id}/insight/transactions\n  method: get\n  operationId: search_beta_transactions_insight_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assess/v1/customer-applications\n  method: post\n  operationId: v1_customer_applications_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assess/v1/customer-applications\n  method: get\n  operationId: v1_customer_applications_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assess/v1/customer-applications/{application_id}\n  method: get\n  operationId: v1_customer_application_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assess/v1/customer-applications/{application_id}\n  method: delete\n  operationId: v1_customer_application_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assess/v1/customer-applications/{application_id}/customer-links\n  method: post\n  operationId: v1_customer_applications_customer_links_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aggregations/v2/buckets\n  method: post\n  operationId: aggregations_v2_buckets_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aggregations/v2/buckets\n  method: get\n  operationId: aggregations_v2_buckets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregations/v2/buckets/{bucket_id}\n  method: get\n  operationId: aggregations_v2_bucket_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /aggregations/v2/buckets/{bucket_id}\n  method: put\n  operationId: aggregations_v2_bucket_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aggregations/v2/buckets/{bucket_id}\n  method: delete\n  operationId: aggregations_v2_bucket_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aggregations/v2/buckets/{bucket_id}/totals\n  method: get\n  operationId: aggregations_v2_bucket_totals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /affordability/v2/report\n  method: get\n  operationId: v2_affordability_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/affordability/report\n  method: get\n  operationId: v1_affordability_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/affordability/transactions\n  method: get\n  operationId: v1_affordability_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /affordability/v2/transactions\n  method: get\n  operationId: v2_affordability_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /insights/beta/report/income-expenditure\n  method: get\n  operationId: insights_beta_report_income_expenditure_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/beta/report/income-expenditure/transactions/{reference}\n  method: get\n  operationId: insights_beta_report_income_expenditure_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/beta/report/merchants\n  method: get\n  operationId: insights_beta_report_merchants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/beta/report/merchants/transactions/{reference}\n  method: get\n  operationId: insights_beta_report_merchants_transactions_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/beta/report/balance/unauthorised-overdraft\n  method: get\n  operationId: insights_beta_report_balance_unauthorised_overdraft_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/beta/report/balance/unauthorised-overdraft/transactions/{reference}\n  method: get\n  operationId: insights_beta_report_unauthorised_overdraft_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/beta/report/income-health\n  method: get\n  operationId: insights_beta_report_income_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /insights/beta/report/income-health/transactions/{reference}\n  method: get\n  operationId: insights_beta_report_income_health_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/providers\n  method: get\n  operationId: v1_payments_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/single/bud-pay-url\n  method: post\n  operationId: v1_payments_single_bud_pay_url_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - \n\n# --- truncated at 32 KB (45 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/agentic-access/bud-co-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/agentic-access/bud-co-agentic-access.yml
summary_line: 153 operations · 66 acting · 1 human-in-the-loop
tags:
- Open Banking
- Transaction Enrichment
- Categorization
- Affordability
- Payments
- AISP
- PISP
- Financial Data
- FinTech
- UK
- AI
- Machine Learning
---
