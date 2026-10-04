---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 24
api_specs:
- filename: goatcounter-exports-api-openapi.yml
  format: yaml
  label: GoatCounter Exports API
  slug: goatcounter-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-exports-api-openapi.yml
- filename: goatcounter-pageviews-api-openapi.yml
  format: yaml
  label: GoatCounter Pageviews API
  slug: goatcounter-pageviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-pageviews-api-openapi.yml
- filename: goatcounter-paths-api-openapi.yml
  format: yaml
  label: GoatCounter Paths API
  slug: goatcounter-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-paths-api-openapi.yml
- filename: goatcounter-sites-api-openapi.yml
  format: yaml
  label: GoatCounter Sites API
  slug: goatcounter-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-sites-api-openapi.yml
- filename: goatcounter-statistics-api-openapi.yml
  format: yaml
  label: GoatCounter Statistics API
  slug: goatcounter-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-statistics-api-openapi.yml
- filename: goatcounter-users-api-openapi.yml
  format: yaml
  label: GoatCounter Users API
  slug: goatcounter-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-users-api-openapi.yml
- filename: goatcounter-count-api-openapi.yml
  format: yaml
  label: GoatCounter Count API
  slug: goatcounter-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-count-api-openapi.yml
- filename: goatcounter-export-api-openapi.yml
  format: yaml
  label: GoatCounter Export API
  slug: goatcounter-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-export-api-openapi.yml
- filename: goatcounter-stats-api-openapi.yml
  format: yaml
  label: GoatCounter Stats API
  slug: goatcounter-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-stats-api-openapi.yml
consequence_counts:
  read: 24
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Goatcounter Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'GoatCounter exposes 32 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoatCounter
provider_slug: goatcounter
slug: goatcounter-agentic-access
source_filename: goatcounter-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/goatcounter-count-api-openapi.yml, openapi/goatcounter-export-api-openapi.yml,\n  openapi/goatcounter-exports-api-openapi.yml, openapi/goatcounter-pageviews-api-openapi.yml,\n  openapi/goatcounter-paths-api-openapi.yml, openapi/goatcounter-sites-api-openapi.yml, openapi/goatcounter-statistics-api-openapi.yml,\n  openapi/goatcounter-stats-api-openapi.yml, openapi/goatcounter-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 24\n    acting: 8\n  by_consequence:\n    read: 24\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v0/count\n  method: post\n  operationId: POST_api_v0_count\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/export\n  method: post\n  operationId: POST_api_v0_export\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0/export/{id}\n  method: get\n  operationId: GET_api_v0_export_{id}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/export/{id}/download\n  method: get\n  operationId: GET_api_v0_export_{id}_download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export\n  method: post\n  operationId:\
  \ createExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /export/{id}\n  method: get\n  operationId: getExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/{id}/download\n  method: get\n  operationId: downloadExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /count\n  method: post\n  operationId: count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/paths\n  method: get\n  operationId: GET_api_v0_paths\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paths\n  method: get\n  operationId: listPaths\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/sites\n  method: get\n  operationId: GET_api_v0_sites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/sites\n  method: put\n  operationId: PUT_api_v0_sites\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0/sites/{id}\n  method: get\n  operationId: GET_api_v0_sites_{id}\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/sites/{id}\n  method: post\n  operationId: POST_api_v0_sites_{id}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0/sites/{id}\n  method: patch\n  operationId: PATCH_api_v0_sites_{id}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /sites\n  method: put\n  operationId: createSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{id}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{id}\n  method: post\n  operationId: updateSitePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{id}\n  method: patch\n  operationId: patchSite\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/total\n  method: get\n  operationId: statsTotal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/hits\n  method: get\n  operationId: statsHits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/hits/{path_id}\n  method: get\n  operationId: statsHitsRefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/{page}\n  method: get\n  operationId: statsByPage\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/{page}/{id}\n  method: get\n  operationId: statsByPageDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/stats/hits\n  method: get\n  operationId: GET_api_v0_stats_hits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/stats/hits/{path_id}\n  method: get\n  operationId: GET_api_v0_stats_hits_{path_id}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/stats/total\n  method: get\n  operationId: GET_api_v0_stats_total\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/stats/{page}\n  method: get\n  operationId: GET_api_v0_stats_{page}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/stats/{page}/{id}\n  method: get\n  operationId: GET_api_v0_stats_{page}_{id}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/me\n  method: get\n  operationId: GET_api_v0_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/agentic-access/goatcounter-agentic-access.yml
summary_line: 32 operations · 8 acting
tags:
- Analytics
- Page Views
- Privacy
- Statistics
- Web Analytics
- Open Source
- Self-Hosted
- Event
- Data Export
- Developer Tools
---
