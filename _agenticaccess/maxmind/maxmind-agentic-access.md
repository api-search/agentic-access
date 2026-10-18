---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: maxmind-geoip-city-api-openapi.yml
  format: yaml
  label: MaxMind GeoIP City API
  slug: maxmind-geoip-city-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-city-api-openapi.yml
- filename: maxmind-geoip-country-api-openapi.yml
  format: yaml
  label: MaxMind GeoIP Country API
  slug: maxmind-geoip-country-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-country-api-openapi.yml
- filename: maxmind-geoip-insights-api-openapi.yml
  format: yaml
  label: MaxMind GeoIP Insights API
  slug: maxmind-geoip-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-insights-api-openapi.yml
- filename: maxmind-minfraud-factors-api-openapi.yml
  format: yaml
  label: MaxMind minFraud Factors API
  slug: maxmind-minfraud-factors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-factors-api-openapi.yml
- filename: maxmind-minfraud-insights-api-openapi.yml
  format: yaml
  label: MaxMind minFraud Insights API
  slug: maxmind-minfraud-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-insights-api-openapi.yml
- filename: maxmind-minfraud-score-api-openapi.yml
  format: yaml
  label: MaxMind minFraud Score API
  slug: maxmind-minfraud-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-score-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Maxmind Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'MaxMind exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MaxMind
provider_slug: maxmind
slug: maxmind-agentic-access
source_filename: maxmind-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/maxmind-geoip-city-api-openapi.yml, openapi/maxmind-geoip-country-api-openapi.yml,\n  openapi/maxmind-geoip-insights-api-openapi.yml, openapi/maxmind-minfraud-factors-api-openapi.yml,\n  openapi/maxmind-minfraud-insights-api-openapi.yml, openapi/maxmind-minfraud-score-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /geoip/v2.1/city/{ipAddress}\n  method: get\n  operationId: getGeoIPCity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geoip/v2.1/country/{ipAddress}\n\
  \  method: get\n  operationId: getGeoIPCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geoip/v2.1/insights/{ipAddress}\n  method: get\n  operationId: getGeoIPInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minfraud/v2.0/factors\n  method: post\n  operationId: getMinFraudFactors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minfraud/v2.0/insights\n  method: post\n  operationId: getMinFraudInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minfraud/v2.0/score\n  method: post\n  operationId: getMinFraudScore\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/agentic-access/maxmind-agentic-access.yml
summary_line: 6 operations
tags:
- IP Intelligence
- Geolocation
- Fraud Prevention
- Risk Scoring
- VPN Detection
- Proxy Detection
- ISP Data
- GeoIP
---
