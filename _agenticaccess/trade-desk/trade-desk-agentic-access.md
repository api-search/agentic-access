---
acting_count: 8
action_class_counts:
  acting: 8
api_specs:
- filename: trade-desk-advertiser-api-openapi.yml
  format: yaml
  label: The Trade Desk Advertiser API
  slug: trade-desk-advertiser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-advertiser-api-openapi.yml
- filename: trade-desk-deletionoptout-api-openapi.yml
  format: yaml
  label: The Trade Desk DeletionOptOut API
  slug: trade-desk-deletionoptout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-deletionoptout-api-openapi.yml
- filename: trade-desk-offlineconversion-api-openapi.yml
  format: yaml
  label: The Trade Desk OfflineConversion API
  slug: trade-desk-offlineconversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-offlineconversion-api-openapi.yml
- filename: trade-desk-thirdparty-api-openapi.yml
  format: yaml
  label: The Trade Desk ThirdParty API
  slug: trade-desk-thirdparty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-thirdparty-api-openapi.yml
- filename: trade-desk-ipaddress-api-openapi.yml
  format: yaml
  label: The Trade Desk IPAddress Data API
  slug: trade-desk-ipaddress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-ipaddress-api-openapi.yml
consequence_counts:
  physical: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trade Desk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /data/deletion-optout/advertiser
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /data/deletion-optout/merchant
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /data/deletion-optout/thirdparty
operation_count: 8
overview: 'The Trade Desk exposes 8 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 write and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Trade Desk
provider_slug: trade-desk
slug: trade-desk-agentic-access
source_filename: trade-desk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/trade-desk-advertiser-api-openapi.yml, openapi/trade-desk-deletionoptout-api-openapi.yml,\n  openapi/trade-desk-ipaddress-api-openapi.yml, openapi/trade-desk-offlineconversion-api-openapi.yml,\n  openapi/trade-desk-thirdparty-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 8\n  by_consequence:\n    write: 5\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /data/advertiser\n  method: post\n  operationId: IngestAdvertiserData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/deletion-optout/advertiser\n  method: post\n  operationId: DataSubjectRequestAdvertiserData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/deletion-optout/merchant\n  method: post\n  operationId: DataSubjectRequestMerchantData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/deletion-optout/thirdparty\n\
  \  method: post\n  operationId: DataSubjectRequestThirdPartyData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/firstpartyipaddress\n  method: post\n  operationId: IngestFirstPartyIPAddressData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/thirdpartyipaddress\n  method: post\n  operationId: IngestThirdPartyIPAddressData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providerapi/offlineconversion\n  method: post\n  operationId: IngestOfflineConversionData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/thirdparty\n  method: post\n  operationId: IngestThirdPartyData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/agentic-access/trade-desk-agentic-access.yml
summary_line: 8 operations · 8 acting
tags:
- Advertising
- Programmatic Advertising
- Demand-Side Platform
- DSP
- AdTech
- Connected TV
- CTV
- Identity
- Unified ID 2.0
- UID2
- OpenPath
- Kokai
- Koa AI
- Galileo
- Sincera
- Open Internet
- Real-Time Bidding
- Open Measurement
---
