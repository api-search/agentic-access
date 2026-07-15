---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 7
api_specs:
- filename: cloverly-estimates-api-openapi.yml
  format: yaml
  label: Cloverly Estimates API
  slug: cloverly-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-estimates-api-openapi.yml
- filename: cloverly-purchases-api-openapi.yml
  format: yaml
  label: Cloverly Purchases API
  slug: cloverly-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-purchases-api-openapi.yml
- filename: cloverly-offset-types-api-openapi.yml
  format: yaml
  label: Cloverly Offset Types API
  slug: cloverly-offset-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-offset-types-api-openapi.yml
- filename: cloverly-account-api-openapi.yml
  format: yaml
  label: Cloverly Account API
  slug: cloverly-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-account-api-openapi.yml
consequence_counts:
  physical: 9
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloverly Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-03-beta/estimates/shipping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-03-beta/purchases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-03-beta/purchases/carbon
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-03-beta/purchases/currency
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-03-beta/purchases/electricity
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-03-beta/purchases/flights
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-03-beta/purchases/shipping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-03-beta/purchases/vehicle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2019-03-beta/purchases/{slug}
operation_count: 22
overview: 'Cloverly exposes 22 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 6 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloverly
provider_slug: cloverly
slug: cloverly-agentic-access
source_filename: cloverly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloverly-account-api-openapi.yml, openapi/cloverly-estimates-api-openapi.yml,\n  openapi/cloverly-offset-types-api-openapi.yml, openapi/cloverly-purchases-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 7\n    acting: 15\n  by_consequence:\n    read: 7\n    write: 6\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /2019-03-beta/account\n  method: get\n  operationId: retrieveAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-03-beta/estimates\n  method: get\n  operationId: listEstimates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-03-beta/estimates/{slug}\n  method: get\n  operationId: retrieveEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-03-beta/estimates/{slug}\n  method: delete\n  operationId: cancelEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/estimates/shipping\n  method: post\n  operationId: estimateShipping\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/estimates/vehicle\n  method: post\n  operationId: estimateVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/estimates/flights\n  method: post\n  operationId: estimateFlight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/estimates/electricity\n  method: post\n  operationId: estimateElectricity\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/estimates/carbon\n  method: post\n  operationId: estimateCarbon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/estimates/currency\n  method: post\n  operationId: estimateCurrency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/offsets\n\
  \  method: get\n  operationId: listOffsets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-03-beta/offsets/{slug}\n  method: get\n  operationId: retrieveOffset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-03-beta/purchases\n  method: get\n  operationId: listPurchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-03-beta/purchases\n  method: post\n  operationId: convertEstimateToPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/purchases/{slug}\n  method: get\n  operationId: retrievePurchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-03-beta/purchases/{slug}\n  method: delete\n  operationId: cancelPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/purchases/shipping\n  method: post\n  operationId: purchaseShipping\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/purchases/vehicle\n  method: post\n  operationId: purchaseVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/purchases/flights\n  method: post\n  operationId: purchaseFlight\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/purchases/electricity\n\
  \  method: post\n  operationId: purchaseElectricity\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/purchases/carbon\n  method: post\n  operationId: purchaseCarbon\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-03-beta/purchases/currency\n  method: post\n  operationId: purchaseCurrency\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/agentic-access/cloverly-agentic-access.yml
summary_line: 22 operations · 15 acting
tags:
- Carbon
- Carbon Credits
- Carbon Offsets
- Catalyst
- Climate
- Climate Action
- Climate Impact X
- CIX
- Decarbonization
- ESG
- Greenhouse Gas
- Net Zero
- Project Developers
- Registries
- Sustainability
- Voluntary Carbon Market
- VCM
---
