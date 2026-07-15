---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 3
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Cloudflare D1 API
  slug: cloudflare-d1-api
  spec_type: OpenAPI
  url: https://developers.cloudflare.com/api/resources/d1/subresources/database/
consequence_counts:
  read: 3
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudflare D1 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Cloudflare D1 exposes 12 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloudflare D1
provider_slug: cloudflare-d1
slug: cloudflare-d1-agentic-access
source_filename: cloudflare-d1-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloudflare-d1-cloudflare-d1-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 3\n    acting: 9\n  by_consequence:\n    read: 3\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/{account_id}/d1/database\n  method: get\n  operationId: d1-list-databases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/d1/database\n  method: post\n  operationId: d1-create-database\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/d1/database/{database_id}\n  method: delete\n  operationId: d1-delete-database\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/d1/database/{database_id}\n  method: get\n  operationId: d1-get-database\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/d1/database/{database_id}\n  method: patch\n  operationId: d1-update-partial-database\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/d1/database/{database_id}\n  method: put\n  operationId: d1-update-database\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/d1/database/{database_id}/export\n  method: post\n  operationId: d1-export-database\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/d1/database/{database_id}/import\n\
  \  method: post\n  operationId: d1-import-database\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/d1/database/{database_id}/query\n  method: post\n  operationId: d1-query-database\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/d1/database/{database_id}/raw\n  method: post\n  operationId: d1-raw-database-query\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/d1/database/{database_id}/time_travel/bookmark\n  method: get\n  operationId: d1-time-travel-get-bookmark\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/d1/database/{database_id}/time_travel/restore\n  method: post\n  operationId: d1-time-travel-restore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-d1/refs/heads/main/agentic-access/cloudflare-d1-agentic-access.yml
summary_line: 12 operations · 9 acting
tags:
- Database
- SQLite
- Serverless
- Edge Computing
- SQL
- Cloudflare
- Workers
---
