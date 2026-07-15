---
acting_count: 0
action_class_counts:
  connected: 27
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Carbon Intensity API
  slug: carbon-intensity-api
  spec_type: OpenAPI
  url: https://carbon-intensity.github.io/api-definitions/
consequence_counts:
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Carbon Intensity Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Carbon Intensity API exposes 27 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Carbon Intensity API
provider_slug: carbon-intensity
slug: carbon-intensity-agentic-access
source_filename: carbon-intensity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/carbon-intensity-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 27\n  by_consequence:\n    read: 27\n  human_in_the_loop_required: 0\noperations:\n- path: /intensity\n  method: get\n  operationId: getCurrentIntensity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/date\n  method: get\n  operationId: getIntensityForToday\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/date/{date}\n  method: get\n  operationId:\
  \ getIntensityByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/date/{date}/{period}\n  method: get\n  operationId: getIntensityByDateAndPeriod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/factors\n  method: get\n  operationId: getIntensityFactors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/{from}\n  method: get\n  operationId: getIntensityFrom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/{from}/fw24h\n  method: get\n  operationId: getIntensityForward24h\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/{from}/fw48h\n  method: get\n  operationId: getIntensityForward48h\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/{from}/pt24h\n  method: get\n  operationId: getIntensityPast24h\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/{from}/{to}\n  method: get\n  operationId: getIntensityRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intensity/stats/{from}/{to}\n  method: get\n  operationId: getIntensityStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /intensity/stats/{from}/{to}/{block}\n  method: get\n  operationId: getIntensityStatsBlocked\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generation\n  method: get\n  operationId: getCurrentGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generation/{from}/{to}\n  method: get\n  operationId: getGenerationRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional\n  method: get\n  operationId: getAllRegionsIntensity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/england\n  method: get\n  operationId: getEnglandIntensity\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/scotland\n  method: get\n  operationId: getScotlandIntensity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/wales\n  method: get\n  operationId: getWalesIntensity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/postcode/{postcode}\n  method: get\n  operationId: getIntensityByPostcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/regionid/{regionid}\n  method: get\n  operationId: getIntensityByRegionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/{from}/{to}\n  method: get\n  operationId: getRegionalIntensityRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/intensity/{from}/fw24h/postcode/{postcode}\n  method: get\n  operationId: getRegionalForward24hByPostcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/intensity/{from}/fw24h/regionid/{regionid}\n  method: get\n  operationId: getRegionalForward24hByRegionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/intensity/{from}/fw48h/postcode/{postcode}\n  method: get\n  operationId: getRegionalForward48hByPostcode\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/intensity/{from}/fw48h/regionid/{regionid}\n  method: get\n  operationId: getRegionalForward48hByRegionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/intensity/{from}/pt24h/postcode/{postcode}\n  method: get\n  operationId: getRegionalPast24hByPostcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regional/intensity/{from}/pt24h/regionid/{regionid}\n  method: get\n  operationId: getRegionalPast24hByRegionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbon-intensity/refs/heads/main/agentic-access/carbon-intensity-agentic-access.yml
summary_line: 27 operations
tags:
- Carbon Intensity
- Environment
- Energy
- Electricity
- Climate
- Great Britain
- National Grid
---
