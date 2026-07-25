---
acting_count: 17
action_class_counts:
  acting: 17
api_specs:
- filename: igdb-companies-api-openapi.yml
  format: yaml
  label: IGDB Companies API
  slug: igdb-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-companies-api-openapi.yml
- filename: igdb-games-api-openapi.yml
  format: yaml
  label: IGDB Games API
  slug: igdb-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-games-api-openapi.yml
- filename: igdb-genres-api-openapi.yml
  format: yaml
  label: IGDB Genres API
  slug: igdb-genres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-genres-api-openapi.yml
- filename: igdb-media-api-openapi.yml
  format: yaml
  label: IGDB Media API
  slug: igdb-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-media-api-openapi.yml
- filename: igdb-platforms-api-openapi.yml
  format: yaml
  label: IGDB Platforms API
  slug: igdb-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-platforms-api-openapi.yml
- filename: igdb-reference-api-openapi.yml
  format: yaml
  label: IGDB Reference API
  slug: igdb-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-reference-api-openapi.yml
- filename: igdb-releases-api-openapi.yml
  format: yaml
  label: IGDB Releases API
  slug: igdb-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-releases-api-openapi.yml
- filename: igdb-search-api-openapi.yml
  format: yaml
  label: IGDB Search API
  slug: igdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-search-api-openapi.yml
consequence_counts:
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Igdb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'IGDB exposes 17 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IGDB
provider_slug: igdb
slug: igdb-agentic-access
source_filename: igdb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/igdb-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 17\n  by_consequence:\n    write: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /games\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platforms\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /involved_companies\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genres\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /themes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /game_modes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /covers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /screenshots\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artworks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /release_dates\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections\n  method: post\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /franchises\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keywords\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /age_ratings\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /websites\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/agentic-access/igdb-agentic-access.yml
summary_line: 17 operations · 17 acting
tags:
- Entertainment
- Game Database
- Gaming
- Video Games
---
