---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: aramark-organization-api-openapi.yml
  format: yaml
  label: Aramark Organization API
  slug: aramark-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/openapi/aramark-organization-api-openapi.yml
- filename: aramark-point-of-sale-api-openapi.yml
  format: yaml
  label: Aramark Point of Sale API
  slug: aramark-point-of-sale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/openapi/aramark-point-of-sale-api-openapi.yml
- filename: aramark-product-api-openapi.yml
  format: yaml
  label: Aramark Product API
  slug: aramark-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/openapi/aramark-product-api-openapi.yml
- filename: aramark-profit-centers-api-openapi.yml
  format: yaml
  label: Aramark Profit Centers API
  slug: aramark-profit-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/openapi/aramark-profit-centers-api-openapi.yml
- filename: aramark-revenue-api-openapi.yml
  format: yaml
  label: Aramark Revenue API
  slug: aramark-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/openapi/aramark-revenue-api-openapi.yml
- filename: aramark-service-api-openapi.yml
  format: yaml
  label: Aramark Service API
  slug: aramark-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/openapi/aramark-service-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aramark Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Aramark exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Aramark
provider_slug: aramark
slug: aramark-agentic-access
source_filename: aramark-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/marko-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /organization\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profit-centers\n  method: get\n  operationId: getProfitCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /revenue-snapshot\n  method: get\n  operationId: getRevenueSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /point-of-sale\n  method: get\n  operationId: getPointOfSale\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/agentic-access/aramark-agentic-access.yml
summary_line: 6 operations
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
---
