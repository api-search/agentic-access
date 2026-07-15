---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 13
api_specs:
- filename: zapier-partner-api.yml
  format: yaml
  label: Zapier Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/openapi/zapier-partner-api.yml
consequence_counts:
  read: 13
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zapier Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Zapier exposes 21 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zapier
provider_slug: zapier
slug: zapier-agentic-access
source_filename: zapier-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zapier-partner-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 13\n    acting: 8\n  by_consequence:\n    read: 13\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/apps\n  method: get\n  operationId: v1_apps_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories\n  method: get\n  operationId: v1_categories_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/me\n  method: get\n\
  \  operationId: v1_profiles_me_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - profile\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/zap-templates\n  method: get\n  operationId: v1_zap_templates_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/zaps\n  method: get\n  operationId: v1_zaps_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - zap\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/action-runs\n  method: post\n  operationId: create-action-run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - action:run\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/action-runs/{id}\n  method: get\n  operationId: retrieve-action-run\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - action:run\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/actions\n  method: get\n  operationId: get-actions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - zap\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/actions/{action_id}/inputs\n  method: post\n  operationId: get-fields-inputs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - zap:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/actions/{action_id}/inputs/{input_id}/choices\n  method: post\n\
  \  operationId: get-choices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - zap\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/actions/{action_id}/outputs\n  method: post\n  operationId: get-fields-outputs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - zap:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/actions/{action_id}/test\n  method: post\n  operationId: test-action\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - zap:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apps\n  method: get\n  operationId: get-v2-apps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - zap\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/authentications\n  method: get\n  operationId: get-authentications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - connection:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/authentications\n  method: post\n  operationId: create-authentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connection:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/authorize\n  method: get\n  operationId: v2_authorize_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/guess\n  method: post\n  operationId: create-zap-guess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/whitelabel/apps\n  method: get\n  operationId: v2-whitelabel-apps-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/zap-runs\n  method: get\n  operationId: get-zap-runs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - zap:runs\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v2/zaps\n  method: get\n  operationId: get-v2-zaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - zap\n    - zap:all\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/zaps\n  method: post\n  operationId: post-zaps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - zap:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zapier/refs/heads/main/agentic-access/zapier-agentic-access.yml
summary_line: 21 operations · 8 acting
tags:
- Integrations
- iPaaS
---
