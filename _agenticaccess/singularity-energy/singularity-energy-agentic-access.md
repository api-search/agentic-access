---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Carbon Intensity API
  slug: carbon-intensity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Forecasts API
  slug: forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Generation & Event Data API
  slug: generation-event-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Regions API
  slug: regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
consequence_counts:
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Singularity Energy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Singularity exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Singularity
provider_slug: singularity-energy
slug: singularity-energy-agentic-access
source_filename: singularity-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/singularity-energy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/region_events/search\n  method: get\n  operationId: searchRegionEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/region_events/{region_or_postal_code}/latest\n  method: get\n  operationId: latestRegionEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/region_events/{dedup_key}\n  method: get\n  operationId: findRegionEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/region_events/bulk-find\n  method: post\n  operationId: findAllRegionEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/emissions/all-factors\n  method: get\n  operationId: getAllEmissionFactors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/emissions/calculate-intensity/generated\n  method: post\n  operationId: calculateGeneratedCarbonIntensity\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/emissions/calculate-intensity/marginal\n  method: post\n  operationId: calculateMarginalCarbonIntensity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/interchange\n  method: get\n  operationId: getInterchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/interchange/latest\n  method: get\n  operationId: getLatestInterchange\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/agentic-access/singularity-energy-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Energy
- Carbon Emissions
- Grid
- Sustainability
- Carbon Intensity
---
