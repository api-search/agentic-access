---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 6
api_specs:
- filename: tenpace-com-review-router-setup-api-openapi.yml
  format: yaml
  label: tenpace-com Review Router setup API
  slug: tenpace-com-review-router-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenpace-com/openapi/tenpace-com-review-router-setup-api-openapi.yml
consequence_counts:
  physical: 3
  read: 6
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tenpace Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/review-router/setup-sessions/{setupId}/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/review-router/setup-sessions/{setupId}/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/review-router/setup-sessions/{setupId}/test
operation_count: 30
overview: 'tenpace-com exposes 30 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 21 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tenpace-com
provider_slug: tenpace-com
slug: tenpace-com-agentic-access
source_filename: tenpace-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/api-tenpace-com-openapi.json, openapi/review-router-tenpace-com-openapi.json,\n  openapi/tenpace-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 24\n    connected: 6\n  by_consequence:\n    write: 21\n    read: 6\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/review-router/setup-sessions\n  method: post\n  operationId: createReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}\n  method: get\n  operationId: getReviewRouterSetupSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/review-router/setup-sessions/{setupId}\n  method: delete\n  operationId: cancelReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/intent\n  method: put\n  operationId: updateReviewRouterSetupIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/plan\n  method: get\n  operationId: previewReviewRouterSetupSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/review-router/setup-sessions/{setupId}/claim\n  method: post\n  operationId: claimReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/apply\n  method: post\n  operationId: applyReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/test\n  method: post\n  operationId: testReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/connections/github\n  method: post\n  operationId: createReviewRouterGitHubConnectionUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/review-router/setup-sessions/{setupId}/connections/slack\n  method: post\n  operationId: createReviewRouterSlackConnectionUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions\n  method: post\n  operationId: createReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}\n  method: get\n  operationId: getReviewRouterSetupSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/review-router/setup-sessions/{setupId}\n  method: delete\n  operationId: cancelReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/intent\n  method: put\n  operationId: updateReviewRouterSetupIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/plan\n  method: get\n  operationId: previewReviewRouterSetupSession\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/review-router/setup-sessions/{setupId}/claim\n  method: post\n  operationId: claimReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/apply\n  method: post\n  operationId: applyReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/test\n  method: post\n  operationId: testReviewRouterSetupSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/connections/github\n  method: post\n  operationId: createReviewRouterGitHubConnectionUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/connections/slack\n  method: post\n  operationId: createReviewRouterSlackConnectionUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions\n  method: post\n  operationId: createReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}\n  method: get\n  operationId: getReviewRouterSetupSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/review-router/setup-sessions/{setupId}\n  method: delete\n  operationId: cancelReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/intent\n  method: put\n  operationId: updateReviewRouterSetupIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/plan\n  method: get\n  operationId: previewReviewRouterSetupSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/review-router/setup-sessions/{setupId}/claim\n  method: post\n  operationId: claimReviewRouterSetupSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/apply\n  method: post\n  operationId: applyReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/test\n  method: post\n  operationId: testReviewRouterSetupSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/connections/github\n  method: post\n  operationId: createReviewRouterGitHubConnectionUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/review-router/setup-sessions/{setupId}/connections/slack\n  method: post\n  operationId: createReviewRouterSlackConnectionUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/tenpace-com/agentic-access/tenpace-com-agentic-access.yml
summary_line: 30 operations · 24 acting
tags:
- Health
- Software-as-a-Service
- Productivity
- Workflows
- Integration
- Company
---
