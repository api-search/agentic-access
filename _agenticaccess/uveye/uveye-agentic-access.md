---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 1
api_specs:
- filename: uveye-appraisal-api-openapi.yml
  format: yaml
  label: UVeye Appraisal API
  slug: uveye-appraisal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-appraisal-api-openapi.yml
- filename: uveye-inspections-api-openapi.yml
  format: yaml
  label: UVeye Inspections API
  slug: uveye-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-inspections-api-openapi.yml
- filename: uveye-media-api-openapi.yml
  format: yaml
  label: UVeye Media API
  slug: uveye-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-media-api-openapi.yml
- filename: uveye-merchandise-api-openapi.yml
  format: yaml
  label: UVeye Merchandise API
  slug: uveye-merchandise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-merchandise-api-openapi.yml
- filename: uveye-public-links-api-openapi.yml
  format: yaml
  label: UVeye Public Links API
  slug: uveye-public-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/openapi/uveye-public-links-api-openapi.yml
consequence_counts:
  read: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uveye Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'UVeye exposes 8 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: UVeye
provider_slug: uveye
slug: uveye-agentic-access
source_filename: uveye-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/uveye-public-api-v1-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 7\n    connected: 1\n  by_consequence:\n    write: 7\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /inspection\n  method: post\n  operationId: getInspectionDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /latest-inspections\n  method: post\n  operationId: listLatestInspections\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public-link\n  method: post\n  operationId: createInspectionPublicLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inspection-shared\n  method: post\n  operationId: recordInspectionShared\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quote\n  method: post\n  operationId:\
  \ getQuoteByInspection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image\n  method: get\n  operationId: getInspectionImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchandise/inventory/vehicles\n  method: post\n  operationId: submitMerchandiseInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchandise/inventory/sold\n  method: post\n  operationId: markMerchandiseVehiclesSold\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uveye/refs/heads/main/agentic-access/uveye-agentic-access.yml
summary_line: 8 operations · 7 acting
tags:
- Automotive
- Vehicle Inspection
- Artificial Intelligence
- Computer Vision
- Dealerships
- Fleet Management
- Auctions and Remarketing
- Automotive Retail
- Inspection Data
- Company
---
