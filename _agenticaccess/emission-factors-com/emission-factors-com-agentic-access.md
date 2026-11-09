---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 13
api_specs:
- filename: emission-factors-com-bulk-api-openapi.yml
  format: yaml
  label: emission-factors-com Bulk API
  slug: emission-factors-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-bulk-api-openapi.yml
- filename: emission-factors-com-calculate-api-openapi.yml
  format: yaml
  label: emission-factors-com Calculate API
  slug: emission-factors-com-calculate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-calculate-api-openapi.yml
- filename: emission-factors-com-cleanest-hours-api-openapi.yml
  format: yaml
  label: emission-factors-com Cleanest Hours API
  slug: emission-factors-com-cleanest-hours-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-cleanest-hours-api-openapi.yml
- filename: emission-factors-com-compare-api-openapi.yml
  format: yaml
  label: emission-factors-com Compare API
  slug: emission-factors-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-compare-api-openapi.yml
- filename: emission-factors-com-fuel-emissions-api-openapi.yml
  format: yaml
  label: emission-factors-com Fuel Emissions API
  slug: emission-factors-com-fuel-emissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-fuel-emissions-api-openapi.yml
- filename: emission-factors-com-health-api-openapi.yml
  format: yaml
  label: emission-factors-com Health API
  slug: emission-factors-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-health-api-openapi.yml
- filename: emission-factors-com-intensity-api-openapi.yml
  format: yaml
  label: emission-factors-com Intensity API
  slug: emission-factors-com-intensity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-intensity-api-openapi.yml
- filename: emission-factors-com-lookup-api-openapi.yml
  format: yaml
  label: emission-factors-com Lookup API
  slug: emission-factors-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-lookup-api-openapi.yml
- filename: emission-factors-com-mcp-api-openapi.yml
  format: yaml
  label: emission-factors-com MCP API
  slug: emission-factors-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-mcp-api-openapi.yml
- filename: emission-factors-com-methodology-api-openapi.yml
  format: yaml
  label: emission-factors-com Methodology API
  slug: emission-factors-com-methodology-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-methodology-api-openapi.yml
- filename: emission-factors-com-openapi-json-api-openapi.yml
  format: yaml
  label: emission-factors-com Openapi.json API
  slug: emission-factors-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-openapi-json-api-openapi.yml
- filename: emission-factors-com-plant-emissions-api-openapi.yml
  format: yaml
  label: emission-factors-com Plant Emissions API
  slug: emission-factors-com-plant-emissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-plant-emissions-api-openapi.yml
- filename: emission-factors-com-rate-api-openapi.yml
  format: yaml
  label: emission-factors-com Rate API
  slug: emission-factors-com-rate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-rate-api-openapi.yml
- filename: emission-factors-com-status-api-openapi.yml
  format: yaml
  label: emission-factors-com Status API
  slug: emission-factors-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-status-api-openapi.yml
- filename: emission-factors-com-utility-rate-api-openapi.yml
  format: yaml
  label: emission-factors-com Utility Rate API
  slug: emission-factors-com-utility-rate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emission-factors-com/openapi/emission-factors-com-utility-rate-api-openapi.yml
consequence_counts:
  read: 13
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Emission Factors Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'emission-factors-com exposes 18 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: emission-factors-com
provider_slug: emission-factors-com
slug: emission-factors-com-agentic-access
source_filename: emission-factors-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/emission-factors-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 13\n    acting: 5\n  by_consequence:\n    read: 13\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/lookup\n  method: get\n  operationId: lookupByZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lookup/by-coordinates\n  method: get\n  operationId: lookupByCoordinates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lookup/batch\n\
  \  method: post\n  operationId: lookupBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calculate\n  method: post\n  operationId: calculate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/bulk\n  method: post\n  operationId: bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rate\n  method: get\n  operationId: retailRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/intensity\n  method: get\n  operationId: hourlyIntensity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/plant-emissions\n  method: get\n  operationId: plantEmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/utility-rate\n  method: get\n  operationId: utilityTariff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/compare\n  method: post\n  operationId: compareSites\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cleanest-hours\n  method: get\n  operationId: cleanestHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fuel-emissions\n  method: get\n  operationId: fuelEmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fuel-emissions\n  method: post\n  operationId: fuelEmissionsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /methodology\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/emission-factors-com/agentic-access/emission-factors-com-agentic-access.yml
summary_line: 18 operations · 5 acting
tags:
- Company
- Emission
- Carbon
- Energy
- Sustainability
---
