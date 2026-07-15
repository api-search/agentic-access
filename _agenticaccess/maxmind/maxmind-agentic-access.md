---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: maxmind-geoip-openapi.yml
  format: yaml
  label: GeoIP Country Web Service
  slug: geoip-country
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-openapi.yml
- filename: maxmind-geoip-openapi.yml
  format: yaml
  label: GeoIP City Plus Web Service
  slug: geoip-city
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-openapi.yml
- filename: maxmind-geoip-openapi.yml
  format: yaml
  label: GeoIP Insights Web Service
  slug: geoip-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-openapi.yml
- filename: maxmind-minfraud-openapi.yml
  format: yaml
  label: minFraud Score
  slug: minfraud-score
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-openapi.yml
- filename: maxmind-minfraud-openapi.yml
  format: yaml
  label: minFraud Insights
  slug: minfraud-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-openapi.yml
- filename: maxmind-minfraud-openapi.yml
  format: yaml
  label: minFraud Factors
  slug: minfraud-factors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Maxmind Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'MaxMind exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MaxMind
provider_slug: maxmind
slug: maxmind-agentic-access
source_filename: maxmind-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/maxmind-geoip-openapi.yml, openapi/maxmind-minfraud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 3\n    acting: 3\n  by_consequence:\n    read: 3\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /geoip/v2.1/country/{ipAddress}\n  method: get\n  operationId: getGeoIPCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geoip/v2.1/city/{ipAddress}\n  method: get\n  operationId: getGeoIPCity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /geoip/v2.1/insights/{ipAddress}\n  method: get\n  operationId: getGeoIPInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minfraud/v2.0/score\n  method: post\n  operationId: getMinFraudScore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /minfraud/v2.0/insights\n  method: post\n  operationId: getMinFraudInsights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /minfraud/v2.0/factors\n\
  \  method: post\n  operationId: getMinFraudFactors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/agentic-access/maxmind-agentic-access.yml
summary_line: 6 operations · 3 acting
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
