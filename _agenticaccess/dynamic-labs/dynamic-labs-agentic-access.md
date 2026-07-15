---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 11
api_specs:
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Users API
  slug: dynamic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Wallets API
  slug: dynamic-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Embedded Wallets API
  slug: dynamic-embedded-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Environments API
  slug: dynamic-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic API Tokens API
  slug: dynamic-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Webhooks API
  slug: dynamic-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Token Verification API
  slug: dynamic-token-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Allowlists API
  slug: dynamic-allowlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
- filename: dynamic-labs-openapi.yml
  format: yaml
  label: Dynamic Analytics API
  slug: dynamic-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/openapi/dynamic-labs-openapi.yml
consequence_counts:
  read: 11
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dynamic Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Dynamic exposes 22 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dynamic
provider_slug: dynamic-labs
slug: dynamic-labs-agentic-access
source_filename: dynamic-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dynamic-labs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 11\n    acting: 11\n  by_consequence:\n    read: 11\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /environments/{environmentId}\n  method: get\n  operationId: getEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}\n  method: patch\n  operationId: updateEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/users/{userId}\n  method: get\n  operationId: getUserById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/users/{userId}\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/users/{userId}\n\
  \  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/users/{userId}/wallets\n  method: get\n  operationId: getWalletsByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/users/{userId}/wallets\n  method: post\n  operationId: createEmbeddedWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/tokens\n\
  \  method: get\n  operationId: getApiTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/tokens\n  method: post\n  operationId: createApiToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/tokens/{tokenId}\n  method: delete\n  operationId: deleteApiToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/webhooks\n  method:\
  \ get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/webhooks/{webhookId}\n  method: get\n  operationId: getWebhookById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/webhooks/{webhookId}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/allowlists\n  method: get\n  operationId: getAllowlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/allowlists\n  method: post\n  operationId: createAllowlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/allowlists/{allowlistId}/entries\n  method: post\n  operationId: createAllowlistEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/analytics/wallets\n  method: get\n  operationId: getAnalyticsWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/exports/{exportId}\n  method: get\n  operationId: downloadExport\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sdk/{environmentId}/.well-known/jwks.json\n  method: get\n  operationId: getJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-labs/refs/heads/main/agentic-access/dynamic-labs-agentic-access.yml
summary_line: 22 operations · 11 acting
tags:
- Web3
- Authentication
- Embedded Wallets
- Wallets
- MPC
- Onboarding
- Crypto
---
