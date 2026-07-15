---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay Ports and Vessels API
  slug: sinay-ports-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay Metocean API
  slug: sinay-metocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay CO2 Emission API
  slug: sinay-co2-emission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay ETA API
  slug: sinay-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay Port Congestion API
  slug: sinay-port-congestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
consequence_counts:
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sinay Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Sinay exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sinay
provider_slug: sinay
slug: sinay-agentic-access
source_filename: sinay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sinay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 10\n    acting: 4\n  by_consequence:\n    read: 10\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /ports-vessels/api/v1/vessels\n  method: get\n  operationId: getVesselsByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ports-vessels/api/v1/ports\n  method: get\n  operationId: getPortsByNameOrCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /ports-vessels/api/v1/usages\n  method: get\n  operationId: getPortsVesselsUsages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metocean/api/v1/models\n  method: get\n  operationId: retrieveMetoceanModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metocean/api/v1/stations\n  method: post\n  operationId: retrieveMetoceanStations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metocean/api/v1/usages\n  method: get\n  operationId: getMetoceanUsages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /co2/api/v2/compute-co2\n  method: post\n  operationId: computeCo2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /co2/api/v2/usages\n  method: get\n  operationId: getCo2Usages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /etac/api/v1/compute-eta\n  method: post\n  operationId: computeEta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /etac/api/v1/usages\n\
  \  method: get\n  operationId: getEtaUsages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congestion/api/v1/congestion/{portCode}\n  method: get\n  operationId: retrieveCongestionAggregate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congestion/api/v1/congestion/batch\n  method: post\n  operationId: retrieveCongestionAggregateBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /congestion/api/v1/consumption/current-period\n  method: get\n  operationId: retrieveCurrentConsumptionPeriod\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congestion/api/v1/consumption/periods\n  method: get\n  operationId: retrieveConsumptionPeriods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/agentic-access/sinay-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Vessel Tracking
- AIS
- Maritime
- Maritime Data
- Weather
- CO2 Emissions
- Port Congestion
- Ship Tracking
- ETA
- Ocean Data
---
