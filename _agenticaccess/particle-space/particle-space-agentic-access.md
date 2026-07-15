---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Property Records API
  slug: property-records
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Address Search API
  slug: address-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Valuations API
  slug: valuations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Comparables API
  slug: comps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Listings API
  slug: listings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Particle Space Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Particle Space exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Particle Space
provider_slug: particle-space
slug: particle-space-agentic-access
source_filename: particle-space-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/particle-space-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /properties\n  method: get\n  operationId: listProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{id}\n  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/search\n  method: get\n  operationId: searchProperties\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valuations\n  method: get\n  operationId: getValuation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comparables\n  method: get\n  operationId: getComparables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings\n  method: get\n  operationId: listListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{id}\n  method: get\n  operationId: getListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/agentic-access/particle-space-agentic-access.yml
summary_line: 7 operations
tags:
- Real Estate
- Property Data
- PropTech
- Listings
- Valuations
---
