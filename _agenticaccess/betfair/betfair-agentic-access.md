---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 1
api_specs:
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Betting API
  slug: betfair-betting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Accounts API
  slug: betfair-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Heartbeat API
  slug: betfair-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
- filename: betfair-asyncapi.yml
  format: yaml
  label: Betfair Exchange Stream API
  slug: betfair-exchange-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/asyncapi/betfair-asyncapi.yml
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Historic Data API
  slug: betfair-historic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
consequence_counts:
  physical: 7
  read: 1
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Betfair Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /GetMyData
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /betting/rest/v1.0/cancelOrders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /betting/rest/v1.0/listClearedOrders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /betting/rest/v1.0/listCurrentOrders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /betting/rest/v1.0/placeOrders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /betting/rest/v1.0/replaceOrders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /betting/rest/v1.0/updateOrders/
operation_count: 27
overview: 'Betfair exposes 27 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 19 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Betfair
provider_slug: betfair
slug: betfair-agentic-access
source_filename: betfair-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/betfair-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 26\n    connected: 1\n  by_consequence:\n    write: 19\n    physical: 7\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keepAlive\n  method: post\n  operationId: keepAlive\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/listEventTypes/\n  method: post\n  operationId: listEventTypes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/listCompetitions/\n  method: post\n  operationId: listCompetitions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/listEvents/\n  method: post\n  operationId: listEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/listMarketTypes/\n  method: post\n  operationId: listMarketTypes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /betting/rest/v1.0/listMarketCatalogue/\n  method: post\n  operationId: listMarketCatalogue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/listMarketBook/\n  method: post\n  operationId: listMarketBook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/listRunnerBook/\n  method: post\n  operationId: listRunnerBook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/listCurrentOrders/\n  method: post\n  operationId: listCurrentOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/listClearedOrders/\n  method: post\n  operationId: listClearedOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/placeOrders/\n\
  \  method: post\n  operationId: placeOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/cancelOrders/\n  method: post\n  operationId: cancelOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/replaceOrders/\n  method: post\n  operationId: replaceOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /betting/rest/v1.0/updateOrders/\n  method: post\n  operationId: updateOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/rest/v1.0/getAccountFunds/\n  method: post\n  operationId: getAccountFunds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /account/rest/v1.0/getAccountDetails/\n  method: post\n  operationId: getAccountDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/rest/v1.0/getAccountStatement/\n  method: post\n  operationId: getAccountStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/rest/v1.0/listCurrencyRates/\n  method: post\n  operationId: listCurrencyRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/rest/v1.0/getDeveloperAppKeys/\n  method: post\n  operationId: getDeveloperAppKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /heartbeat/rest/v1.0/heartbeat/\n  method: post\n  operationId: heartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetMyData\n  method: post\n  operationId: getMyData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetCollectionOptions\n  method: post\n  operationId: getCollectionOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetAdvBasketDataSize\n  method: post\n  operationId: getAdvBasketDataSize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DownloadListOfFiles\n\
  \  method: post\n  operationId: downloadListOfFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DownloadFile\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/agentic-access/betfair-agentic-access.yml
summary_line: 27 operations · 26 acting
tags:
- Betting Exchange
- Sports Betting
- Wagering
- Trading
- Market Data
- JSON-RPC
- Streaming
---
