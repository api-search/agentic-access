---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: n0t1fy-dev-health-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Health API
  slug: n0t1fy-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-health-api-openapi.yml
- filename: n0t1fy-dev-keys-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Keys API
  slug: n0t1fy-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-keys-api-openapi.yml
- filename: n0t1fy-dev-messages-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Messages API
  slug: n0t1fy-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-messages-api-openapi.yml
- filename: n0t1fy-dev-verifications-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Verifications API
  slug: n0t1fy-dev-verifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-verifications-api-openapi.yml
consequence_counts:
  physical: 4
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: N0T1Fy Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/verifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/verifications
operation_count: 14
overview: 'n0t1fy-dev exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 2 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: n0t1fy-dev
provider_slug: n0t1fy-dev
slug: n0t1fy-dev-agentic-access
source_filename: n0t1fy-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/n0t1fy-dev-api-openapi.json, openapi/n0t1fy-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    physical: 4\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  operationId: healthz_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /readyz\n  method: get\n  operationId: readyz_readyz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/messages\n  method: post\n  operationId: create_message_route_v1_messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{message_id}\n  method: get\n  operationId: get_message_route_v1_messages__message_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verifications\n  method: post\n  operationId: start_verification_route_v1_verifications_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verifications/{verification_id}/check\n  method: post\n  operationId: check_verification_route_v1_verifications__verification_id__check_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/test-keys\n  method: post\n  operationId: create_test_key_v1_test_keys_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: healthz_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /readyz\n  method: get\n  operationId: readyz_readyz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages\n  method: post\n  operationId: create_message_route_v1_messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{message_id}\n  method: get\n  operationId: get_message_route_v1_messages__message_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verifications\n  method: post\n  operationId: start_verification_route_v1_verifications_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verifications/{verification_id}/check\n  method: post\n  operationId: check_verification_route_v1_verifications__verification_id__check_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/test-keys\n  method: post\n  operationId: create_test_key_v1_test_keys_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/n0t1fy-dev/agentic-access/n0t1fy-dev-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Company
- SMS
- Georgia
- Transactional
- Developer-First
---
