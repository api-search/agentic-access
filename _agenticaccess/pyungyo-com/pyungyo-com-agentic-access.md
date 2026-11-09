---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: pyungyo-com-carriers-api-openapi.yml
  format: yaml
  label: pyungyo-com Carriers API
  slug: pyungyo-com-carriers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyungyo-com/openapi/pyungyo-com-carriers-api-openapi.yml
- filename: pyungyo-com-changes-api-openapi.yml
  format: yaml
  label: pyungyo-com Changes API
  slug: pyungyo-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyungyo-com/openapi/pyungyo-com-changes-api-openapi.yml
- filename: pyungyo-com-cheapest-api-openapi.yml
  format: yaml
  label: pyungyo-com Cheapest API
  slug: pyungyo-com-cheapest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyungyo-com/openapi/pyungyo-com-cheapest-api-openapi.yml
- filename: pyungyo-com-index-api-openapi.yml
  format: yaml
  label: pyungyo-com Index API
  slug: pyungyo-com-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyungyo-com/openapi/pyungyo-com-index-api-openapi.yml
- filename: pyungyo-com-meta-api-openapi.yml
  format: yaml
  label: pyungyo-com Meta API
  slug: pyungyo-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyungyo-com/openapi/pyungyo-com-meta-api-openapi.yml
- filename: pyungyo-com-plans-api-openapi.yml
  format: yaml
  label: pyungyo-com Plans API
  slug: pyungyo-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyungyo-com/openapi/pyungyo-com-plans-api-openapi.yml
- filename: pyungyo-com-search-api-openapi.yml
  format: yaml
  label: pyungyo-com Search API
  slug: pyungyo-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyungyo-com/openapi/pyungyo-com-search-api-openapi.yml
- filename: pyungyo-com-ssal-api-openapi.yml
  format: yaml
  label: pyungyo-com Ssal API
  slug: pyungyo-com-ssal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyungyo-com/openapi/pyungyo-com-ssal-api-openapi.yml
- filename: pyungyo-com-stats-api-openapi.yml
  format: yaml
  label: pyungyo-com Stats API
  slug: pyungyo-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyungyo-com/openapi/pyungyo-com-stats-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pyungyo Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'pyungyo-com exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: pyungyo-com
provider_slug: pyungyo-com
slug: pyungyo-com-agentic-access
source_filename: pyungyo-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/pyungyo-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/search\n  method: get\n  operationId: searchPlansByText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/plans\n  method: get\n  operationId: searchPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/plans/{id}\n  method: get\n  operationId: getPlan\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/plans/{id}/history\n  method: get\n  operationId: getPlanPriceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cheapest\n  method: get\n  operationId: cheapestByData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stats\n  method: get\n  operationId: marketStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ssal\n  method: get\n  operationId: ssalEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/changes\n  method: get\n  operationId: recentPriceChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/carriers\n  method: get\n  operationId: listCarriers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/index\n  method: get\n  operationId: priceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/meta\n  method: get\n  operationId: meta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/pyungyo-com/agentic-access/pyungyo-com-agentic-access.yml
summary_line: 11 operations
tags:
- Company
- Telecommunications
- Mobile
- South Korea
- Price Comparison
- OpenAPI
---
