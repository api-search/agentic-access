---
acting_count: 396
action_class_counts:
  acting: 396
  connected: 336
api_specs:
- filename: treadio-horizon-openapi.json
  format: json
  label: Tread Horizon API V1
  slug: tread-horizon-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treadio/refs/heads/main/openapi/treadio-horizon-openapi.json
consequence_counts:
  physical: 89
  read: 336
  safety-critical: 2
  write: 305
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Treadio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/reset_password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/users/{user-id}/sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/add_on_charges/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/add_on_charges/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/auth/magic_link
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/auth/otp_sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/companies/{company-id}/fuel_price_indices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/companies/{company-id}/fuel_surcharge_schedules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/companies/{company-id}/invoices/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/companies/{company-id}/invoices/{invoice-id}/add_on_charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/companies/{company-id}/invoices/{invoice-id}/add_on_charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/invoices/{invoice-id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/invoices/{invoice-id}/customer_approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/invoices/{invoice-id}/customer_pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/invoices/{invoice-id}/export
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/companies/{company-id}/invoices/{invoice-id}/invoice_line_items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/companies/{company-id}/invoices/{invoice-id}/invoice_line_items/generate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/invoices/{invoice-id}/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/invoices/{invoice-id}/send_invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/invoices/{invoice-id}/unapprove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/invoices/{invoice-id}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/jobs/bulk_send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/jobs/bulk_send_day
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/managed_companies/{managed-company-id}/users/{user-id}/invite/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/companies/{company-id}/managed_companies/{managed-company-id}/users/{user-id}/invite/sms
operation_count: 732
overview: 'tread.io exposes 732 API operations that an AI agent could call, of which 396 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 336 read, 305 write, 89 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tread.io
provider_slug: treadio
slug: treadio-agentic-access
source_filename: treadio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/treadio-horizon-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 732\n  by_action_class:\n    connected: 336\n    acting: 396\n  by_consequence:\n    read: 336\n    write: 305\n    physical: 89\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /health\n  method: get\n  operationId: get-health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts\n  method: post\n  operationId: post-v1-accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts\n  method: get\n  operationId: get-v1-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/bulk_update\n  method: patch\n  operationId: patch-v1-accounts-bulk_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/connected\n  method: post\n  operationId: post-v1-accounts-connected\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/connected\n  method: get\n  operationId: get-v1-accounts-connected\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/invite\n  method: post\n  operationId: post-v1-accounts-invite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/typeahead\n  method: get\n  operationId: get-v1-accounts-typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account-id}/auto_add_on_assignments\n  method: post\n \
  \ operationId: post-v1-accounts-account-id-auto_add_on_assignments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account-id}/auto_add_on_assignments\n  method: get\n  operationId: get-v1-accounts-account-id-auto_add_on_assignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account-id}/auto_add_ons\n  method: get\n  operationId: get-v1-accounts-account-id-auto_add_ons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account-id}/auto_add_ons/{auto-add-on-id}/customer_add_on\n  method: delete\n  operationId:\
  \ delete-v1-accounts-account-id-auto_add_ons-id-customer_add_on\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account-id}/auto_add_ons/{auto-add-on-id}/vendor_add_on\n  method: delete\n  operationId: delete-v1-accounts-account-id-auto_add_ons-id-vendor_add_on\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account-id}/scheduled_time_offs\n  method: post\n  operationId: post-v1-accounts-id-scheduled_time_offs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account-id}/scheduled_time_offs\n  method: get\n  operationId: get-v1-accounts-account-id-scheduled-time-offs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account-id}/scheduled_time_offs/available\n  method: put\n  operationId: put-v1-accounts-account-id-scheduled_time_offs-available\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account-id}/scheduled_time_offs/unavailable\n  method: put\n  operationId:\
  \ put-v1-accounts-account-id-scheduled_time_offs-unavailable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account-id}/scheduled_time_offs/{id}\n  method: delete\n  operationId: delete-v1-accounts-account-id-scheduled_time_offs-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}\n  method: get\n  operationId: get-v1-accounts-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}\n\
  \  method: patch\n  operationId: patch-v1-accounts-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}\n  method: delete\n  operationId: delete-v1-accounts-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/add_on_charges/{id}\n  method: get\n  operationId: get-v1-add-on-charges-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/add_on_charges/{id}\n  method: patch\n  operationId: patch-v1-add-on-charges-id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/add_on_charges/{id}\n  method: delete\n  operationId: delete-v1-add-on-charges-id\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/add_ons\n  method: post\n  operationId: post-v1-add_ons\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/add_ons\n  method: get\n  operationId: get-v1-add_ons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/add_ons/{id}\n  method: get\n  operationId: get-v1-add_ons-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/add_ons/{id}\n  method: patch\n  operationId: patch-v1-add_ons-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agave/customers/{id}\n  method: patch\n  operationId: patch-v1-agave-customers-id\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agave/items/{id}\n  method: patch\n  operationId: patch-v1-agave-items-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agave/ledger_accounts/{id}\n  method: patch\n  operationId: patch-v1-agave-ledger_accounts-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/agave/link_tokens\n  method: post\n  operationId: post-v1-agave-link_tokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agave/linked_accounts\n  method: post\n  operationId: post-v1-agave-linked_accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agave/linked_accounts\n  method: get\n  operationId: get-v1-agave-linked_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agave/linked_accounts/{id}\n\
  \  method: delete\n  operationId: delete-v1-users-me-agave-linked_accounts-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agave/linked_accounts/{linked-account-id}/customers\n  method: get\n  operationId: get-v1-agave-linked_accounts-linked-account-id-customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agave/linked_accounts/{linked-account-id}/customers/accounts/typeahead\n  method: get\n  operationId: get-v1-linked_accounts-linked-account-id-customers-accounts-typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agave/linked_accounts/{linked-account-id}/import\n\
  \  method: put\n  operationId: put-v1-agave-linked_accounts-linked-account-id-import\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agave/linked_accounts/{linked-account-id}/items\n  method: get\n  operationId: get-v1-agave-linked_accounts-linked-account-id-items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agave/linked_accounts/{linked-account-id}/items/add_ons/typeahead\n  method: get\n  operationId: get-v1-agave-linked_accounts-linked-account-id-items-add_ons-typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agave/linked_accounts/{linked-account-id}/items/services/typeahead\n\
  \  method: get\n  operationId: get-v1-agave-linked_accounts-linked-account-id-items-services-typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agave/linked_accounts/{linked-account-id}/ledger_accounts\n  method: get\n  operationId: get-v1-agave-linked_accounts-linked-account-id-ledger_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agave/linked_accounts/{linked-account-id}/vendors\n  method: get\n  operationId: get-v1-agave-linked_accounts-linked-account-id-vendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agave/linked_accounts/{linked-account-id}/vendors/accounts/typeahead\n  method: get\n  operationId: get-v1-linked_accounts-linked-account-id-vendors-accounts-typeahead\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agave/vendors/{id}\n  method: patch\n  operationId: patch-v1-agave-vendors-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/forgot_password\n  method: post\n  operationId: post-v1-auth-forgot_password\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/login\n  method: post\n  operationId: post-v1-auth-login\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/login\n  method: delete\n  operationId: delete-v1-auth-login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/magic_link\n  method: post\n  operationId: post-v1-auth-magic_link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/auth/magic_link/login\n  method: post\n  operationId: post-v1-auth-magic_link-login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp_sms\n  method: post\n  operationId: post-v1-auth-otp_sms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/otp_sms/login\n  method: post\n  operationId: post-v1-auth-otp_sms-login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/reset_password\n  method: post\n  operationId: post-v1-auth-reset_password\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/signup\n  method: post\n  operationId: post-v1-auth-signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/sso/login\n  method: post\n  operationId: post-v1-auth-sso-login\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth_methods\n  method: post\n  operationId: post-v1-auth_methods\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auto_add_on_assignments/{id}\n  method: patch\n  operationId: patch-v1-auto_add_on_assignments-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/auto_add_on_assignments/{id}\n  method: delete\n  operationId: delete-v1-auto_add_on_assignments-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bulk_downloads\n  method: post\n  operationId: post-v1-bulk_downloads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies\n  method: post\n  operationId: post-v1-companies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies\n  method: get\n  operationId: get-v1-companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/tread_id/{tread-id}\n  method: get\n  operationId: get-v1-companies-tread_id-tread-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/typeahead\n  method: get\n  operationId: get-v1-companies-typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/account_external_truck_identifiers\n  method: get\n  operationId: get-v1-companies-company-id-account-external-truck-identifiers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/account_external_truck_identifiers/{id}\n  method: get\n  operationId: get-v1-companies-account_external_truck_identifiers-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/account_external_truck_identifiers/{id}\n  method: patch\n  operationId: patch-v1-companies-account_external_truck_identifiers-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/account_external_truck_identifiers/{id}\n  method: delete\n  operationId: delete-v1-companies-account_external_truck_identifiers-id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/accounts\n  method: get\n  operationId: get-v1-companies-company-id-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/accounts/capacity/typeahead\n  method: get\n  operationId: get-v1-companies-accounts-capacity-typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/accounts/connected\n  method: post\n  operationId: post-v1-companies-company-id-accounts-connected\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/accounts/connected\n  method: get\n  operationId: get-v1-companies-company-id-accounts-connected\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/accounts/invite\n  method: post\n  operationId: post-v1-companies-company-id-accounts-invite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/accounts/typeahead\n  method: get\n  operationId:\
  \ get-v1-companies-accounts-typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/accounts/{account-id}/compliance_documents\n  method: post\n  operationId: post-account-compliance-documents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/accounts/{account-id}/compliance_documents\n  method: get\n  operationId: get-account-compliance-documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/accounts/{account-id}/compliance_documents/checklist\n  method: get\n\
  \  operationId: get-account-compliance-checklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/accounts/{account-id}/compliance_documents/{id}\n  method: get\n  operationId: get-account-compliance-document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/accounts/{account-id}/compliance_documents/{id}\n  method: patch\n  operationId: patch-account-compliance-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/accounts/{account-id}/compliance_documents/{id}\n\
  \  method: delete\n  operationId: delete-account-compliance-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/add_ons\n  method: post\n  operationId: post-v1-companies-company-id-add_ons\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/add_ons\n  method: get\n  operationId: get-v1-companies-company-id-add_ons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/companies/{company-id}/add_ons/typeahead\n  method: get\n  operationId: get-v1-companies-company-id-add_ons-typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/add_ons/{id}/fuel_surcharge_rate\n  method: get\n  operationId: get-v1-companies-company-id-add_ons-id-fuel_surcharge_rate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/children\n  method: get\n  operationId: get-v1-companies-id-children\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/children/typeahead\n  method: get\n  operationId: get-v1-companies-company-id-accounts-typeahead\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/company_day_job_stats/{date}\n  method: get\n  operationId: get-v1-companies-company-id-company-day-job-stats-date\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/company_shares\n  method: post\n  operationId: post-v1-companies-company_id-company_shares\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/company_shares\n  method: get\n  operationId: get-v1-companies-company_id-company_shares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/company_shares/{id}\n  method: patch\n  operationId: patch-v1-companies-company-id-company_shares-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/company_shares/{id}\n  method: delete\n  operationId: delete-v1-companies-company-id-company_shares-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/compliance_check\n  method: get\n  operationId: get-v1-companies-company-id-compliance-check\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/compliance_document_types\n  method: post\n  operationId: post-v1-companies-company-id-compliance-document-types\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/compliance_document_types\n  method: get\n  operationId: get-v1-companies-company-id-compliance-document-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/compliance_document_types/{id}\n  method: get\n  operationId: get-v1-companies-company-id-compliance-document-types-id\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/compliance_document_types/{id}\n  method: patch\n  operationId: patch-v1-companies-company-id-compliance-document-types-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company-id}/compliance_document_types/{id}\n  method: delete\n  operationId: delete-v1-companies-company-id-compliance-document-types-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/companies/{company-id}/connected_companies\n  method: get\n  operationId: get-v1-companies-company-id-connected_companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/connected_companies/typeahead\n  method: get\n  operationId: get-v1-companies-company-id-connected_companies-typeahead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company-id}/data_export/tickets/day/{date}\n  method: get\n  operationId: get-v1-companies-daily-export-tickets-day\n  x-agentic-access:\n\n\n# --- truncated at 32 KB (239 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/treadio/refs/heads/main/agentic-access/treadio-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treadio/refs/heads/main/agentic-access/treadio-agentic-access.yml
summary_line: 732 operations · 396 acting · 2 human-in-the-loop
tags:
- Company
- Construction
- Logistics
- Transportation Management
- Dispatch
- Fleet Management
- Bulk Materials
- Trucking
- Webhooks
- API
---
