---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 14
api_specs:
- filename: astroclaw-xyz-forecasts-api-openapi.yml
  format: yaml
  label: Astroclaw Forecasts API
  slug: astroclaw-xyz-forecasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astroclaw-xyz/openapi/astroclaw-xyz-forecasts-api-openapi.yml
- filename: astroclaw-xyz-sign-api-openapi.yml
  format: yaml
  label: Astroclaw Sign API
  slug: astroclaw-xyz-sign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astroclaw-xyz/openapi/astroclaw-xyz-sign-api-openapi.yml
- filename: astroclaw-xyz-signs-json-api-openapi.yml
  format: yaml
  label: Astroclaw Signs.json API
  slug: astroclaw-xyz-signs-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astroclaw-xyz/openapi/astroclaw-xyz-signs-json-api-openapi.yml
- filename: astroclaw-xyz-webhooks-api-openapi.yml
  format: yaml
  label: Astroclaw Webhooks API
  slug: astroclaw-xyz-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astroclaw-xyz/openapi/astroclaw-xyz-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 14
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Astroclaw Xyz Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/webhooks/trigger
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/webhooks/trigger
operation_count: 20
overview: 'Astroclaw exposes 20 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 4 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Astroclaw
provider_slug: astroclaw-xyz
slug: astroclaw-xyz-agentic-access
source_filename: astroclaw-xyz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/astroclaw-xyz-openapi.yaml, openapi/astroclaw-xyz.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 14\n    acting: 6\n  by_consequence:\n    read: 14\n    write: 4\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/forecasts/today/{sign}.json\n  method: get\n  operationId: getTodayForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/forecasts/today.json\n  method: get\n  operationId: getTodayForecasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api/forecasts/{date}/{sign}.json\n  method: get\n  operationId: getForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/forecasts/{date}.json\n  method: get\n  operationId: getForecastDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/forecasts/index.json\n  method: get\n  operationId: listForecastDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/signs.json\n  method: get\n  operationId: listSigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sign\n  method: get\n  operationId: findSign\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/subscribe\n  method: post\n  operationId: subscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/trigger\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/unsubscribe\n  method: post\n  operationId: unsubscribeWebhook\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/forecasts/today/{sign}.json\n  method: get\n  operationId: getTodayForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/forecasts/today.json\n  method: get\n  operationId: getTodayForecasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/forecasts/{date}/{sign}.json\n  method: get\n  operationId: getForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/forecasts/{date}.json\n\
  \  method: get\n  operationId: getForecastDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/forecasts/index.json\n  method: get\n  operationId: listForecastDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/signs.json\n  method: get\n  operationId: listSigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sign\n  method: get\n  operationId: findSign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/subscribe\n  method: post\n  operationId: subscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/trigger\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/unsubscribe\n  method: post\n  operationId: unsubscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/astroclaw-xyz/agentic-access/astroclaw-xyz-agentic-access.yml
summary_line: 20 operations · 6 acting
tags:
- Astrology
- Artificial Intelligence
- Agents
- Horoscopes
- Data
---
