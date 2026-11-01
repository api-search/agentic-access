---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: dyno-nobel-robotslandingpage-api-openapi.yml
  format: yaml
  label: Dyno Nobel Robots Landing Page API
  slug: dyno-nobel-robotslandingpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-robotslandingpage-api-openapi.yml
- filename: dyno-nobel-robotstext-api-openapi.yml
  format: yaml
  label: Dyno Nobel Robots Text API
  slug: dyno-nobel-robotstext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-robotstext-api-openapi.yml
- filename: dyno-nobel-searchapi-api-openapi.yml
  format: yaml
  label: Dyno Nobel Search API
  slug: dyno-nobel-searchapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-searchapi-api-openapi.yml
- filename: dyno-nobel-sitemanifest-api-openapi.yml
  format: yaml
  label: Dyno Nobel Site Manifest API
  slug: dyno-nobel-sitemanifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-sitemanifest-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dyno Nobel Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Dyno Nobel exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dyno Nobel
provider_slug: dyno-nobel
slug: dyno-nobel-agentic-access
source_filename: dyno-nobel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/dyno-nobel-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /stott.robotshandler/administration\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stott.robotshandler/static/{staticFileName}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /robots.txt\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/global-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/article-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/document-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/dyno-nobel-product-hub-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/ipf-product-search\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/resource-hub-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/extended-resource-hub-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/team-member-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/ipf-location-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/ipf-related-resource\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/autocomplete\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SearchApi/yourip\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site.webmanifest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/agentic-access/dyno-nobel-agentic-access.yml
summary_line: 16 operations
tags:
- Company
- Explosives
- Mining
- Industrial Manufacturing
- Blasting
- Australia
---
