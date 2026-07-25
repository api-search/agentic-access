---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: cornell-config-api-openapi.yml
  format: yaml
  label: Cornell University config API
  slug: cornell-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-config-api-openapi.yml
- filename: cornell-dining-api-openapi.yml
  format: yaml
  label: Cornell University dining API
  slug: cornell-dining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-dining-api-openapi.yml
- filename: cornell-events-api-openapi.yml
  format: yaml
  label: Cornell University events API
  slug: cornell-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-events-api-openapi.yml
- filename: cornell-location-api-openapi.yml
  format: yaml
  label: Cornell University location API
  slug: cornell-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-location-api-openapi.yml
- filename: cornell-map-items-api-openapi.yml
  format: yaml
  label: Cornell University map items API
  slug: cornell-map-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-map-items-api-openapi.yml
- filename: cornell-search-api-openapi.yml
  format: yaml
  label: Cornell University search API
  slug: cornell-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-search-api-openapi.yml
- filename: cornell-tags-api-openapi.yml
  format: yaml
  label: Cornell University tags API
  slug: cornell-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-tags-api-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cornell Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Cornell University exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cornell University
provider_slug: cornell
slug: cornell-agentic-access
source_filename: cornell-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cornell-codi-classes.yaml, openapi/cornell-codi-days.yaml, openapi/cornell-codi-dining.yaml,\n  openapi/cornell-codi-events.yaml, openapi/cornell-codi-map.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /config/rosters.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/acadCareers.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /config/acadGroups.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/classLevels.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/subjects.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/classes.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/pages.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dining/announcements.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dining/eateries.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations.cfm\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /overlay-items.cfm\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/agentic-access/cornell-agentic-access.yml
summary_line: 15 operations
tags:
- Education
- Higher Education
- University
- Open Data
- Course Catalog
- Library
- Research
- United States
---
