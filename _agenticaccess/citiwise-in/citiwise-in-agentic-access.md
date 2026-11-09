---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 9
api_specs:
- filename: citiwise-in-check-api-openapi.yml
  format: yaml
  label: Citiwise Check API
  slug: citiwise-in-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-check-api-openapi.yml
- filename: citiwise-in-clause-api-openapi.yml
  format: yaml
  label: Citiwise Clause API
  slug: citiwise-in-clause-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-clause-api-openapi.yml
- filename: citiwise-in-compare-api-openapi.yml
  format: yaml
  label: Citiwise Compare API
  slug: citiwise-in-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-compare-api-openapi.yml
- filename: citiwise-in-dxf-api-openapi.yml
  format: yaml
  label: Citiwise Dxf API
  slug: citiwise-in-dxf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-dxf-api-openapi.yml
- filename: citiwise-in-feasibility-api-openapi.yml
  format: yaml
  label: Citiwise Feasibility API
  slug: citiwise-in-feasibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-feasibility-api-openapi.yml
- filename: citiwise-in-find-api-openapi.yml
  format: yaml
  label: Citiwise Find API
  slug: citiwise-in-find-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-find-api-openapi.yml
- filename: citiwise-in-pdf-api-openapi.yml
  format: yaml
  label: Citiwise PDF API
  slug: citiwise-in-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-pdf-api-openapi.yml
- filename: citiwise-in-plot-api-openapi.yml
  format: yaml
  label: Citiwise Plot API
  slug: citiwise-in-plot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-plot-api-openapi.yml
- filename: citiwise-in-regulation-api-openapi.yml
  format: yaml
  label: Citiwise Regulation API
  slug: citiwise-in-regulation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-regulation-api-openapi.yml
- filename: citiwise-in-search-api-openapi.yml
  format: yaml
  label: Citiwise Search API
  slug: citiwise-in-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-search-api-openapi.yml
- filename: citiwise-in-towns-api-openapi.yml
  format: yaml
  label: Citiwise Towns API
  slug: citiwise-in-towns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citiwise-in/openapi/citiwise-in-towns-api-openapi.yml
consequence_counts:
  read: 9
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Citiwise In Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Citiwise exposes 13 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Citiwise
provider_slug: citiwise-in
slug: citiwise-in-agentic-access
source_filename: citiwise-in-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/citiwise-in-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 9\n    acting: 4\n  by_consequence:\n    read: 9\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/feasibility\n  method: get\n  operationId: feasibilityByLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feasibility\n  method: post\n  operationId: feasibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/compare\n  method: get\n  operationId: compareUsesByLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/compare\n  method: post\n  operationId: compareUses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/check\n  method: post\n  operationId: checkDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/clause\n  method: get\n  operationId: clause\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: get\n  operationId: searchUdcpr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/towns\n  method: get\n  operationId: towns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pdf\n  method: get\n  operationId: reportPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/plot\n  method: post\n  operationId: drawPlot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dxf\n  method: get\n  operationId: plotDxf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/regulation\n  method: get\n  operationId: regulation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/find\n  method: get\n  operationId: findUdcpr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/citiwise-in/agentic-access/citiwise-in-agentic-access.yml
summary_line: 13 operations · 4 acting
tags:
- Real Estate
- India
- Urban Planning
- Land Use
- Mapping
---
