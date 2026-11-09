---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: bestaffiliateprograms-cc-categories-api-openapi.yml
  format: yaml
  label: BestAffiliatePrograms.cc Categories API
  slug: bestaffiliateprograms-cc-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bestaffiliateprograms-cc/openapi/bestaffiliateprograms-cc-categories-api-openapi.yml
- filename: bestaffiliateprograms-cc-networks-api-openapi.yml
  format: yaml
  label: BestAffiliatePrograms.cc Networks API
  slug: bestaffiliateprograms-cc-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bestaffiliateprograms-cc/openapi/bestaffiliateprograms-cc-networks-api-openapi.yml
- filename: bestaffiliateprograms-cc-programs-api-openapi.yml
  format: yaml
  label: BestAffiliatePrograms.cc Programs API
  slug: bestaffiliateprograms-cc-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bestaffiliateprograms-cc/openapi/bestaffiliateprograms-cc-programs-api-openapi.yml
- filename: bestaffiliateprograms-cc-stats-api-openapi.yml
  format: yaml
  label: BestAffiliatePrograms.cc Stats API
  slug: bestaffiliateprograms-cc-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bestaffiliateprograms-cc/openapi/bestaffiliateprograms-cc-stats-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bestaffiliateprograms Cc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'BestAffiliatePrograms.cc exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BestAffiliatePrograms.cc
provider_slug: bestaffiliateprograms-cc
slug: bestaffiliateprograms-cc-agentic-access
source_filename: bestaffiliateprograms-cc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bestaffiliateprograms-cc-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /programs\n  method: get\n  operationId: listPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/{slug}\n  method: get\n  operationId: getProgram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: listCategories\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks\n  method: get\n  operationId: listNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bestaffiliateprograms-cc/agentic-access/bestaffiliateprograms-cc-agentic-access.yml
summary_line: 5 operations
tags:
- Affiliates
- Comparison
- Marketing
- Data
- Platform
---
