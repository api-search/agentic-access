---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Property Records API
  slug: property-records
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Rental Estimate API
  slug: rental-estimate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Sale Estimate API
  slug: sale-estimate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Listings API
  slug: listings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Realtymole Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'RealtyMole exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RealtyMole
provider_slug: realtymole
slug: realtymole-agentic-access
source_filename: realtymole-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/realtymole-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /properties\n  method: get\n  operationId: getProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentalPrice\n  method: get\n  operationId: getRentalPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /salePrice\n  method: get\n  operationId: getSalePrice\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saleListings\n  method: get\n  operationId: getSaleListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentalListings\n  method: get\n  operationId: getRentalListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/agentic-access/realtymole-agentic-access.yml
summary_line: 5 operations
tags:
- Real Estate
- Property Data
- Rental Estimate
- Valuation
- Listings
---
