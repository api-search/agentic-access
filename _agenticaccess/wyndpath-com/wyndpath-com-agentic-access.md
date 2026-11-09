---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 10
api_specs:
- filename: wyndpath-com-account-api-openapi.yml
  format: yaml
  label: wyndpath-com Account API
  slug: wyndpath-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-account-api-openapi.yml
- filename: wyndpath-com-charge-api-openapi.yml
  format: yaml
  label: wyndpath-com Charge API
  slug: wyndpath-com-charge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-charge-api-openapi.yml
- filename: wyndpath-com-estimate-api-openapi.yml
  format: yaml
  label: wyndpath-com Estimate API
  slug: wyndpath-com-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-estimate-api-openapi.yml
- filename: wyndpath-com-geo-api-openapi.yml
  format: yaml
  label: wyndpath-com Geo API
  slug: wyndpath-com-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-geo-api-openapi.yml
- filename: wyndpath-com-healthz-api-openapi.yml
  format: yaml
  label: wyndpath-com Healthz API
  slug: wyndpath-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-healthz-api-openapi.yml
- filename: wyndpath-com-internal-api-openapi.yml
  format: yaml
  label: wyndpath-com Internal API
  slug: wyndpath-com-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-internal-api-openapi.yml
- filename: wyndpath-com-profiles-api-openapi.yml
  format: yaml
  label: wyndpath-com Profiles API
  slug: wyndpath-com-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-profiles-api-openapi.yml
- filename: wyndpath-com-requests-api-openapi.yml
  format: yaml
  label: wyndpath-com Requests API
  slug: wyndpath-com-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-requests-api-openapi.yml
- filename: wyndpath-com-stats-api-openapi.yml
  format: yaml
  label: wyndpath-com Stats API
  slug: wyndpath-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-stats-api-openapi.yml
- filename: wyndpath-com-target-api-openapi.yml
  format: yaml
  label: wyndpath-com Target API
  slug: wyndpath-com-target-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-target-api-openapi.yml
- filename: wyndpath-com-wyndpath-api-openapi.yml
  format: yaml
  label: wyndpath-com Wynd Path API
  slug: wyndpath-com-wyndpath-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wyndpath-com/openapi/wyndpath-com-wyndpath-api-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wyndpath Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/internal/charge
operation_count: 12
overview: 'wyndpath-com exposes 12 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: wyndpath-com
provider_slug: wyndpath-com
slug: wyndpath-com-agentic-access
source_filename: wyndpath-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/wyndpath-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 10\n    acting: 2\n  by_consequence:\n    read: 10\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  operationId: healthz_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/\n  method: get\n  operationId: proxy_v1__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/\n  method: post\n\
  \  operationId: proxy_v1__get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/stats\n  method: get\n  operationId: stats_v1_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/requests\n  method: get\n  operationId: requests_viewer_v1_requests_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/target\n  method: get\n  operationId: target_info_v1_target_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles\n\
  \  method: get\n  operationId: profiles_view_v1_profiles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geo\n  method: get\n  operationId: geo_coverage_v1_geo_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/estimate\n  method: get\n  operationId: estimate_v1_estimate_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/charge\n  method: get\n  operationId: charge_view_v1_charge_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: account_view_v1_account_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/internal/charge\n  method: post\n  operationId: internal_charge_v1_internal_charge_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/wyndpath-com/agentic-access/wyndpath-com-agentic-access.yml
summary_line: 12 operations · 2 acting
tags:
- Company
- Web Scraping
- Data
- Automation
- Web
---
