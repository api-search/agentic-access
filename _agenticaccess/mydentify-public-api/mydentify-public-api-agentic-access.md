---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: mydentify-public-api-directories-api-openapi.yml
  format: yaml
  label: Mydentify Public API Directories API
  slug: mydentify-public-api-directories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-directories-api-openapi.yml
- filename: mydentify-public-api-directories-json-api-openapi.yml
  format: yaml
  label: Mydentify Public API Directories.json API
  slug: mydentify-public-api-directories-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-directories-json-api-openapi.yml
- filename: mydentify-public-api-imports-api-openapi.yml
  format: yaml
  label: Mydentify Public API Imports API
  slug: mydentify-public-api-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-imports-api-openapi.yml
- filename: mydentify-public-api-leaderboards-api-openapi.yml
  format: yaml
  label: Mydentify Public API Leaderboards API
  slug: mydentify-public-api-leaderboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-leaderboards-api-openapi.yml
- filename: mydentify-public-api-leaderboards-json-api-openapi.yml
  format: yaml
  label: Mydentify Public API Leaderboards.json API
  slug: mydentify-public-api-leaderboards-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-leaderboards-json-api-openapi.yml
- filename: mydentify-public-api-product-categories-json-api-openapi.yml
  format: yaml
  label: Mydentify Public API Product Categories.json API
  slug: mydentify-public-api-product-categories-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/openapi/mydentify-public-api-product-categories-json-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mydentify Public Api Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/imports/{id}/manual-review
operation_count: 14
overview: 'Mydentify Public API exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mydentify Public API
provider_slug: mydentify-public-api
slug: mydentify-public-api-agentic-access
source_filename: mydentify-public-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/mydentify-public-api-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    write: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /leaderboards.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/leaderboards/{slug}/json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directories.json\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product-categories.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/directories/{slug}/json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directories/{slug}/llms.txt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/imports/dry-run\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/imports\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/imports/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/imports/{id}/events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/imports/{id}/retry\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/imports/{id}/manual-review\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/imports/{id}/goals\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/imports/{id}/verify-badge\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mydentify-public-api/refs/heads/main/agentic-access/mydentify-public-api-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- product discovery
- startup directories
- leaderboards
- research
- Software-as-a-Service
- Developer Tools
- agent-native
- llms-txt
- agent skills
- Directories
---
