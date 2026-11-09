---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: scento-contrast-api-openapi.yml
  format: yaml
  label: Scento Compendium API Contrast API
  slug: scento-contrast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-contrast-api-openapi.yml
- filename: scento-perfume-portrait-api-openapi.yml
  format: yaml
  label: Scento Compendium API Perfume portrait API
  slug: scento-perfume-portrait-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-perfume-portrait-api-openapi.yml
- filename: scento-scent-neighbours-api-openapi.yml
  format: yaml
  label: Scento Compendium API Scent neighbours API
  slug: scento-scent-neighbours-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-scent-neighbours-api-openapi.yml
- filename: scento-search-the-compendium-api-openapi.yml
  format: yaml
  label: Scento Compendium API Search the Compendium API
  slug: scento-search-the-compendium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scento/openapi/scento-search-the-compendium-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scento Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Scento Compendium API exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scento Compendium API
provider_slug: scento
slug: scento-agentic-access
source_filename: scento-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/scento-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  operationId: searchCompendium\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /perfumes\n  method: get\n  operationId: searchPerfumes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /perfumes/{perfume}\n  method: get\n  operationId: getPerfumePortrait\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /perfumes/{perfume}/neighbours\n  method: get\n  operationId: getScentNeighbours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contrast\n  method: get\n  operationId: getPerfumeContrast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/scento/agentic-access/scento-agentic-access.yml
summary_line: 5 operations
tags:
- Company
- E-Commerce
- Fragrance
- Decant
---
