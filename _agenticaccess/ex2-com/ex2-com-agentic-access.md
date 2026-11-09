---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: ex2-com-compare-api-openapi.yml
  format: yaml
  label: ex2-com Compare API
  slug: ex2-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-compare-api-openapi.yml
- filename: ex2-com-domains-api-openapi.yml
  format: yaml
  label: ex2-com Domains API
  slug: ex2-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-domains-api-openapi.yml
- filename: ex2-com-ex2-catalogue-api-api-openapi.yml
  format: yaml
  label: ex2-com Ex2 Catalogue API
  slug: ex2-com-ex2-catalogue-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-ex2-catalogue-api-api-openapi.yml
- filename: ex2-com-migration-api-openapi.yml
  format: yaml
  label: ex2-com Migration API
  slug: ex2-com-migration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-migration-api-openapi.yml
- filename: ex2-com-plans-api-openapi.yml
  format: yaml
  label: ex2-com Plans API
  slug: ex2-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-plans-api-openapi.yml
- filename: ex2-com-status-api-openapi.yml
  format: yaml
  label: ex2-com Status API
  slug: ex2-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ex2-com/openapi/ex2-com-status-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ex2 Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'ex2-com exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ex2-com
provider_slug: ex2-com
slug: ex2-com-agentic-access
source_filename: ex2-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/ex2-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/plans/{id}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/compare\n  method: get\n  operationId: comparePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/domains/pricing\n  method: get\n  operationId: getDomainPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/domains/availability\n  method: get\n  operationId: checkDomainAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/migration\n  method: get\n  operationId: quoteMigration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ex2-com/agentic-access/ex2-com-agentic-access.yml
summary_line: 8 operations
tags:
- Hosting
- Sustainability
- Web Hosting
- Quebec
- GreenTech
---
