---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: swagger-codegen-generation-api-openapi.yml
  format: yaml
  label: Swagger Codegen Generation API
  slug: swagger-codegen-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-generation-api-openapi.yml
- filename: swagger-codegen-languages-api-openapi.yml
  format: yaml
  label: Swagger Codegen Languages API
  slug: swagger-codegen-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-languages-api-openapi.yml
- filename: swagger-codegen-options-api-openapi.yml
  format: yaml
  label: Swagger Codegen Options API
  slug: swagger-codegen-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-options-api-openapi.yml
- filename: swagger-codegen-utilities-api-openapi.yml
  format: yaml
  label: Swagger Codegen Utilities API
  slug: swagger-codegen-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-utilities-api-openapi.yml
- filename: swagger-codegen-clients-api-openapi.yml
  format: yaml
  label: Swagger Codegen Clients API
  slug: swagger-codegen-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-clients-api-openapi.yml
- filename: swagger-codegen-documentation-api-openapi.yml
  format: yaml
  label: Swagger Codegen Documentation API
  slug: swagger-codegen-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-documentation-api-openapi.yml
- filename: swagger-codegen-servers-api-openapi.yml
  format: yaml
  label: Swagger Codegen Servers API
  slug: swagger-codegen-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-servers-api-openapi.yml
consequence_counts:
  read: 7
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Swagger Codegen Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Swagger Codegen exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Swagger Codegen
provider_slug: swagger-codegen
slug: swagger-codegen-agentic-access
source_filename: swagger-codegen-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/swagger-codegen-generation-api-openapi.yml, openapi/swagger-codegen-languages-api-openapi.yml,\n  openapi/swagger-codegen-options-api-openapi.yml, openapi/swagger-codegen-utilities-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 3\n    connected: 7\n  by_consequence:\n    write: 3\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /generate\n  method: post\n  operationId: generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /generate\n  method: get\n  operationId: generateFromURL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{type}/{version}\n  method: get\n  operationId: languages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /types\n  method: get\n  operationId: languagesMulti\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients\n  method: get\n  operationId: clientLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers\n  method: get\n  operationId: serverLanguages\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation\n  method: get\n  operationId: documentationLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options\n  method: get\n  operationId: listOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model\n  method: post\n  operationId: generateBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render\n  method: post\n  operationId: renderTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/agentic-access/swagger-codegen-agentic-access.yml
summary_line: 10 operations · 3 acting
tags:
- Client Libraries
- Code Generation
- Open-Source
- OpenAPI
- SDK
---
