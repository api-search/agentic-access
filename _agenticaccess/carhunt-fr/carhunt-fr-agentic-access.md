---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 8
api_specs:
- filename: carhunt-fr-analyses-api-openapi.yml
  format: yaml
  label: CarHunt Analyses API
  slug: carhunt-fr-analyses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-analyses-api-openapi.yml
- filename: carhunt-fr-compte-api-openapi.yml
  format: yaml
  label: CarHunt Compte API
  slug: carhunt-fr-compte-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-compte-api-openapi.yml
- filename: carhunt-fr-march-api-openapi.yml
  format: yaml
  label: CarHunt Marché API
  slug: carhunt-fr-march-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-march-api-openapi.yml
- filename: carhunt-fr-recherche-api-openapi.yml
  format: yaml
  label: CarHunt Recherche API
  slug: carhunt-fr-recherche-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-recherche-api-openapi.yml
- filename: carhunt-fr-synchronisation-api-openapi.yml
  format: yaml
  label: CarHunt Synchronisation API
  slug: carhunt-fr-synchronisation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-synchronisation-api-openapi.yml
- filename: carhunt-fr-watchlists-api-openapi.yml
  format: yaml
  label: CarHunt Watchlists API
  slug: carhunt-fr-watchlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carhunt-fr/openapi/carhunt-fr-watchlists-api-openapi.yml
consequence_counts:
  read: 8
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Carhunt Fr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'CarHunt exposes 12 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CarHunt
provider_slug: carhunt-fr
slug: carhunt-fr-agentic-access
source_filename: carhunt-fr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/carhunt-fr-pro-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 8\n    acting: 4\n  by_consequence:\n    read: 8\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/listings/search\n  method: get\n  operationId: search_listings_v1_listings_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/listings/resolve\n  method: get\n  operationId: resolve_listing_v1_listings_resolve_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/deals\n  method: get\n  operationId: deals_v1_deals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/listings/{listing_id}/market\n  method: get\n  operationId: listing_market_v1_listings__listing_id__market_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists\n  method: get\n  operationId: list_watchlists_v1_watchlists_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists\n  method: post\n\
  \  operationId: create_watchlist_v1_watchlists_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{watchlist_id}\n  method: patch\n  operationId: update_watchlist_v1_watchlists__watchlist_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{watchlist_id}\n  method: delete\n  operationId: delete_watchlist_v1_watchlists__watchlist_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/estimate\n  method: post\n  operationId: estimate_vehicle_v1_estimate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listings/{listing_id}/analysis\n  method: get\n  operationId: listing_analysis_v1_listings__listing_id__analysis_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/listings/changes\n  method: get\n  operationId: listing_changes_v1_listings_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://artifacts.apis.io/carhunt-fr/agentic-access/carhunt-fr-agentic-access.yml
summary_line: 12 operations · 4 acting
tags:
- Company
---
