---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: energy-information-administration-co2-emissions-api-openapi.yml
  format: yaml
  label: Energy Information Administration CO2 Emissions API
  slug: energy-information-administration-co2-emissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-co2-emissions-api-openapi.yml
- filename: energy-information-administration-coal-api-openapi.yml
  format: yaml
  label: Energy Information Administration Coal API
  slug: energy-information-administration-coal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-coal-api-openapi.yml
- filename: energy-information-administration-discovery-api-openapi.yml
  format: yaml
  label: Energy Information Administration Discovery API
  slug: energy-information-administration-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-discovery-api-openapi.yml
- filename: energy-information-administration-electricity-api-openapi.yml
  format: yaml
  label: Energy Information Administration Electricity API
  slug: energy-information-administration-electricity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-electricity-api-openapi.yml
- filename: energy-information-administration-international-api-openapi.yml
  format: yaml
  label: Energy Information Administration International API
  slug: energy-information-administration-international-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-international-api-openapi.yml
- filename: energy-information-administration-natural-gas-api-openapi.yml
  format: yaml
  label: Energy Information Administration Natural Gas API
  slug: energy-information-administration-natural-gas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-natural-gas-api-openapi.yml
- filename: energy-information-administration-nuclear-api-openapi.yml
  format: yaml
  label: Energy Information Administration Nuclear API
  slug: energy-information-administration-nuclear-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-nuclear-api-openapi.yml
- filename: energy-information-administration-petroleum-api-openapi.yml
  format: yaml
  label: Energy Information Administration Petroleum API
  slug: energy-information-administration-petroleum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-petroleum-api-openapi.yml
- filename: energy-information-administration-seds-api-openapi.yml
  format: yaml
  label: Energy Information Administration SEDS API
  slug: energy-information-administration-seds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-seds-api-openapi.yml
- filename: energy-information-administration-total-energy-api-openapi.yml
  format: yaml
  label: Energy Information Administration Total Energy API
  slug: energy-information-administration-total-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-total-energy-api-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Energy Information Administration Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Energy Information Administration exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Energy Information Administration
provider_slug: energy-information-administration
slug: energy-information-administration-agentic-access
source_filename: energy-information-administration-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/energy-information-administration-open-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /electricity\n  method: get\n  operationId: getElectricityRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /electricity/retail-sales/data\n  method:\
  \ get\n  operationId: getElectricityRetailSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /natural-gas\n  method: get\n  operationId: getNaturalGasRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /natural-gas/pri/sum/data\n  method: get\n  operationId: getNaturalGasPriceSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /petroleum\n  method: get\n  operationId: getPetroleumRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /petroleum/pri/gnd/data\n  method: get\n  operationId: getPetroleumGasolineDieselPrices\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coal\n  method: get\n  operationId: getCoalRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nuclear-outages\n  method: get\n  operationId: getNuclearOutagesRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /total-energy/data\n  method: get\n  operationId: getTotalEnergy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /international\n  method: get\n  operationId: getInternationalRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /seds/data\n\
  \  method: get\n  operationId: getStateEnergyData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2-emissions/co2-emissions-aggregates/data\n  method: get\n  operationId: getCO2EmissionsAggregates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/agentic-access/energy-information-administration-agentic-access.yml
summary_line: 13 operations
tags:
- Energy
- Federal-Government
- Open Data
---
