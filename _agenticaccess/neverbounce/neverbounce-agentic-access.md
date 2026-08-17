---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: neverbounce-account-api-openapi.yml
  format: yaml
  label: NeverBounce Account API
  slug: neverbounce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-account-api-openapi.yml
- filename: neverbounce-jobs-api-openapi.yml
  format: yaml
  label: NeverBounce Jobs API
  slug: neverbounce-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-jobs-api-openapi.yml
- filename: neverbounce-single-api-openapi.yml
  format: yaml
  label: NeverBounce Single API
  slug: neverbounce-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-single-api-openapi.yml
- filename: neverbounce-poe-api-openapi.yml
  format: yaml
  label: NeverBounce POE API
  slug: neverbounce-poe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-poe-api-openapi.yml
consequence_counts:
  read: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Neverbounce Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'NeverBounce exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NeverBounce
provider_slug: neverbounce
slug: neverbounce-agentic-access
source_filename: neverbounce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/neverbounce-account-api-openapi.yml, openapi/neverbounce-jobs-api-openapi.yml,\n  openapi/neverbounce-poe-api-openapi.yml, openapi/neverbounce-single-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 5\n    acting: 5\n  by_consequence:\n    read: 5\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /account/info\n  method: get\n  operationId: account-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/search\n  method: get\n  operationId: jobs-search\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/create\n  method: post\n  operationId: jobs-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/parse\n  method: post\n  operationId: jobs-parse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/start\n  method: post\n  operationId: jobs-start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/status\n  method: get\n  operationId: jobs-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/results\n  method: get\n  operationId: jobs-results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/delete\n  method: post\n  operationId: jobs-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poe/confirm\n  method: post\n  operationId: widget-poe-confirm\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /single/check\n  method: get\n  operationId: single-check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/agentic-access/neverbounce-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- Email Verification
- Email Validation
- Email Hygiene
- Deliverability
- Marketing
- List Cleaning
- Data Quality
- ZoomInfo
---
