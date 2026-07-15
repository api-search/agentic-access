---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 3
api_specs:
- filename: passage-1password-openapi.yml
  format: yaml
  label: Passage Management API
  slug: passage-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-openapi.yml
- filename: passage-1password-openapi.yml
  format: yaml
  label: Passage Users API
  slug: passage-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-openapi.yml
- filename: passage-1password-openapi.yml
  format: yaml
  label: Passage Magic Links API
  slug: passage-magic-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-openapi.yml
- filename: passage-1password-openapi.yml
  format: yaml
  label: Passage Authentication API
  slug: passage-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/openapi/passage-1password-openapi.yml
consequence_counts:
  read: 3
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Passage 1Password Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /apps/{app_id}/users/{user_id}/tokens
operation_count: 11
overview: 'Passage by 1Password exposes 11 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 7 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Passage by 1Password
provider_slug: passage-1password
slug: passage-1password-agentic-access
source_filename: passage-1password-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/passage-1password-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 3\n    acting: 8\n  by_consequence:\n    read: 3\n    write: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /apps/{app_id}/users\n  method: get\n  operationId: listPaginatedUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id}/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/users/{user_id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id}/users/{user_id}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/users/{user_id}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/users/{user_id}/activate\n  method: patch\n  operationId: activateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/users/{user_id}/deactivate\n  method: patch\n  operationId: deactivateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/users/{user_id}/devices\n  method: get\n  operationId: listUserDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id}/users/{user_id}/devices/{device_id}\n  method: delete\n  operationId: deleteUserDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/users/{user_id}/tokens\n  method: delete\n  operationId: revokeUserRefreshTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /apps/{app_id}/magic-links\n  method: post\n  operationId: createMagicLink\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passage-1password/refs/heads/main/agentic-access/passage-1password-agentic-access.yml
summary_line: 11 operations · 8 acting · 1 human-in-the-loop
tags:
- Authentication
- Passkeys
- WebAuthn
- Passwordless
- Identity
- Magic Links
---
