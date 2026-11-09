---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: filtersolutions-co-uk-openapi.yml
  format: yaml
  label: Filter Solutions Ltd Public Content API
  slug: filter-solutions-ltd-public-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filtersolutions-co-uk/openapi/filtersolutions-co-uk-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Filtersolutions Co Uk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Filter Solutions Ltd exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Filter Solutions Ltd
provider_slug: filtersolutions-co-uk
slug: filtersolutions-co-uk-agentic-access
source_filename: filtersolutions-co-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/filtersolutions-co-uk-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /wp-json/wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp-json/wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp-json/wp/v2/categories\n  method: get\n  operationId:\
  \ listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp-json/wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp-json/filter-solutions-agent/v1/health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/filtersolutions-co-uk/agentic-access/filtersolutions-co-uk-agentic-access.yml
summary_line: 5 operations
tags:
- Company
- Oil Filtration
- Condition Monitoring
- Industrial Maintenance
- Lubricants
- Power Generation
- United Kingdom
---
