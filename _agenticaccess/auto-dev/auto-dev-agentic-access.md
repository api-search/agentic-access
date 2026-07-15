---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: auto-dev-openapi.yml
  format: yaml
  label: Auto.dev VIN Decoding API
  slug: vin-decoding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-openapi.yml
- filename: auto-dev-openapi.yml
  format: yaml
  label: Auto.dev Listings / Search API
  slug: listings-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-openapi.yml
- filename: auto-dev-openapi.yml
  format: yaml
  label: Auto.dev Market Value / Pricing API
  slug: market-value-pricing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-openapi.yml
- filename: auto-dev-openapi.yml
  format: yaml
  label: Auto.dev Dealers API
  slug: dealers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-openapi.yml
- filename: auto-dev-openapi.yml
  format: yaml
  label: Auto.dev Recalls API
  slug: recalls
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Auto Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Auto.dev exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Auto.dev
provider_slug: auto-dev
slug: auto-dev-agentic-access
source_filename: auto-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/auto-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /vin/{vin}\n  method: get\n  operationId: decodeVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /specs/{vin}\n  method: get\n  operationId: getSpecifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings\n  method: get\n  operationId: searchListings\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{vin}\n  method: get\n  operationId: getListingByVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openrecalls/{vin}\n  method: get\n  operationId: getOpenRecalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/agentic-access/auto-dev-agentic-access.yml
summary_line: 5 operations
tags:
- Automotive
- Vehicle Data
- VIN Decoding
- Vehicle Listings
- Recalls
---
