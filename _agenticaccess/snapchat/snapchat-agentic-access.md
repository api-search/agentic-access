---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: snapchat-conversion-events-api-openapi.yml
  format: yaml
  label: Snapchat Conversion Events API
  slug: snapchat-conversion-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-conversion-events-api-openapi.yml
- filename: snapchat-user-profile-api-openapi.yml
  format: yaml
  label: Snapchat User Profile API
  slug: snapchat-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-user-profile-api-openapi.yml
- filename: snapchat-oauth-api-openapi.yml
  format: yaml
  label: Snapchat O Auth API
  slug: snapchat-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-oauth-api-openapi.yml
consequence_counts:
  physical: 2
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Snapchat Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{pixel_id}/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{snap_app_id}/events
operation_count: 5
overview: 'Snapchat exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 1 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Snapchat
provider_slug: snapchat
slug: snapchat-agentic-access
source_filename: snapchat-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/snapchat-conversion-events-api-openapi.yml, openapi/snapchat-oauth-api-openapi.yml,\n  openapi/snapchat-user-profile-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    physical: 2\n    read: 2\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /{pixel_id}/events\n  method: post\n  operationId: sendWebConversionEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{snap_app_id}/events\n  method: post\n  operationId: sendAppConversionEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/oauth2/auth\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login/oauth2/access_token\n  method: post\n  operationId: exchangeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId: getUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/agentic-access/snapchat-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Advertising
- AR
- Augmented Reality
- Marketing
- Messaging
- Social-Media
---
