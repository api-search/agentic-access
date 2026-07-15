---
acting_count: 12
action_class_counts:
  acting: 12
api_specs:
- filename: ttd-data-api.yaml
  format: yaml
  label: The Trade Desk Data API
  slug: the-trade-desk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-trade-desk/refs/heads/main/openapi/ttd-data-api.yaml
consequence_counts:
  physical: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: The Trade Desk Agentic Access
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
  path: /data/deletion-optout/merchant
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /data/deletion-optout/thirdparty
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /data/deletion-optout/thirdparty
operation_count: 12
overview: 'The Trade Desk exposes 12 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 write and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Trade Desk
provider_slug: the-trade-desk
slug: the-trade-desk-agentic-access
source_filename: the-trade-desk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ttd-data-api-raw.json, openapi/ttd-data-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 12\n  by_consequence:\n    write: 6\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /data/advertiser\n  method: post\n  operationId: IngestAdvertiserData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/thirdparty\n  method: post\n  operationId: IngestThirdPartyData\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providerapi/offlineconversion\n  method: post\n  operationId: IngestOfflineConversionData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/deletion-optout/advertiser\n  method: post\n  operationId: DataSubjectRequestAdvertiserData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/deletion-optout/merchant\n  method: post\n  operationId: DataSubjectRequestMerchantData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/deletion-optout/thirdparty\n  method: post\n  operationId: DataSubjectRequestThirdPartyData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/advertiser\n  method: post\n  operationId:\
  \ IngestAdvertiserData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/thirdparty\n  method: post\n  operationId: IngestThirdPartyData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providerapi/offlineconversion\n  method: post\n  operationId: IngestOfflineConversionData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /data/deletion-optout/advertiser\n  method: post\n  operationId: DataSubjectRequestAdvertiserData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/deletion-optout/merchant\n  method: post\n  operationId: DataSubjectRequestMerchantData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/deletion-optout/thirdparty\n  method: post\n  operationId: DataSubjectRequestThirdPartyData\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-trade-desk/refs/heads/main/agentic-access/the-trade-desk-agentic-access.yml
summary_line: 12 operations · 12 acting
tags:
- Advertising
- Programmatic Advertising
- DSP
- Demand-Side Platform
- Campaign Management
- Connected TV
- Digital Advertising
- Marketing
- AdTech
---
