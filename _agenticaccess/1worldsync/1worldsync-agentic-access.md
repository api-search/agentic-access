---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: 1worldsync-fetchproduct-api-openapi.yml
  format: yaml
  label: 1WorldSync FetchProduct API
  slug: 1worldsync-fetchproduct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1worldsync/refs/heads/main/openapi/1worldsync-fetchproduct-api-openapi.yml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 1Worldsync Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: '1WorldSync exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 1WorldSync
provider_slug: 1worldsync
slug: 1worldsync-agentic-access
source_filename: 1worldsync-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/1worldsync-fetchproduct-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /V1/product/count\n  method: post\n  operationId: fetchItemCountByCriteria\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /V1/product/fetch\n  method: post\n  operationId: fetchItemByCriteria\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /V1/product/hierarchy\n\
  \  method: post\n  operationId: fetchHierarchiesByCriteria\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1worldsync/refs/heads/main/agentic-access/1worldsync-agentic-access.yml
summary_line: 3 operations
tags:
- Company
- Product Content
- GDSN
- Data Syndication
- Master Data
- Digital Shelf
- Product Information Management
- Consumer Packaged Goods
- Retail
- GS1
---
