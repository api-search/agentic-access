---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: feedico-io-auth-api-openapi.yml
  format: yaml
  label: feedico-io Auth API
  slug: feedico-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedico-io/openapi/feedico-io-auth-api-openapi.yml
- filename: feedico-io-catalog-api-openapi.yml
  format: yaml
  label: feedico-io Catalog API
  slug: feedico-io-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedico-io/openapi/feedico-io-catalog-api-openapi.yml
- filename: feedico-io-coupons-api-openapi.yml
  format: yaml
  label: feedico-io Coupons API
  slug: feedico-io-coupons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedico-io/openapi/feedico-io-coupons-api-openapi.yml
- filename: feedico-io-firms-api-openapi.yml
  format: yaml
  label: feedico-io Firms API
  slug: feedico-io-firms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedico-io/openapi/feedico-io-firms-api-openapi.yml
- filename: feedico-io-global-catalogue-api-openapi.yml
  format: yaml
  label: feedico-io Global catalogue API
  slug: feedico-io-global-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedico-io/openapi/feedico-io-global-catalogue-api-openapi.yml
- filename: feedico-io-health-api-openapi.yml
  format: yaml
  label: feedico-io Health API
  slug: feedico-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedico-io/openapi/feedico-io-health-api-openapi.yml
- filename: feedico-io-products-api-openapi.yml
  format: yaml
  label: feedico-io Products API
  slug: feedico-io-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedico-io/openapi/feedico-io-products-api-openapi.yml
- filename: feedico-io-user-api-openapi.yml
  format: yaml
  label: feedico-io User API
  slug: feedico-io-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedico-io/openapi/feedico-io-user-api-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Feedico Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'feedico-io exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: feedico-io
provider_slug: feedico-io
slug: feedico-io-agentic-access
source_filename: feedico-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/feedico-io-customer.yaml, openapi/feedico-io-openapi.yaml, openapi/feedico-io-partner.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 6\n    acting: 2\n  by_consequence:\n    read: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/me/products\n  method: post\n  operationId: meProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/catalog/products\n  method: post\n  operationId: catalogProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/networks\n  method: post\n  operationId: meNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/coupons\n  method: post\n  operationId: meCoupons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/login\n  method: post\n  operationId: authLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me\n  method: get\n  operationId: me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog/coupons\n  method: post\n  operationId: listPartnerCoupons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/feedico-io/agentic-access/feedico-io-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Affiliates
- Marketing
- E-Commerce
- Coupons
---
