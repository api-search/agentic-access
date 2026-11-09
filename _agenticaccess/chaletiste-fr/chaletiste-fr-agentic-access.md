---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 12
api_specs:
- filename: chaletiste-fr-calculs-api-openapi.yml
  format: yaml
  label: Chaletiste Calculs API
  slug: chaletiste-fr-calculs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaletiste-fr/openapi/chaletiste-fr-calculs-api-openapi.yml
- filename: chaletiste-fr-donn-es-api-openapi.yml
  format: yaml
  label: Chaletiste Données API
  slug: chaletiste-fr-donn-es-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaletiste-fr/openapi/chaletiste-fr-donn-es-api-openapi.yml
- filename: chaletiste-fr-recherche-api-openapi.yml
  format: yaml
  label: Chaletiste Recherche API
  slug: chaletiste-fr-recherche-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaletiste-fr/openapi/chaletiste-fr-recherche-api-openapi.yml
- filename: chaletiste-fr-transactions-api-openapi.yml
  format: yaml
  label: Chaletiste Transactions API
  slug: chaletiste-fr-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaletiste-fr/openapi/chaletiste-fr-transactions-api-openapi.yml
consequence_counts:
  read: 12
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chaletiste Fr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Chaletiste exposes 15 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chaletiste
provider_slug: chaletiste-fr
slug: chaletiste-fr-agentic-access
source_filename: chaletiste-fr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/chaletiste-fr-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 12\n    acting: 3\n  by_consequence:\n    read: 12\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/index.json\n  method: get\n  operationId: getIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products.json\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products/{id}.json\n\
  \  method: get\n  operationId: getProductFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/brands.json\n  method: get\n  operationId: listBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/categories.json\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/guides.json\n  method: get\n  operationId: listGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  operationId: searchChalets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/compare\n  method: get\n  operationId: compareChalets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/budget\n  method: get\n  operationId: estimateBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/permit\n  method: get\n  operationId: checkPermit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quote\n  method: post\n  operationId: requestQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/price-alert\n  method: post\n  operationId: createPriceAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/match\n  method: post\n  operationId: findChalets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/match-photo\n  method: post\n  operationId: findChaletsFromPhoto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/chaletiste-fr/agentic-access/chaletiste-fr-agentic-access.yml
summary_line: 15 operations · 3 acting
tags:
- Company
- Data
- Real Estate
- Construction
- Open Data
---
