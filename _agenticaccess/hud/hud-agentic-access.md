---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: hud-fair-market-rents-openapi.yml
  format: yaml
  label: HUD User Fair Market Rents API
  slug: hud-user-fair-market-rents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-fair-market-rents-openapi.yml
- filename: hud-income-limits-openapi.yml
  format: yaml
  label: HUD User Income Limits API
  slug: hud-user-income-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-income-limits-openapi.yml
- filename: hud-usps-zip-code-crosswalk-openapi.yml
  format: yaml
  label: HUD User USPS ZIP Code Crosswalk API
  slug: hud-user-usps-zip-code-crosswalk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-usps-zip-code-crosswalk-openapi.yml
- filename: hud-chas-openapi.yml
  format: yaml
  label: HUD User CHAS API
  slug: hud-user-chas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-chas-openapi.yml
- filename: hud-housing-counselor-search-openapi.yml
  format: yaml
  label: HUD Housing Counselor Search API
  slug: hud-housing-counselor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-housing-counselor-search-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hud Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'HUD - US Department of Housing and Urban Development exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HUD - US Department of Housing and Urban Development
provider_slug: hud
slug: hud-agentic-access
source_filename: hud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hud-chas-openapi.yml, openapi/hud-fair-market-rents-openapi.yml, openapi/hud-housing-counselor-search-openapi.yml,\n  openapi/hud-income-limits-openapi.yml, openapi/hud-usps-zip-code-crosswalk-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /chas\n  method: get\n  operationId: getCHASData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fmr/statedata/{state}\n  method: get\n  operationId: getFMRByState\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fmr/data/{entityid}\n  method: get\n  operationId: getFMRByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Housing_Counselor/search\n  method: get\n  operationId: searchHousingCounselors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Housing_Counselor/searchByLocation\n  method: get\n  operationId: searchHousingCounselorsByLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /il/data/{entityid}\n  method: get\n  operationId: getIncomeLimitsByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /il/statedata/{state}\n  method: get\n  operationId: getIncomeLimitsByState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usps\n  method: get\n  operationId: getZIPCrosswalk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/agentic-access/hud-agentic-access.yml
summary_line: 8 operations
tags:
- Housing
- Government
- Fair Market Rent
- Mortgage
- Community Development
- Public Housing
- Section 8
- Income Limits
---
