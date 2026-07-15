---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 9
api_specs:
- filename: la-trobe-university-opal-figshare.yaml
  format: yaml
  label: OPAL (Open @ La Trobe) Figshare REST API
  slug: opal-figshare-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-trobe-university/refs/heads/main/openapi/la-trobe-university-opal-figshare.yaml
consequence_counts:
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: La Trobe University Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'La Trobe University exposes 11 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: La Trobe University
provider_slug: la-trobe-university
slug: la-trobe-university-agentic-access
source_filename: la-trobe-university-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/la-trobe-university-opal-figshare.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 9\n    acting: 2\n  by_consequence:\n    read: 9\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /articles\n  method: get\n  operationId: articles_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/search\n  method: post\n  operationId: articles_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /articles/{article_id}\n  method: get\n  operationId: article_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/files\n  method: get\n  operationId: article_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/files/{file_id}\n  method: get\n  operationId: article_file_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/versions\n  method: get\n  operationId: article_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /articles/{article_id}/versions/{version_id}\n  method: get\n  operationId: article_version_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: collections_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/search\n  method: post\n  operationId: collections_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}\n  method: get\n  operationId: collection_details\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/articles\n  method: get\n  operationId: collection_articles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-trobe-university/refs/heads/main/agentic-access/la-trobe-university-agentic-access.yml
summary_line: 11 operations · 2 acting
tags:
- Education
- Higher Education
- University
- Australia
- Research
- Open Data
- Repository
- Library
---
