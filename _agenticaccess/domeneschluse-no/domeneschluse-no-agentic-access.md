---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 15
api_specs:
- filename: domeneschluse-no-app-api-openapi.yml
  format: yaml
  label: Domeneschluse App API
  slug: domeneschluse-no-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-app-api-openapi.yml
- filename: domeneschluse-no-healthz-api-openapi.yml
  format: yaml
  label: Domeneschluse Healthz API
  slug: domeneschluse-no-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-healthz-api-openapi.yml
- filename: domeneschluse-no-historikk-api-openapi.yml
  format: yaml
  label: Domeneschluse Historikk API
  slug: domeneschluse-no-historikk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-historikk-api-openapi.yml
- filename: domeneschluse-no-koble-til-api-openapi.yml
  format: yaml
  label: Domeneschluse Koble Til API
  slug: domeneschluse-no-koble-til-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-koble-til-api-openapi.yml
- filename: domeneschluse-no-mcp-api-openapi.yml
  format: yaml
  label: Domeneschluse MCP API
  slug: domeneschluse-no-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-mcp-api-openapi.yml
- filename: domeneschluse-no-samtykke-api-openapi.yml
  format: yaml
  label: Domeneschluse Samtykke API
  slug: domeneschluse-no-samtykke-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-samtykke-api-openapi.yml
- filename: domeneschluse-no-well-known-api-openapi.yml
  format: yaml
  label: Domeneschluse .well Known API
  slug: domeneschluse-no-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-well-known-api-openapi.yml
consequence_counts:
  read: 15
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Domeneschluse No Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Domeneschluse exposes 22 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Domeneschluse
provider_slug: domeneschluse-no
slug: domeneschluse-no-agentic-access
source_filename: domeneschluse-no-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/domeneschluse-no-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 15\n    acting: 7\n  by_consequence:\n    read: 15\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  operationId: healthz_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: prm__well_known_oauth_protected_resource_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /koble-til\n  method: get\n  operationId: koble_til_side_koble_til_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /samtykke\n  method: get\n  operationId: samtykke_side_samtykke_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app\n  method: get\n  operationId: app_dashboard_app_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/historikk\n  method: get\n  operationId: app_historikk_app_historikk_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/tilkobling\n  method: get\n  operationId: app_tilkobling_app_tilkobling_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/tilkobling/data\n  method: get\n  operationId: tilkobling_data_app_tilkobling_data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/tilkobling/api-noekkel\n  method: post\n  operationId: tilkobling_api_noekkel_app_tilkobling_api_noekkel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/tilkobling/api-noekkel/fjern\n  method: post\n  operationId: tilkobling_api_noekkel_fjern_app_tilkobling_api_noekkel_fjern_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/tilkobling/koble-fra\n  method: post\n  operationId: tilkobling_koble_fra_app_tilkobling_koble_fra_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/tall\n  method: get\n  operationId: app_tall_app_tall_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/tall/data\n  method: get\n  operationId: app_tall_data_app_tall_data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/konto\n  method: get\n  operationId: app_konto_app_konto_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historikk/trace/{trace_id}\n  method: get\n  operationId: trace_detalj_historikk_trace__trace_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historikk\n  method: get\n  operationId: historikk_redirect_historikk_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historikk/data\n  method: get\n  operationId: historikk_data_historikk_data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /koble-til/sjekk\n  method: post\n  operationId: koble_til_sjekk_koble_til_sjekk_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /koble-til/verifiser\n  method: post\n  operationId: koble_til_verifiser_koble_til_verifiser_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcp_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId:\
  \ mcp_mcp_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: delete\n  operationId: mcp_mcp_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/domeneschluse-no/agentic-access/domeneschluse-no-agentic-access.yml
summary_line: 22 operations · 7 acting
tags:
- Company
- Email
- Artificial Intelligence
- MCP
- Open Source
- Privacy
---
