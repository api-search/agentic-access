---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 34
api_specs:
- filename: hypto-banking-api-openapi.yml
  format: yaml
  label: Hypto Banking API
  slug: hypto-banking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-banking-api-openapi.yml
- filename: hypto-generate-qr-api-openapi.yml
  format: yaml
  label: Hypto Generate QR API
  slug: hypto-generate-qr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-generate-qr-api-openapi.yml
- filename: hypto-payments-api-openapi.yml
  format: yaml
  label: Hypto Payments API
  slug: hypto-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-payments-api-openapi.yml
- filename: hypto-status-api-openapi.yml
  format: yaml
  label: Hypto Status API
  slug: hypto-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-status-api-openapi.yml
- filename: hypto-upi-api-openapi.yml
  format: yaml
  label: Hypto UPI API
  slug: hypto-upi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-upi-api-openapi.yml
- filename: hypto-upi-collections-api-openapi.yml
  format: yaml
  label: Hypto UPI Collections API
  slug: hypto-upi-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-upi-collections-api-openapi.yml
- filename: hypto-webhooks-api-openapi.yml
  format: yaml
  label: Hypto Webhooks API
  slug: hypto-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hypto/openapi/hypto-webhooks-api-openapi.yml
consequence_counts:
  physical: 8
  read: 34
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hypto Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/transfers/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/upi_collections/invalid_credits/{id}/refund_action
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/upi_collections/refund/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/virtual_accounts/invalid_credits/{id}/refund_action
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/virtual_accounts/{id}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bank_transfer_status_webhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /va_transfer_status_webhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: api/upi_collections/invalid_credits/{id}/refund_status
operation_count: 65
overview: 'Hypto exposes 65 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 23 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hypto
provider_slug: hypto
slug: hypto-agentic-access
source_filename: hypto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/hypto-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    connected: 34\n    acting: 31\n  by_consequence:\n    read: 34\n    write: 23\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/status\n  method: get\n  operationId: current_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status/events_history\n  method: get\n  operationId: events_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status/upcoming_events\n\
  \  method: get\n  operationId: upcoming_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit_va_webhook\n  method: post\n  operationId: credit_va\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /va_transfer_status_webhook\n  method: post\n  operationId: va_transfer_status\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: credit_va_upi_webhook\n  method:\
  \ post\n  operationId: credit_va_upi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credit_upi_webhooks\n  method: post\n  operationId: credit_upi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upi_collection_status\n  method: post\n  operationId: upi_collection_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /bank_verification_webhook\n  method: post\n  operationId: bank_account_verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upi_id_verification_webhook\n  method: post\n  operationId: upi_id_verification_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funds_added_webhook\n  method: post\n  operationId: funds_added\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bank_transfer_status_webhook\n  method: post\n  operationId: bank_transfer_status\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /low_balance_alert_webhook\n  method: post\n  operationId: low_balance_alert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invalid_va_credit\n  method: post\n  operationId: invalid_va_credit\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connected_banking_va\n  method: post\n  operationId: va_connected_banking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: connected_banking_upi\n  method: post\n  operationId: upi_connected_banking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: api/upi_collections/invalid_credits/{id}/refund_status\n\
  \  method: post\n  operationId: invalid_upi_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: lien_marked\n  method: post\n  operationId: lien_marked\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: lien_marked_va\n  method: post\n  operationId: lien_marked_va\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /JS\n  method: get\n  operationId: JS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Android\n  method: get\n  operationId: Android\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Demo\n  method: get\n  operationId: Demo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/balance\n  method: get\n  operationId: fetch_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/connected_banking_balance\n  method: get\n  operationId: fetch_connected_banking_balance\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/transactions\n  method: get\n  operationId: account_statement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/transfers/initiate\n  method: post\n  operationId: fund_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/transfers/status/{reference_number}\n  method: get\n  operationId: fetch_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/virtual_accounts\n  method: post\n  operationId: create_virtual_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/virtual_accounts/{id}\n  method: get\n  operationId: fetch_virtual_account_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/virtual_accounts/{id}/modify\n  method: post\n  operationId: update_virtual_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/virtual_accounts/{id}/activate\n  method: post\n  operationId: activate_virtual_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/virtual_accounts/{id}/deactivate\n  method: post\n  operationId: deactivate_virtual_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/api/virtual_accounts '\n  method: get\n  operationId: list_virtual_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/virtual_accounts/search\n  method: get\n  operationId: search_virtual_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/virtual_accounts/transactions\n  method: get\n  operationId: va_txn_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/transactions/{id}\n  method: get\n  operationId: get_va_txn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/virtual_accounts/{id}/transfer\n  method: post\n  operationId: va_bank_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/virtual_accounts/{id}/transfer/{reference_number}\n  method: get\n  operationId: fetch_status_va_bank_transfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/virtual_accounts/invalid_credits\n  method: get\n  operationId: va_invalid_credits_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/virtual_accounts/invalid_credits/{id}\n  method: get\n  operationId: va_invalid_credits_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/virtual_accounts/invalid_credits/{id}/refund_action\n  method: post\n  operationId: va_invalid_credits_refund_action\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/virtual_accounts/invalid_credits/{id}/refunds\n  method: get\n  operationId: va_invalid_credits_refunds_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/virtual_accounts/invalid_credits/{id}/refund_status\n  method: get\n  operationId: va_invalid_credits_refund_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upis\n  method: post\n  operationId: create_upi\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/upis/deactivate\n  method: post\n  operationId: deactivate_upi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/upis/activate\n  method: post\n  operationId: activate_upi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/api/upis '\n  method: get\n  operationId: list_upis\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upis/search\n  method: get\n  operationId: search_upis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upis/transactions\n  method: get\n  operationId: upi_txn_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: '/api/transactions/{id} '\n  method: get\n  operationId: fetch_upi_txn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify/bank_account\n  method: post\n  operationId: verify_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/verify/bank_status/{reference_number}\n  method: get\n  operationId: bank_verification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ifscs/{ifsc}\n  method: get\n  operationId: ifsc_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify/upi_id\n  method: post\n  operationId: verify_upi_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/verify/upi_id_status/{reference_number}\n\
  \  method: get\n  operationId: upi_id_verification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upi_collections\n  method: post\n  operationId: create_upi_collect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/upi_collections/status/{order_id}\n  method: get\n  operationId: fetch_upi_collect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: '/api/upi_collections '\n  method: get\n  operationId: list_upi_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/upi_collections/search\n  method: get\n  operationId: search_upi_collect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upi_collections/invalid_credits\n  method: get\n  operationId: upi_collections_invalid_credits_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upi_collections/invalid_credits/{id}\n  method: get\n  operationId: upi_collections_invalid_credits_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upi_collections/invalid_credits/{id}/refund_action\n  method: post\n  operationId: upi_collections_invalid_credits_refund_action\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/upi_collections/invalid_credits/{id}/refunds\n  method: get\n  operationId: upi_collections_invalid_credits_refunds_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upi_collections/invalid_credits/{id}/refund_status\n  method: get\n  operationId: upi_collections_invalid_credits_refund_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upi_collections/refund/{order_id}\n  method: post\n  operationId: create_upi_collection_refund\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/hypto/agentic-access/hypto-agentic-access.yml
summary_line: 65 operations · 31 acting
tags:
- Company
- Payments
- Fintech
- Collection
---
