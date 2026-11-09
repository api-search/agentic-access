---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 2
api_specs:
- filename: iproov-enrol-api-openapi.yml
  format: yaml
  label: iProov Enrol API
  slug: iproov-enrol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-enrol-api-openapi.yml
- filename: iproov-management-api-openapi.yml
  format: yaml
  label: iProov Management API
  slug: iproov-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-management-api-openapi.yml
- filename: iproov-user-api-openapi.yml
  format: yaml
  label: iProov User API
  slug: iproov-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-user-api-openapi.yml
- filename: iproov-verify-api-openapi.yml
  format: yaml
  label: iProov Verify API
  slug: iproov-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-verify-api-openapi.yml
consequence_counts:
  read: 2
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Iproov Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'iProov exposes 12 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: iProov
provider_slug: iproov
slug: iproov-agentic-access
source_filename: iproov-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/iproov-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 2\n    acting: 10\n  by_consequence:\n    read: 2\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /availability\n  method: get\n  operationId: platformAvailable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claim/{token}/invalidate\n  method: post\n  operationId: invalidateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/verify/token\n  method: post\n  operationId: userVerifyServerToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/verify/validate\n  method: post\n  operationId: userVerifyValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{api_key}/access_token\n  method: post\n  operationId: generateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/enrol/token\n  method: post\n  operationId: userEnrolServerToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/enrol/image\n  method: post\n  operationId: userEnrolImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/verify/image\n  method: post\n  operationId: userVerifyImage\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/enrol/validate\n  method: post\n  operationId: userEnrolValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{existing_user_id}\n  method: get\n  operationId: userGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{existing_user_id}\n  method: put\n  operationId: userUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - user-write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{existing_user_id}\n  method: delete\n  operationId: userDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user-write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/iproov/agentic-access/iproov-agentic-access.yml
summary_line: 12 operations · 10 acting
tags:
- Company
- Biometrics
- Identity Verification
- Authentication
- Liveness Detection
- Face Verification
- Fraud Prevention
- Deepfake Detection
---
