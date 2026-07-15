---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: octopus-energy-public-api-openapi.yml
  format: yaml
  label: Octopus Energy Public API
  slug: octopus-energy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-energy/refs/heads/main/openapi/octopus-energy-public-api-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Octopus Energy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Octopus Energy exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Octopus Energy
provider_slug: octopus-energy
slug: octopus-energy-agentic-access
source_filename: octopus-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/octopus-energy-public-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /products/\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_code}/\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_code}/electricity-tariffs/{tariff_code}/standard-unit-rates/\n\
  \  method: get\n  operationId: listElectricityStandardUnitRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_code}/electricity-tariffs/{tariff_code}/standing-charges/\n  method: get\n  operationId: listElectricityStandingCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_code}/electricity-tariffs/{tariff_code}/day-unit-rates/\n  method: get\n  operationId: listElectricityDayUnitRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_code}/electricity-tariffs/{tariff_code}/night-unit-rates/\n  method: get\n  operationId: listElectricityNightUnitRates\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_code}/gas-tariffs/{tariff_code}/standard-unit-rates/\n  method: get\n  operationId: listGasStandardUnitRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_code}/gas-tariffs/{tariff_code}/standing-charges/\n  method: get\n  operationId: listGasStandingCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /electricity-meter-points/{mpan}/\n  method: get\n  operationId: getElectricityMeterPoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /electricity-meter-points/{mpan}/meters/{serial_number}/consumption/\n  method: get\n  operationId: listElectricityConsumption\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gas-meter-points/{mprn}/\n  method: get\n  operationId: getGasMeterPoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gas-meter-points/{mprn}/meters/{serial_number}/consumption/\n  method: get\n  operationId: listGasConsumption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /industry/grid-supply-points/\n  method: get\n  operationId: listGridSupplyPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octopus-energy/refs/heads/main/agentic-access/octopus-energy-agentic-access.yml
summary_line: 13 operations
tags:
- Energy
- Electricity
- Gas
- Renewable Energy
- Smart Meter
- Tariffs
- Kraken
- UK
- DER
- Electric Vehicles
- Heat Pumps
- Solar
- Battery
---
