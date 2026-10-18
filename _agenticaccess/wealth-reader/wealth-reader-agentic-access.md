---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 8
api_specs:
- filename: wealth-reader-advanced-api-openapi.yml
  format: yaml
  label: Wealth Reader Advanced API
  slug: wealth-reader-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-reader/refs/heads/main/openapi/wealth-reader-advanced-api-openapi.yml
- filename: wealth-reader-cards-real-time-api-openapi.yml
  format: yaml
  label: Wealth Reader Cards (real time) API
  slug: wealth-reader-cards-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-reader/refs/heads/main/openapi/wealth-reader-cards-real-time-api-openapi.yml
- filename: wealth-reader-core-api-openapi.yml
  format: yaml
  label: Wealth Reader Core API
  slug: wealth-reader-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-reader/refs/heads/main/openapi/wealth-reader-core-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  safety-critical: 2
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Wealth Reader Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tokens/revoke/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/revoke/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify/iban-ownership/
operation_count: 20
overview: 'Wealth Reader exposes 20 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 9 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wealth Reader
provider_slug: wealth-reader
slug: wealth-reader-agentic-access
source_filename: wealth-reader-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/wealth-reader-advanced-api-openapi.yml, openapi/wealth-reader-cards-real-time-api-openapi.yml,\n  openapi/wealth-reader-core-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 8\n    acting: 12\n  by_consequence:\n    read: 8\n    physical: 1\n    write: 9\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /entities/\n  method: get\n  operationId: getEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/iban-ownership/\n  method: post\n  operationId: postVerifyIbanOwnership\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/register/\n  method: post\n  operationId: registerUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/check/\n  method: post\n  operationId: checkUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /user/revoke/\n  method: post\n  operationId: revokeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /batch/load/\n  method: post\n  operationId: postBatchLoad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/fetch/statistics/\n  method: post\n  operationId: postBatchFetchStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/fetch/connection-result/\n\
  \  method: post\n  operationId: postBatchFetchConnectionResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/webhook/\n  method: post\n  operationId: cardsWebhookRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/enrollments/\n  method: post\n  operationId: cardsEnrollmentsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/enrollments/\n  method: get\n  operationId: cardsEnrollmentsStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/transactions/\n  method: get\n  operationId: cardsTransactionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/\n  method: post\n  operationId: postEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entities/category-types/\n  method: get\n  operationId: getEntitiesCategoryTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/\n  method: post\n  operationId:\
  \ queryTokensByApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/revoke/\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tokens/reasign/\n  method: post\n  operationId: reasignToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /domains/\n  method: post\n  operationId: addDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /error-codes/\n  method: get\n  operationId: getErrorCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /warning-codes/\n  method: get\n  operationId: getWarningCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealth-reader/refs/heads/main/agentic-access/wealth-reader-agentic-access.yml
summary_line: 20 operations · 12 acting · 2 human-in-the-loop
tags:
- Bank Aggregation
- Open Banking
- PSD2
- Financial Data
- Account Aggregation
- Investment Portfolios
- Wealth Management
- Banking
- Fintech
- Data Aggregation
---
