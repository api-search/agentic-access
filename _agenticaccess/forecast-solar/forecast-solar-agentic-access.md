---
acting_count: 0
action_class_counts:
  connected: 56
api_specs:
- filename: forecast-solar-chart-api-openapi.yml
  format: yaml
  label: Forecast.Solar Chart API
  slug: forecast-solar-chart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecast-solar/openapi/forecast-solar-chart-api-openapi.yml
- filename: forecast-solar-clear-sky-api-openapi.yml
  format: yaml
  label: Forecast.Solar Clear sky API
  slug: forecast-solar-clear-sky-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecast-solar/openapi/forecast-solar-clear-sky-api-openapi.yml
- filename: forecast-solar-forecast-api-openapi.yml
  format: yaml
  label: Forecast.Solar Forecast API
  slug: forecast-solar-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecast-solar/openapi/forecast-solar-forecast-api-openapi.yml
- filename: forecast-solar-history-api-openapi.yml
  format: yaml
  label: Forecast.Solar History API
  slug: forecast-solar-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecast-solar/openapi/forecast-solar-history-api-openapi.yml
- filename: forecast-solar-misc-api-openapi.yml
  format: yaml
  label: Forecast.Solar Misc API
  slug: forecast-solar-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecast-solar/openapi/forecast-solar-misc-api-openapi.yml
- filename: forecast-solar-professional-api-openapi.yml
  format: yaml
  label: Forecast.Solar Professional API
  slug: forecast-solar-professional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecast-solar/openapi/forecast-solar-professional-api-openapi.yml
- filename: forecast-solar-public-api-openapi.yml
  format: yaml
  label: Forecast.Solar Public API
  slug: forecast-solar-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecast-solar/openapi/forecast-solar-public-api-openapi.yml
- filename: forecast-solar-weather-api-openapi.yml
  format: yaml
  label: Forecast.Solar Weather API
  slug: forecast-solar-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecast-solar/openapi/forecast-solar-weather-api-openapi.yml
consequence_counts:
  read: 56
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Forecast Solar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 56
overview: 'Forecast.Solar exposes 56 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 56 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Forecast.Solar
provider_slug: forecast-solar
slug: forecast-solar-agentic-access
source_filename: forecast-solar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/forecast-solar-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    connected: 56\n  by_consequence:\n    read: 56\n  human_in_the_loop_required: 0\noperations:\n- path: /help\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check/{lat}/{lon}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /swagger.yaml\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimate/{lat}/{lon}/{dec}/{az}/{kwp}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimate/watts/{lat}/{lon}/{dec}/{az}/{kwp}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimate/watthours/{lat}/{lon}/{dec}/{az}/{kwp}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimate/watthours/day/{lat}/{lon}/{dec}/{az}/{kwp}\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/watts/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/watts/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/watts/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/watthours/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/watthours/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/watthours/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/watthours/day/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/watthours/day/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/estimate/watthours/day/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/watts/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /{apikey}/history/watts/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/watts/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/watthours/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/watthours/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /{apikey}/history/watthours/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/watthours/day/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/watthours/day/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/history/watthours/day/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  operationId: clearsky1Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  operationId: clearsky2Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  operationId: clearsky3Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/watts/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  operationId: clearskyWatts1Get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/watts/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  operationId: clearskyWatts2Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/watts/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  operationId: clearskyWatts3Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/watthours/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  operationId: clearskyWatthours1Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/watthours/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n\
  \  method: get\n  operationId: clearskyWatthours2Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/watthours/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  operationId: clearskyWatthours3Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/watthours/day/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  operationId: clearskyWatthoursDay1Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/watthours/day/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  operationId: clearskyWatthoursDay2Get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/clearsky/watthours/day/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  operationId: clearskyWatthoursDay3Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/weather/{lat}/{lon}\n  method: get\n  operationId: weatherGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/charts\n  method: get\n  operationId: chartsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/chart/{lat}/{lon}/{dec1}/{az1}/{kwp1}\n  method: get\n  operationId: chart1Get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/chart/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}\n  method: get\n  operationId: chart2Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apikey}/chart/{lat}/{lon}/{dec1}/{az1}/{kwp1}/{dec2}/{az2}/{kwp2}/{dec3}/{az3}/{kwp3}\n  method: get\n  operationId: chart3Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/init.js\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/{token}.js\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /chart/{day}/{token}.js\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/history/{token}.js\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/history/{day}/{token}.js\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/clearsky/{token}.js\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/clearsky/{day}/{token}.js\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/forecast-solar/agentic-access/forecast-solar-agentic-access.yml
summary_line: 56 operations
tags:
- Company
- Solar
- Forecast
- Renewable Energy
---
