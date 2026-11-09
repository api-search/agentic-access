---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: docrocket-ai-brand-from-url-api-openapi.yml
  format: yaml
  label: docrocket-ai Brand From Url API
  slug: docrocket-ai-brand-from-url-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-brand-from-url-api-openapi.yml
- filename: docrocket-ai-generate-document-api-openapi.yml
  format: yaml
  label: docrocket-ai Generate Document API
  slug: docrocket-ai-generate-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-generate-document-api-openapi.yml
- filename: docrocket-ai-get-document-api-openapi.yml
  format: yaml
  label: docrocket-ai Get Document API
  slug: docrocket-ai-get-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-get-document-api-openapi.yml
- filename: docrocket-ai-https-json-api-api-openapi.yml
  format: yaml
  label: docrocket-ai HTTPS JSON API
  slug: docrocket-ai-https-json-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-https-json-api-api-openapi.yml
- filename: docrocket-ai-list-brands-api-openapi.yml
  format: yaml
  label: docrocket-ai List Brands API
  slug: docrocket-ai-list-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-list-brands-api-openapi.yml
- filename: docrocket-ai-list-components-api-openapi.yml
  format: yaml
  label: docrocket-ai List Components API
  slug: docrocket-ai-list-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-list-components-api-openapi.yml
- filename: docrocket-ai-list-templates-api-openapi.yml
  format: yaml
  label: docrocket-ai List Templates API
  slug: docrocket-ai-list-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-list-templates-api-openapi.yml
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Docrocket Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'docrocket-ai exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: docrocket-ai
provider_slug: docrocket-ai
slug: docrocket-ai-agentic-access
source_filename: docrocket-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/docrocket-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 4\n    connected: 4\n  by_consequence:\n    write: 4\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: http_invoke_action\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin\n  method: post\n  operationId: http_invoke_admin_action\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brand-from-url\n  method: post\n  operationId: docrocket_brand_from_url\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /list-brands\n  method: get\n  operationId: docrocket_list_brands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list-templates\n  method: get\n  operationId: docrocket_list_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /list-components\n  method: get\n  operationId: docrocket_list_components\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generate-document\n  method: post\n  operationId: docrocket_generate_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-document\n  method: get\n  operationId: docrocket_get_document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/docrocket-ai/agentic-access/docrocket-ai-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- Document Generation
- Multi-tenant SaaS
- Brand Extraction
- PDF Generation
- AI Agents
- MCP Protocol
- SaaS Integration
---
