---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 6
api_specs:
- filename: disban-io-auth-api-openapi.yml
  format: yaml
  label: disban-io Auth API
  slug: disban-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-auth-api-openapi.yml
- filename: disban-io-batch-api-openapi.yml
  format: yaml
  label: disban-io Batch API
  slug: disban-io-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-batch-api-openapi.yml
- filename: disban-io-check-api-openapi.yml
  format: yaml
  label: disban-io Check API
  slug: disban-io-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-check-api-openapi.yml
- filename: disban-io-features-api-openapi.yml
  format: yaml
  label: disban-io Features API
  slug: disban-io-features-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-features-api-openapi.yml
- filename: disban-io-keys-api-openapi.yml
  format: yaml
  label: disban-io Keys API
  slug: disban-io-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-keys-api-openapi.yml
- filename: disban-io-plans-api-openapi.yml
  format: yaml
  label: disban-io Plans API
  slug: disban-io-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-plans-api-openapi.yml
- filename: disban-io-referrals-api-openapi.yml
  format: yaml
  label: disban-io Referrals API
  slug: disban-io-referrals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-referrals-api-openapi.yml
- filename: disban-io-subscription-api-openapi.yml
  format: yaml
  label: disban-io Subscription API
  slug: disban-io-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-subscription-api-openapi.yml
- filename: disban-io-webhooks-api-openapi.yml
  format: yaml
  label: disban-io Webhooks API
  slug: disban-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-webhooks-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Disban Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/account/{action}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/keys/{id}
operation_count: 16
overview: 'disban-io exposes 16 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 8 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: disban-io
provider_slug: disban-io
slug: disban-io-agentic-access
source_filename: disban-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/disban-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 6\n    acting: 10\n  by_consequence:\n    read: 6\n    safety-critical: 2\n    write: 8\n  human_in_the_loop_required: 2\noperations:\n- path: /api/features\n  method: get\n  operationId: getAccountFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/account/sessions\n  method: get\n  operationId: countAccountSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/auth/account/{action}\n  method: post\n  operationId: manageAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/otp/request\n  method: post\n  operationId: requestEmailCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/otp/verify\n \
  \ method: post\n  operationId: verifyEmailCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys/{id}\n  method: delete\n  operationId: revokeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/referrals\n  method: get\n  operationId: getReferrals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/subscription\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/subscription\n  method: post\n  operationId: changePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/check\n  method: post\n  operationId: checkDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/check\n  method: post\n  operationId: receiveChecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/batch\n  method: post\n  operationId: checkBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/disban-io/agentic-access/disban-io-agentic-access.yml
summary_line: 16 operations · 10 acting · 2 human-in-the-loop
tags:
- Company
- Email
- Disposable Email
- Security
- Fraud Prevention
---
