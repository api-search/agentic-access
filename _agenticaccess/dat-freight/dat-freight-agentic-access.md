---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 3
api_specs:
- filename: dat-freight-booknow-api-openapi.yml
  format: yaml
  label: DAT Freight & Analytics BookNow API
  slug: dat-freight-booknow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-booknow-api-openapi.yml
- filename: dat-freight-freight-posting-api-openapi.yml
  format: yaml
  label: DAT Freight & Analytics Freight Posting API
  slug: dat-freight-freight-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-freight-posting-api-openapi.yml
- filename: dat-freight-identity-api-openapi.yml
  format: yaml
  label: DAT Freight & Analytics Identity API
  slug: dat-freight-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-identity-api-openapi.yml
- filename: dat-freight-load-board-search-api-openapi.yml
  format: yaml
  label: DAT Freight & Analytics Load Board Search API
  slug: dat-freight-load-board-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-load-board-search-api-openapi.yml
- filename: dat-freight-rateview-api-openapi.yml
  format: yaml
  label: DAT Freight & Analytics RateView API
  slug: dat-freight-rateview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-rateview-api-openapi.yml
- filename: dat-freight-tracking-api-openapi.yml
  format: yaml
  label: DAT Freight & Analytics Tracking API
  slug: dat-freight-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-tracking-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dat Freight Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tracking/v1/shipments
operation_count: 10
overview: 'DAT Freight & Analytics exposes 10 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DAT Freight & Analytics
provider_slug: dat-freight
slug: dat-freight-agentic-access
source_filename: dat-freight-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/dat-freight-booknow-api-openapi.yml, openapi/dat-freight-freight-posting-api-openapi.yml,\n  openapi/dat-freight-identity-api-openapi.yml, openapi/dat-freight-load-board-search-api-openapi.yml,\n  openapi/dat-freight-rateview-api-openapi.yml, openapi/dat-freight-tracking-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 7\n    connected: 3\n  by_consequence:\n    write: 6\n    read: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /booknow/v1/bookings\n  method: post\n  operationId: createBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadboard/v2/assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loadboard/v2/assets\n  method: post\n  operationId: createAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadboard/v2/assets/{assetId}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/v1/token/organization\n  method: post\n  operationId: createOrganizationToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/v1/token/user\n  method: post\n  operationId: createUserToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadboard/v3/searches\n  method: post\n  operationId: createLoadSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /linehaulrates/v1/lookups\n  method: post\n  operationId: lookupRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/v1/shipments\n  method: post\n  operationId: registerShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tracking/v1/shipments/{shipmentId}\n  method: get\n  operationId: getShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/agentic-access/dat-freight-agentic-access.yml
summary_line: 10 operations · 7 acting
tags:
- Freight
- Trucking
- Load Board
- Logistics
- Freight Rates
- RateView
- Supply Chain
- Transportation
- Analytics
---
