---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 7
api_specs:
- filename: sift-openapi.yml
  format: yaml
  label: Sift Events API
  slug: sift-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Score API
  slug: sift-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Decisions API
  slug: sift-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Workflow Status API
  slug: sift-workflow-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Labels API
  slug: sift-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Verification API
  slug: sift-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift PSP Merchant Management API
  slug: sift-psp-merchant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
consequence_counts:
  physical: 4
  read: 7
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sift Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/verification/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/verification/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v205/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/accounts/{account_id}/users/{user_id}/orders/{order_id}/decisions
operation_count: 20
overview: 'Sift exposes 20 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 9 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sift
provider_slug: sift
slug: sift-agentic-access
source_filename: sift-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sift-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 13\n    connected: 7\n  by_consequence:\n    physical: 4\n    read: 7\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v205/events\n  method: post\n  operationId: postEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v205/score/{user_id}\n  method: get\n  operationId: getScore\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v205/users/{user_id}/score\n  method: get\n  operationId: getUserScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v205/users/{user_id}/score\n  method: post\n  operationId: rescoreUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v205/users/{user_id}/labels\n  method: post\n  operationId: applyLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v205/users/{user_id}/labels\n  method: delete\n  operationId: removeLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/accounts/{account_id}/decisions\n  method: get\n  operationId: listDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/{account_id}/users/{user_id}/decisions\n  method: get\n  operationId: getUserDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/{account_id}/users/{user_id}/decisions\n\
  \  method: post\n  operationId: applyUserDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/accounts/{account_id}/users/{user_id}/orders/{order_id}/decisions\n  method: post\n  operationId: applyOrderDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/accounts/{account_id}/users/{user_id}/sessions/{session_id}/decisions\n  method: post\n  operationId: applySessionDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/accounts/{account_id}/users/{user_id}/content/{content_id}/decisions\n  method: post\n  operationId: applyContentDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/accounts/{account_id}/workflows/runs/{run_id}\n  method: get\n  operationId: getWorkflowRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/{account_id}/psp_management/merchants\n  method: get\n  operationId: listPspMerchants\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/{account_id}/psp_management/merchants\n  method: post\n  operationId: createPspMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/accounts/{account_id}/psp_management/merchants/{merchant_id}\n  method: get\n  operationId: getPspMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/accounts/{account_id}/psp_management/merchants/{merchant_id}\n  method: put\n  operationId: updatePspMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verification/send\n  method: post\n  operationId: verificationSend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verification/resend\n  method: post\n  operationId: verificationResend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/verification/check\n  method: post\n  operationId: verificationCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/agentic-access/sift-agentic-access.yml
summary_line: 20 operations · 13 acting
tags:
- Fraud Detection
- Fraud Prevention
- Risk
- Trust and Safety
- Machine Learning
- Payment Fraud
- Account Takeover
- Chargebacks
- Digital Trust
---
