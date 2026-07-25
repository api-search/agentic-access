---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: tenor-autocomplete-api-openapi.yml
  format: yaml
  label: Tenor Autocomplete API
  slug: tenor-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenor/refs/heads/main/openapi/tenor-autocomplete-api-openapi.yml
- filename: tenor-categories-api-openapi.yml
  format: yaml
  label: Tenor Categories API
  slug: tenor-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenor/refs/heads/main/openapi/tenor-categories-api-openapi.yml
- filename: tenor-featured-api-openapi.yml
  format: yaml
  label: Tenor Featured API
  slug: tenor-featured-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenor/refs/heads/main/openapi/tenor-featured-api-openapi.yml
- filename: tenor-posts-api-openapi.yml
  format: yaml
  label: Tenor Posts API
  slug: tenor-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenor/refs/heads/main/openapi/tenor-posts-api-openapi.yml
- filename: tenor-registershare-api-openapi.yml
  format: yaml
  label: Tenor Registershare API
  slug: tenor-registershare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenor/refs/heads/main/openapi/tenor-registershare-api-openapi.yml
- filename: tenor-search-api-openapi.yml
  format: yaml
  label: Tenor Search API
  slug: tenor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenor/refs/heads/main/openapi/tenor-search-api-openapi.yml
- filename: tenor-search-suggestions-api-openapi.yml
  format: yaml
  label: Tenor Search Suggestions API
  slug: tenor-search-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenor/refs/heads/main/openapi/tenor-search-suggestions-api-openapi.yml
- filename: tenor-trending-terms-api-openapi.yml
  format: yaml
  label: Tenor Trending Terms API
  slug: tenor-trending-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenor/refs/heads/main/openapi/tenor-trending-terms-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tenor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Tenor exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tenor
provider_slug: tenor
slug: tenor-agentic-access
source_filename: tenor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /featured\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /search_suggestions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocomplete\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trending_terms\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registershare\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenor/refs/heads/main/agentic-access/tenor-agentic-access.yml
summary_line: 8 operations
tags:
- GIFs
- Animated Images
- Search
- Media
- Google
---
