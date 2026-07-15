---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 5
api_specs:
- filename: sift-events-api-openapi.yml
  format: yaml
  label: Sift Events API
  slug: sift-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-events-api-openapi.yml
- filename: sift-decisions-api-openapi.yml
  format: yaml
  label: Sift Decisions API
  slug: sift-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-decisions-api-openapi.yml
- filename: sift-score-api-openapi.yml
  format: yaml
  label: Sift Score API
  slug: sift-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-score-api-openapi.yml
- filename: sift-verification-api-openapi.yml
  format: yaml
  label: Sift Verification API
  slug: sift-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-verification-api-openapi.yml
- filename: sift-workflows-api-openapi.yml
  format: yaml
  label: Sift Workflows API
  slug: sift-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-workflows-api-openapi.yml
- filename: sift-labels-api-openapi.yml
  format: yaml
  label: Sift Labels API
  slug: sift-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/openapi/sift-labels-api-openapi.yml
consequence_counts:
  physical: 4
  read: 5
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sift Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{account_id}/users/{user_id}/orders/{order_id}/decisions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verification/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verification/send
operation_count: 16
overview: 'Sift exposes 16 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 7 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sift
provider_slug: sift-com
slug: sift-com-agentic-access
source_filename: sift-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sift-decisions-api-openapi.yml, openapi/sift-events-api-openapi.yml, openapi/sift-labels-api-openapi.yml,\n  openapi/sift-score-api-openapi.yml, openapi/sift-verification-api-openapi.yml, openapi/sift-workflows-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 11\n    connected: 5\n  by_consequence:\n    write: 7\n    read: 5\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/{account_id}/users/{user_id}/decisions\n  method: post\n  operationId: applyUserDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/users/{user_id}/decisions\n  method: get\n  operationId: getUserDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/users/{user_id}/orders/{order_id}/decisions\n  method: post\n  operationId: applyOrderDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/users/{user_id}/sessions/{session_id}/decisions\n  method: post\n  operationId: applySessionDecision\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/users/{user_id}/content/{content_id}/decisions\n  method: post\n  operationId: applyContentDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/decisions\n  method: get\n  operationId: listDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: post\n  operationId: sendEvent\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}/labels\n  method: post\n  operationId: applyLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}/labels\n  method: delete\n  operationId: removeLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /score/{user_id}\n  method: get\n  operationId: getScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rescore/{user_id}\n  method: post\n  operationId: rescoreUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verification/send\n  method: post\n  operationId: sendVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verification/resend\n  method:\
  \ post\n  operationId: resendVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verification/check\n  method: post\n  operationId: checkVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/workflows/runs/{run_id}\n  method: get\n  operationId: getWorkflowRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/users/{user_id}/workflows\n\
  \  method: get\n  operationId: listUserWorkflowRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sift-com/refs/heads/main/agentic-access/sift-com-agentic-access.yml
summary_line: 16 operations · 11 acting
tags:
- Fraud Prevention
- Trust And Safety
- Risk Scoring
- Identity Verification
- Chargebacks
- Account Takeover
- Content Abuse
---
