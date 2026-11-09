---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: bezal-ai-businesses-api-openapi.yml
  format: yaml
  label: Bezal Businesses API
  slug: bezal-ai-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-businesses-api-openapi.yml
- filename: bezal-ai-categories-api-openapi.yml
  format: yaml
  label: Bezal Categories API
  slug: bezal-ai-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-categories-api-openapi.yml
- filename: bezal-ai-health-api-openapi.yml
  format: yaml
  label: Bezal Health API
  slug: bezal-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-health-api-openapi.yml
- filename: bezal-ai-requests-api-openapi.yml
  format: yaml
  label: Bezal Requests API
  slug: bezal-ai-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-requests-api-openapi.yml
- filename: bezal-ai-open-api-api-openapi.yml
  format: yaml
  label: Bezal Open API
  slug: bezal-ai-open-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-open-api-api-openapi.yml
consequence_counts:
  physical: 1
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bezal Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /requests
operation_count: 6
overview: 'Bezal exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bezal
provider_slug: bezal-ai
slug: bezal-ai-agentic-access
source_filename: bezal-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bezal-ai-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /businesses/search\n  method: get\n  operationId: searchBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{id}\n  method: get\n  operationId: getBusinessById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method:\
  \ get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /requests\n  method: post\n  operationId: createQuoteRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi\n  method: get\n  operationId: getOpenApiSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bezal-ai/agentic-access/bezal-ai-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Company
- Artificial Intelligence
- Software-as-a-Service
- Local Business
- Lead Generation
- Automation
---
