---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: disputes-online-categories-api-openapi.yml
  format: yaml
  label: Disputes.online Categories API
  slug: disputes-online-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disputes-online/openapi/disputes-online-categories-api-openapi.yml
- filename: disputes-online-disputes-api-openapi.yml
  format: yaml
  label: Disputes.online Disputes API
  slug: disputes-online-disputes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disputes-online/openapi/disputes-online-disputes-api-openapi.yml
- filename: disputes-online-feeds-api-openapi.yml
  format: yaml
  label: Disputes.online Feeds API
  slug: disputes-online-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disputes-online/openapi/disputes-online-feeds-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Disputes Online Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Disputes.online exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Disputes.online
provider_slug: disputes-online
slug: disputes-online-agentic-access
source_filename: disputes-online-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/disputes-online-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /disputes/finder\n  method: get\n  operationId: listDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disputes/search\n  method: get\n  operationId: searchDisputesByTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disputes/{id}\n  method: get\n  operationId: getDispute\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disputes/{id}/odds\n  method: get\n  operationId: getDisputeOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disputes/variant/{id}\n  method: get\n  operationId: getDisputeByVariant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /category/\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rss.xml\n  method: get\n  operationId: getFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /rss.json\n  method: get\n  operationId: getJSONFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/disputes-online/agentic-access/disputes-online-agentic-access.yml
summary_line: 8 operations
tags:
- Dispute
- Community
- Predictions
- Sports
- Politics
---
