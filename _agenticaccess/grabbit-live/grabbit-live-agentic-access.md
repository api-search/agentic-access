---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: grabbit-live-account-api-openapi.yml
  format: yaml
  label: grabbit-live Account API
  slug: grabbit-live-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabbit-live/openapi/grabbit-live-account-api-openapi.yml
- filename: grabbit-live-grabs-api-openapi.yml
  format: yaml
  label: grabbit-live Grabs API
  slug: grabbit-live-grabs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabbit-live/openapi/grabbit-live-grabs-api-openapi.yml
consequence_counts:
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Grabbit Live Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'grabbit-live exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: grabbit-live
provider_slug: grabbit-live
slug: grabbit-live-agentic-access
source_filename: grabbit-live-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/grabbit-live-openapi.json, openapi/www.grabbit.live_openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 2\n    connected: 8\n  by_consequence:\n    write: 2\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /grabs\n  method: post\n  operationId: createGrab\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - grabs\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /grabs\n  method: get\n  operationId: listGrabs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - grabs\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grabs/{id}\n  method: get\n  operationId: getGrab\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - grabs\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - grabs\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - grabs\n- path: /grabs\n  method: post\n  operationId: createGrab\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - grabs\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /grabs\n  method: get\n  operationId: listGrabs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - grabs\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grabs/{id}\n  method: get\n  operationId: getGrab\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - grabs\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - grabs\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - grabs\n"
source_yaml_url: https://artifacts.apis.io/grabbit-live/agentic-access/grabbit-live-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- Company
- Screenshots
- AI Agents
- Automation
- Visual
---
