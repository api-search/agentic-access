---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 21
api_specs:
- filename: darwin-so-account-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Account API
  slug: darwin-so-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-account-api-openapi.yml
- filename: darwin-so-accounts-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Accounts API
  slug: darwin-so-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-accounts-api-openapi.yml
- filename: darwin-so-act-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Act API
  slug: darwin-so-act-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-act-api-openapi.yml
- filename: darwin-so-search-api-openapi.yml
  format: yaml
  label: Darwin Technologies, Inc. Search API
  slug: darwin-so-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/darwin-so/openapi/darwin-so-search-api-openapi.yml
consequence_counts:
  physical: 4
  read: 21
  safety-critical: 5
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Darwin So Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/ais/{aiId}/connections/auth-credentials/{credentialId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/ais/{aiId}/connections/targets/{targetAiId}/{connectionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/ais/{aiId}/payment-methods/{methodId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/auth-credentials/{credentialId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/payment-methods/{methodId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/ais/{aiId}/payment-methods/{methodId}/default
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/payment-method-setups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /act/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /act/threads/{thread}/messages
operation_count: 40
overview: 'Darwin Technologies, Inc. exposes 40 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 10 write, 4 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Darwin Technologies, Inc.
provider_slug: darwin-so
slug: darwin-so-agentic-access
source_filename: darwin-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/darwin-so-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 21\n    acting: 19\n  by_consequence:\n    read: 21\n    write: 10\n    physical: 4\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: create_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account\n  method: get\n  operationId: get_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/applications\n  method: post\n  operationId: create_application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/applications/{applicationId}\n  method: get\n  operationId: get_application\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/api-keys\n  method: post\n  operationId: create_api_key\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/api-keys\n  method: get\n  operationId: list_api_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/api-keys/usage\n  method: get\n  operationId: get_api_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/api-keys/{apiKeyId}\n  method: delete\n  operationId: delete_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /account/searches\n  method: get\n  operationId: list_search_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/observability/spend\n  method: get\n  operationId: get_account_spend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/observability/usage\n  method: get\n  operationId: get_account_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/memory\n  method: get\n  operationId: get_account_memory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/memory\n  method:\
  \ put\n  operationId: replace_account_memory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act/threads\n  method: post\n  operationId: start_thread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act/threads\n  method: get\n  operationId: list_threads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act/threads/{thread}/messages\n  method: post\n  operationId: send_message\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act/threads/{thread}\n  method: get\n  operationId: get_thread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act/threads/{thread}/archive\n  method: post\n  operationId: archive_thread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act/authentications\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act/payments\n  method: post\n  operationId: pay\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act/threads/{thread}/result-artifacts/{ticket}/download-url\n  method: post\n  operationId: get_result_artifact_download_url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act/payment-requests/{paymentRequestId}/options\n  method: get\n  operationId: get_payment_options\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act/payments/{paymentId}\n  method: get\n  operationId: get_payment_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/auth-credential-setups\n  method: post\n  operationId: start_account_auth_credential_setup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/auth-credential-setups/{setupId}\n  method: get\n  operationId: get_account_auth_credential_setup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /account/payment-method-setups\n  method: post\n  operationId: start_account_payment_method_setup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/payment-method-setups/{setupId}\n  method: get\n  operationId: get_account_payment_method_setup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/auth-credentials\n  method: get\n  operationId: list_account_auth_credentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/auth-credentials/{credentialId}\n\
  \  method: delete\n  operationId: revoke_account_auth_credential\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/payment-methods\n  method: get\n  operationId: list_account_payment_methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/payment-methods/{methodId}\n  method: delete\n  operationId: revoke_account_payment_method\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /account/ais/{aiId}/connections/auth-credentials\n  method: get\n  operationId: list_auth_credentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/ais/{aiId}/connections/auth-credentials/{credentialId}\n  method: delete\n  operationId: revoke_auth_credential\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/ais/{aiId}/payment-methods/{methodId}/default\n  method: post\n  operationId: set_payment_method_default\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/ais/{aiId}/payment-methods/{methodId}\n  method: delete\n  operationId: revoke_payment_method\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/ais/{aiId}/payment-methods\n  method: get\n  operationId: list_payment_methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/ais/{aiId}/connections/targets/{targetAiId}\n  method: get\n  operationId: list_target_accounts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/ais/{aiId}/connections/targets/{targetAiId}/{connectionId}/default\n  method: post\n  operationId: set_target_account_default\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/ais/{aiId}/connections/targets/{targetAiId}/{connectionId}\n  method: delete\n  operationId: revoke_target_account\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/darwin-so/agentic-access/darwin-so-agentic-access.yml
summary_line: 40 operations · 19 acting · 5 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Platform
- Developer Tools
- Marketplace
- Productivity
---
