---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 17
api_specs:
- filename: tu-dresden-slub-lod.yaml
  format: yaml
  label: SLUB Dresden Linked Open Data API
  slug: slub-lod
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tu-dresden/refs/heads/main/openapi/tu-dresden-slub-lod.yaml
consequence_counts:
  read: 17
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tu Dresden Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'TU Dresden exposes 18 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TU Dresden
provider_slug: tu-dresden
slug: tu-dresden-agentic-access
source_filename: tu-dresden-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tu-dresden-slub-lod.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 17\n    acting: 1\n  by_consequence:\n    read: 17\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /explore/aggregations\n  method: get\n  operationId: aggregateTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /explore/correlations\n  method: get\n  operationId: correlateTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /explore/topicsearch\n\
  \  method: get\n  operationId: queryTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reconcile/\n  method: get\n  operationId: getReconcile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reconcile/\n  method: post\n  operationId: postReconcile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reconcile/flyout/entity\n  method: get\n  operationId: flyoutEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reconcile/flyout/property\n\
  \  method: get\n  operationId: flyoutProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reconcile/flyout/type\n  method: get\n  operationId: flyoutType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reconcile/properties\n  method: get\n  operationId: reconcileProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reconcile/suggest/entity\n  method: get\n  operationId: suggestEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reconcile/suggest/property\n  method: get\n  operationId: suggestProperty\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reconcile/suggest/type\n  method: get\n  operationId: suggestType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /source/{source_index}/{id}\n  method: get\n  operationId: getSourceRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{authority_provider}/{entity_type}/{id}\n  method: get\n  operationId: getByAuthorityAndEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /{authority_provider}/{id}\n  method: get\n  operationId: getByAuthority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{entity_type}/search\n  method: get\n  operationId: searchInIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{entity_type}/{id}\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-dresden/refs/heads/main/agentic-access/tu-dresden-agentic-access.yml
summary_line: 18 operations · 1 acting
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- Germany
---
