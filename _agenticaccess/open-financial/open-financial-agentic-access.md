---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 18
api_specs:
- filename: open-financial-accounts-api-openapi.yml
  format: yaml
  label: Open (open.money) Accounts API
  slug: open-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-accounts-api-openapi.yml
- filename: open-financial-constants-api-openapi.yml
  format: yaml
  label: Open (open.money) Constants API
  slug: open-financial-constants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-constants-api-openapi.yml
- filename: open-financial-events-api-openapi.yml
  format: yaml
  label: Open (open.money) Events API
  slug: open-financial-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-events-api-openapi.yml
- filename: open-financial-icp-api-openapi.yml
  format: yaml
  label: Open (open.money) Icp API
  slug: open-financial-icp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-icp-api-openapi.yml
- filename: open-financial-kycs-api-openapi.yml
  format: yaml
  label: Open (open.money) Kycs API
  slug: open-financial-kycs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-kycs-api-openapi.yml
- filename: open-financial-pg-api-openapi.yml
  format: yaml
  label: Open (open.money) Pg API
  slug: open-financial-pg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-pg-api-openapi.yml
- filename: open-financial-pg-settlements-api-openapi.yml
  format: yaml
  label: Open (open.money) Pg Settlements API
  slug: open-financial-pg-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-pg-settlements-api-openapi.yml
- filename: open-financial-refund-api-openapi.yml
  format: yaml
  label: Open (open.money) Refund API
  slug: open-financial-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-refund-api-openapi.yml
- filename: open-financial-transfers-api-openapi.yml
  format: yaml
  label: Open (open.money) Transfers API
  slug: open-financial-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-transfers-api-openapi.yml
- filename: open-financial-verifications-api-openapi.yml
  format: yaml
  label: Open (open.money) Verifications API
  slug: open-financial-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/openapi/open-financial-verifications-api-openapi.yml
consequence_counts:
  physical: 5
  read: 18
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Open Financial Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refund/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pg/sandbox/payment_token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/transfers/bulk
operation_count: 39
overview: 'Open (open.money) exposes 39 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 16 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Open (open.money)
provider_slug: open-financial
slug: open-financial-agentic-access
source_filename: open-financial-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/open-financial-1-openapi.yml, openapi/open-financial-2-openapi.yml, openapi/open-financial-4-openapi.yml,\n  openapi/open-financial-5-openapi.yml, openapi/open-financial-6-openapi.yml, openapi/open-financial-8-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 21\n    connected: 18\n  by_consequence:\n    write: 16\n    read: 18\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /icp/upi/intent\n  method: post\n  operationId: upi-qr-intent-string\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg_settlements/sub_accounts\n  method: put\n  operationId: update-sub-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pg_settlements/sub_accounts\n  method: get\n  operationId: get-all-sub-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pg_settlements/sub_accounts/{{sub_account_ref_id}}\n  method: get\n  operationId: get-sub-account-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refund/batch\n  method: post\n  operationId:\
  \ batch-refund-api\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refund/batch/requery\n  method: get\n  operationId: requery-batch-refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts\n  method: get\n  operationId: accounts-get-all\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/beneficiaries/{beneficiary_id}\n  method: get\n  operationId: beneficiaries-get-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/beneficiaries/{beneficiary_id}\n  method: post\n  operationId: beneficiaries-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/beneficiaries/{beneficiary_id}\n  method: delete\n  operationId: beneficiaries-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}\n  method: get\n  operationId: accounts-get-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/balance\n  method: get\n  operationId: accounts-get-balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/beneficiaries\n  method: post\n  operationId: beneficiaries-bank-account-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/beneficiaries\n  method: get\n  operationId: beneficiaries-get-all\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deactivate\n  method: post\n  operationId:\
  \ accounts-virtual-deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/statements\n  method: get\n  operationId: accounts-get-statement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/test-balance\n  method: post\n  operationId: accounts-virtual-test-balance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/constants/business-categories\n  method: get\n\
  \  operationId: constants-business-categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/constants/business-types\n  method: get\n  operationId: constants-business-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/constants/ifsc-codes\n  method: get\n  operationId: constants-ifsc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/constants/states\n  method: get\n  operationId: constants-state-codes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n  operationId: webhooks-get-all-events\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kycs/name-match\n  method: post\n  operationId: verifications-name-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kycs/pan\n  method: post\n  operationId: verifications-pan-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kycs/verifications/bank-account/pennyless\n  method: post\n  operationId: bank-account-verification-copy-1\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kycs/verifications/vpa\n  method: post\n  operationId: verifications-vpa-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pg/sandbox/payment_token\n  method: post\n  operationId: create-payment-token\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/pg/sandbox/payment_token/{tokenvalue}/payment\n  method: get\n  operationId: status-check-api-with-payment_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transfers\n  method: post\n  operationId: transfers-virtual-accounts-create-to-account-beneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transfers\n  method: get\n  operationId: transfers-bulk-get-all\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transfers/bulk/{bulk_transfer_id}\n\
  \  method: get\n  operationId: transfers-bulk-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transfers/{transfer_id}\n  method: get\n  operationId: transfers-get-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verifications/bank-account\n  method: post\n  operationId: verifications-bank-account-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transfers/bulk\n  method: post\n  operationId: transfers-bulk-create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts\n  method: post\n  operationId: accounts-virtual-transfer-wallet-create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kycs/name-match\n  method: post\n  operationId: verifications-pan-vs-account-verification-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /pg_settlements/sub_accounts\n  method: post\n  operationId: sub-account-onboarding-api\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts\n  method: post\n  operationId: accounts-virtual-collection-tool-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts\n  method: post\n  operationId: accounts-virtual-collection-wallet-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/agentic-access/open-financial-agentic-access.yml
summary_line: 39 operations · 21 acting
tags:
- Connected Banking
- Neobank
- Small Business
- Embedded Finance
- Banking as a Service
- Payments
- Payouts
- UPI
- Accounting
- Payroll
- Expense Management
- India
- Fintech
---
