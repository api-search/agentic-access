---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 14
api_specs:
- filename: uetr-ai-account-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Account API
  slug: uetr-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-account-api-openapi.yml
- filename: uetr-ai-owner-confirmation-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Owner confirmation API
  slug: uetr-ai-owner-confirmation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-owner-confirmation-api-openapi.yml
- filename: uetr-ai-payment-records-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Payment records API
  slug: uetr-ai-payment-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-payment-records-api-openapi.yml
- filename: uetr-ai-team-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Team API
  slug: uetr-ai-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-team-api-openapi.yml
- filename: uetr-ai-transfers-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Transfers API
  slug: uetr-ai-transfers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-transfers-api-openapi.yml
- filename: uetr-ai-webhooks-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Webhooks API
  slug: uetr-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-webhooks-api-openapi.yml
consequence_counts:
  physical: 11
  read: 14
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uetr Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /team/members/{member_id}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /transfers/{uetr}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers/{uetr}/archive
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /transfers/{uetr}/check-frequency
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /transfers/{uetr}/details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /transfers/{uetr}/label
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers/{uetr}/recheck
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers/{uetr}/record-share
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers/{uetr}/restore
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/{id}/test
operation_count: 33
overview: 'SWIFT UETR Tracker exposes 33 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 8 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SWIFT UETR Tracker
provider_slug: uetr-ai
slug: uetr-ai-agentic-access
source_filename: uetr-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 14\n    acting: 19\n  by_consequence:\n    read: 14\n    write: 8\n    physical: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /account\n  method: get\n  operationId: get_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/billing-link\n  method: get\n  operationId: get_billing_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/usage\n  method:\
  \ get\n  operationId: get_plan_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export\n  method: get\n  operationId: export_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pending-access\n  method: get\n  operationId: list_pending_access\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records/{record_token}\n  method: get\n  operationId: get_payment_record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team\n  method: get\n  operationId: list_team_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/invitations/decline\n  method: post\n  operationId: decline_team_invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/members\n  method: post\n  operationId: invite_team_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/members/{member_id}\n  method: delete\n  operationId: remove_team_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/members/{member_id}/resend\n  method: post\n  operationId: resend_team_invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers\n  method: get\n  operationId: list_transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers\n  method: post\n  operationId: add_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{uetr}\n  method: delete\n  operationId: delete_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{uetr}\n  method: get\n  operationId: get_transfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/{uetr}/archive\n  method: post\n  operationId: archive_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{uetr}/check-frequency\n  method: patch\n  operationId: set_check_frequency\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{uetr}/details\n  method: patch\n  operationId: update_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{uetr}/label\n  method: patch\n  operationId: rename_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{uetr}/recheck\n  method: post\n  operationId: recheck_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{uetr}/record-share\n  method: post\n  operationId: share_payment_record\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{uetr}/restore\n  method: post\n  operationId: restore_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{uetr}/share-link\n  method: get\n  operationId: get_share_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/{uetr}/watchers\n  method:\
  \ get\n  operationId: get_watcher_count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: list_webhook_endpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: create_webhook_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: delete_webhook_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  operationId: get_webhook_endpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: patch\n  operationId: update_webhook_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/deliveries\n  method: get\n  operationId: list_webhook_deliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}/rotate-secret\n  method: post\n  operationId:\
  \ rotate_webhook_secret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/test\n  method: post\n  operationId: send_webhook_test\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/url\n  method: patch\n  operationId: change_webhook_endpoint_url\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/uetr-ai/agentic-access/uetr-ai-agentic-access.yml
summary_line: 33 operations · 19 acting
tags:
- Payments
- SWIFT
- Tracking
- Financial Services
---
