---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: tppflow-com-cbp-api-openapi.yml
  format: yaml
  label: tppflow-com Cbp API
  slug: tppflow-com-cbp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-cbp-api-openapi.yml
- filename: tppflow-com-faa-api-openapi.yml
  format: yaml
  label: tppflow-com Faa API
  slug: tppflow-com-faa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-faa-api-openapi.yml
- filename: tppflow-com-fcc-api-openapi.yml
  format: yaml
  label: tppflow-com Fcc API
  slug: tppflow-com-fcc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-fcc-api-openapi.yml
- filename: tppflow-com-fda-api-openapi.yml
  format: yaml
  label: tppflow-com Fda API
  slug: tppflow-com-fda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-fda-api-openapi.yml
- filename: tppflow-com-meta-api-openapi.yml
  format: yaml
  label: tppflow-com Meta API
  slug: tppflow-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-meta-api-openapi.yml
- filename: tppflow-com-nppes-api-openapi.yml
  format: yaml
  label: tppflow-com Nppes API
  slug: tppflow-com-nppes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-nppes-api-openapi.yml
- filename: tppflow-com-rrc-api-openapi.yml
  format: yaml
  label: tppflow-com Rrc API
  slug: tppflow-com-rrc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-rrc-api-openapi.yml
- filename: tppflow-com-toll-api-openapi.yml
  format: yaml
  label: tppflow-com Toll API
  slug: tppflow-com-toll-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-toll-api-openapi.yml
- filename: tppflow-com-usda-api-openapi.yml
  format: yaml
  label: tppflow-com Usda API
  slug: tppflow-com-usda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-usda-api-openapi.yml
- filename: tppflow-com-warn-api-openapi.yml
  format: yaml
  label: tppflow-com Warn API
  slug: tppflow-com-warn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tppflow-com/openapi/tppflow-com-warn-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tppflow Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'tppflow-com exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tppflow-com
provider_slug: tppflow-com
slug: tppflow-com-agentic-access
source_filename: tppflow-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/tppflow-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/warn/notices\n  method: get\n  operationId: notices_api_v1_warn_notices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/warn/stats\n  method: get\n \
  \ operationId: stats_api_v1_warn_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rrc/describe_layout\n  method: get\n  operationId: describe_layout_api_v1_rrc_describe_layout_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rrc/wellbores\n  method: get\n  operationId: wellbores_api_v1_rrc_wellbores_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rrc/stats\n  method: get\n  operationId: stats_api_v1_rrc_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /toll/claim\n  method: get\n  operationId: claim_toll_claim_get\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/faa/aircraft/{n_number}\n  method: get\n  operationId: aircraft_api_v1_faa_aircraft__n_number__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/faa/aircraft\n  method: get\n  operationId: search_aircraft_api_v1_faa_aircraft_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fcc/licenses\n  method: get\n  operationId: licenses_api_v1_fcc_licenses_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fcc/licenses/{callsign}\n  method: get\n  operationId: licence_api_v1_fcc_licenses__callsign__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/nppes/providers/{npi}\n  method: get\n  operationId: provider_api_v1_nppes_providers__npi__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/nppes/providers\n  method: get\n  operationId: search_providers_api_v1_nppes_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fda/shortages\n  method: get\n  operationId: shortages_api_v1_fda_shortages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usda/terminal\n  method: get\n  operationId: terminal_api_v1_usda_terminal_get\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cbp/waits\n  method: get\n  operationId: waits_api_v1_cbp_waits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tppflow-com/agentic-access/tppflow-com-agentic-access.yml
summary_line: 16 operations
tags:
- Company
- Data
- Analytics
---
