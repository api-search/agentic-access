---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: geospatialsystem-com-catalogue-api-openapi.yml
  format: yaml
  label: geospatialsystem-com Catalogue API
  slug: geospatialsystem-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geospatialsystem-com/openapi/geospatialsystem-com-catalogue-api-openapi.yml
- filename: geospatialsystem-com-level-1-pixel-api-openapi.yml
  format: yaml
  label: geospatialsystem-com Level 1 — Pixel API
  slug: geospatialsystem-com-level-1-pixel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geospatialsystem-com/openapi/geospatialsystem-com-level-1-pixel-api-openapi.yml
- filename: geospatialsystem-com-level-2-neighbourhood-api-openapi.yml
  format: yaml
  label: geospatialsystem-com Level 2 — Neighbourhood API
  slug: geospatialsystem-com-level-2-neighbourhood-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geospatialsystem-com/openapi/geospatialsystem-com-level-2-neighbourhood-api-openapi.yml
- filename: geospatialsystem-com-level-3-area-maps-api-openapi.yml
  format: yaml
  label: geospatialsystem-com Level 3 — Area Maps API
  slug: geospatialsystem-com-level-3-area-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geospatialsystem-com/openapi/geospatialsystem-com-level-3-area-maps-api-openapi.yml
consequence_counts:
  read: 8
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Geospatialsystem Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'geospatialsystem-com exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: geospatialsystem-com
provider_slug: geospatialsystem-com
slug: geospatialsystem-com-agentic-access
source_filename: geospatialsystem-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/geospatialsystem-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 8\n    acting: 8\n  by_consequence:\n    read: 8\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /datasets\n  method: get\n  operationId: list_datasets_datasets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lp/elevation\n  method: get\n  operationId: lp_get_elevation_lp_elevation_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /lp/elevation\n  method: post\n  operationId: lp_post_elevation_lp_elevation_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lp/elevation/batch\n  method: post\n  operationId: lp_elevation_batch_lp_elevation_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lp/elevation_stats\n  method: get\n  operationId: lp_get_elevation_stats_lp_elevation_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /lp/elevation_stats\n  method: post\n  operationId: lp_post_elevation_stats_lp_elevation_stats_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lp/slope_stats\n  method: get\n  operationId: lp_get_slope_stats_lp_slope_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lp/slope_stats\n  method: post\n  operationId: lp_post_slope_stats_lp_slope_stats_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /lp/elevation_chart\n  method: get\n  operationId: lp_get_elevation_chart_lp_elevation_chart_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lp/elevation_chart\n  method: post\n  operationId: lp_post_elevation_chart_lp_elevation_chart_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lp/slope_chart\n  method: get\n  operationId: lp_get_slope_chart_lp_slope_chart_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lp/slope_chart\n  method: post\n  operationId: lp_post_slope_chart_lp_slope_chart_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lp/terrain_map\n  method: get\n  operationId: lp_get_terrain_map_lp_terrain_map_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lp/terrain_map\n  method: post\n  operationId: lp_post_terrain_map_lp_terrain_map_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lp/terrain_3d\n  method: get\n  operationId: lp_get_terrain_3d_lp_terrain_3d_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lp/terrain_3d\n  method: post\n  operationId: lp_post_terrain_3d_lp_terrain_3d_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/geospatialsystem-com/agentic-access/geospatialsystem-com-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Company
- Geospatial
- Terrain
- Artificial Intelligence
- Location
---
