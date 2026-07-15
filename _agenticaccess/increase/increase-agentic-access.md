---
acting_count: 132
action_class_counts:
  acting: 132
  connected: 106
api_specs:
- filename: increase-openapi.json
  format: json
  label: Increase ACH API
  slug: increase-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Wire Transfers API
  slug: increase-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Real-Time Payments API
  slug: increase-real-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Check API
  slug: increase-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Cards API
  slug: increase-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Accounts API
  slug: increase-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
consequence_counts:
  physical: 64
  read: 106
  safety-critical: 1
  write: 67
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Increase Agentic Access
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
  path: /account_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account_transfers/{account_transfer_id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account_transfers/{account_transfer_id}/cancel
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
  path: /card_disputes/{card_dispute_id}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /card_push_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /card_push_transfers/{card_push_transfer_id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /card_push_transfers/{card_push_transfer_id}/cancel
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
  path: /check_transfers/{check_transfer_id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check_transfers/{check_transfer_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fednow_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fednow_transfers/{fednow_transfer_id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fednow_transfers/{fednow_transfer_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inbound_ach_transfers/{inbound_ach_transfer_id}/create_notification_of_change
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inbound_ach_transfers/{inbound_ach_transfer_id}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inbound_ach_transfers/{inbound_ach_transfer_id}/transfer_return
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inbound_check_deposits/{inbound_check_deposit_id}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inbound_check_deposits/{inbound_check_deposit_id}/return
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inbound_wire_transfers/{inbound_wire_transfer_id}/reverse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /intrafi_account_enrollments
operation_count: 238
overview: 'Increase exposes 238 API operations that an AI agent could call, of which 132 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 106 read, 67 write, 64 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Increase
provider_slug: increase
slug: increase-agentic-access
source_filename: increase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/increase-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 238\n  by_action_class:\n    connected: 106\n    acting: 132\n  by_consequence:\n    read: 106\n    write: 67\n    physical: 64\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /account_numbers\n  method: get\n  operationId: list_account_numbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_numbers\n  method: post\n  operationId: create_an_account_number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_numbers/{account_number_id}\n  method: get\n  operationId: retrieve_an_account_number\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_numbers/{account_number_id}\n  method: patch\n  operationId: update_an_account_number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_statements\n  method: get\n  operationId: list_account_statements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /account_statements/{account_statement_id}\n  method: get\n  operationId: retrieve_an_account_statement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_transfers\n  method: get\n  operationId: list_account_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_transfers\n  method: post\n  operationId: create_an_account_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_transfers/{account_transfer_id}\n  method: get\n  operationId:\
  \ retrieve_an_account_transfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account_transfers/{account_transfer_id}/approve\n  method: post\n  operationId: approve_an_account_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_transfers/{account_transfer_id}/cancel\n  method: post\n  operationId: cancel_an_account_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: list_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: create_an_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}\n  method: get\n  operationId: retrieve_an_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}\n  method: patch\n  operationId: update_an_account\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/balance\n  method: get\n  operationId: retrieve_an_account_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/close\n  method: post\n  operationId: close_an_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/intrafi_balance\n  method: get\n  operationId: get_intrafi_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach_prenotifications\n  method: get\n  operationId: list_ach_prenotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach_prenotifications\n  method: post\n  operationId: create_an_ach_prenotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach_prenotifications/{ach_prenotification_id}\n  method: get\n  operationId: retrieve_an_ach_prenotification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach_transfers\n  method: get\n  operationId: list_ach_transfers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach_transfers\n  method: post\n  operationId: create_an_ach_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach_transfers/{ach_transfer_id}\n  method: get\n  operationId: retrieve_an_ach_transfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach_transfers/{ach_transfer_id}/approve\n  method: post\n  operationId: approve_an_ach_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach_transfers/{ach_transfer_id}/cancel\n  method: post\n  operationId: cancel_a_pending_ach_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card_disputes\n  method: get\n  operationId: list_card_disputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_disputes\n  method: post\n  operationId: create_a_card_dispute\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card_disputes/{card_dispute_id}\n  method: get\n  operationId: retrieve_a_card_dispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_disputes/{card_dispute_id}/submit_user_submission\n  method: post\n  operationId: submit_a_user_submission_for_a_card_dispute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card_disputes/{card_dispute_id}/withdraw\n  method: post\n  operationId: withdraw_a_card_dispute\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card_payments\n  method: get\n  operationId: list_card_payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_payments/{card_payment_id}\n  method: get\n  operationId: retrieve_a_card_payment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_purchase_supplements\n  method: get\n  operationId: list_card_purchase_supplements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /card_purchase_supplements/{card_purchase_supplement_id}\n  method: get\n  operationId: retrieve_a_card_purchase_supplement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_push_transfers\n  method: get\n  operationId: list_card_push_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_push_transfers\n  method: post\n  operationId: create_a_card_push_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card_push_transfers/{card_push_transfer_id}\n\
  \  method: get\n  operationId: retrieve_a_card_push_transfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_push_transfers/{card_push_transfer_id}/approve\n  method: post\n  operationId: approve_a_card_push_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card_push_transfers/{card_push_transfer_id}/cancel\n  method: post\n  operationId: cancel_a_pending_card_push_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card_tokens\n  method: get\n  operationId: list_card_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_tokens/{card_token_id}\n  method: get\n  operationId: retrieve_a_card_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_tokens/{card_token_id}/capabilities\n  method: get\n  operationId: retrieve_the_capabilities_of_a_card_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_validations\n  method: get\n  operationId: list_card_validations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card_validations\n  method: post\n  operationId: create_a_card_validation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card_validations/{card_validation_id}\n  method: get\n  operationId: retrieve_a_card_validation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards\n  method: get\n  operationId: list_cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards\n  method: post\n  operationId: create_a_card\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}\n  method: get\n  operationId: retrieve_a_card\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{card_id}\n  method: patch\n  operationId: update_a_card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/create_details_iframe\n  method: post\n  operationId: create_a_card_details_iframe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{card_id}/details\n  method: get\n  operationId: retrieve_sensitive_details_for_a_card\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{card_id}/update_pin\n  method: post\n  operationId: update_a_cards_pin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check_deposits\n  method: get\n  operationId: list_check_deposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /check_deposits\n  method: post\n  operationId: create_a_check_deposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check_deposits/{check_deposit_id}\n  method: get\n  operationId: retrieve_a_check_deposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_transfers\n  method: get\n  operationId: list_check_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_transfers\n  method: post\n  operationId: create_a_check_transfer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check_transfers/{check_transfer_id}\n  method: get\n  operationId: retrieve_a_check_transfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_transfers/{check_transfer_id}/approve\n  method: post\n  operationId: approve_a_check_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check_transfers/{check_transfer_id}/cancel\n\
  \  method: post\n  operationId: cancel_a_pending_check_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check_transfers/{check_transfer_id}/stop_payment\n  method: post\n  operationId: stop_payment_on_a_check_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /declined_transactions\n  method: get\n  operationId: list_declined_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /declined_transactions/{declined_transaction_id}\n  method: get\n  operationId: retrieve_a_declined_transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital_card_profiles\n  method: get\n  operationId: list_card_profiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital_card_profiles\n  method: post\n  operationId: create_a_digital_card_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital_card_profiles/{digital_card_profile_id}\n  method:\
  \ get\n  operationId: retrieve_a_digital_card_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital_card_profiles/{digital_card_profile_id}/archive\n  method: post\n  operationId: archive_a_digital_card_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital_card_profiles/{digital_card_profile_id}/clone\n  method: post\n  operationId: clones_a_digital_card_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /digital_wallet_tokens\n  method: get\n  operationId: list_digital_wallet_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital_wallet_tokens/{digital_wallet_token_id}\n  method: get\n  operationId: retrieve_a_digital_wallet_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities\n  method: get\n  operationId: list_entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities\n  method: post\n  operationId: create_an_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entities/{entity_id}\n  method: get\n  operationId: retrieve_an_entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/{entity_id}\n  method: patch\n  operationId: update_an_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entities/{entity_id}/archive\n  method: post\n  operationId: archive_an_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /entity_beneficial_owners\n  method: get\n  operationId: list_beneficial_owners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entity_beneficial_owners\n  method: post\n  operationId: create_a_beneficial_owner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entity_beneficial_owners/{entity_beneficial_owner_id}\n  method: get\n  operationId: retrieve_a_beneficial_owner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entity_beneficial_owners/{entity_beneficial_owner_id}\n  method: patch\n  operationId: update_a_beneficial_owner\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entity_beneficial_owners/{entity_beneficial_owner_id}/archive\n  method: post\n  operationId: archive_a_beneficial_owner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entity_onboarding_sessions\n  method: get\n  operationId: list_entity_onboarding_session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entity_onboarding_sessions\n  method: post\n  operationId: create_an_entity_onboarding_session\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entity_onboarding_sessions/{entity_onboarding_session_id}\n  method: get\n  operationId: retrieve_an_entity_onboarding_session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entity_onboarding_sessions/{entity_onboarding_session_id}/expire\n  method: post\n  operationId: expire_an_entity_onboarding_session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entity_supplemental_documents\n\
  \  method: get\n  operationId: list_entity_supplemental_document_submissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entity_supplemental_documents\n  method: post\n  operationId: create_a_supplemental_document_for_an_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event_subscriptions\n  method: get\n  operationId: list_event_subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_subscriptions\n  method: post\n  operationId: create_an_event_subscription\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event_subscriptions/{event_subscription_id}\n  method: get\n  operationId: retrieve_an_event_subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_subscriptions/{event_subscription_id}\n  method: patch\n  operationId: update_an_event_subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: list_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}\n  method: get\n  operationId: retrieve_an_event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exports\n  method: get\n  operationId: list_exports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exports\n  method: post\n  operationId: create_an_export\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exports/{export_id}\n  method: get\n  operationId: retrieve_an_export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external_accounts\n  method: get\n  operationId: list_external_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external_accounts\n  method: post\n  operationId: create_an_external_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external_accounts/{external_account_id}\n  method: get\n  operationId: retrieve_an_external_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external_accounts/{external_account_id}\n  method: patch\n  operationId:\
  \ update_an_external_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fednow_transfers\n  method: get\n  operationId: list_fednow_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fednow_transfers\n  method: post\n  operationId: create_a_fednow_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fednow_transfers/{fednow_transfer_id}\n  method:\
  \ get\n  operationId: retrieve_a_fednow_transfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fednow_transfers/{fednow_transfer_id}/approve\n  method: post\n  operationId: approve_a_fednow_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fednow_transfers/{fednow_transfer_id}/cancel\n  method: post\n  operationId: cancel_a_pending_fednow_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file_links\n  method: post\n  operationId: create_a_file_link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: get\n  operationId: list_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: create_a_file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- p\n\n# --- truncated\
  \ at 32 KB (76 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/agentic-access/increase-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/agentic-access/increase-agentic-access.yml
summary_line: 238 operations · 132 acting · 1 human-in-the-loop
tags:
- Fintech
- Banking
- Payments
- ACH
- Wires
---
