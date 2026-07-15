---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: vehicle-history-api
  format: yaml
  label: VINaudit Vehicle History API
  slug: vinaudit-vehicle-history-api
  spec_type: OpenAPI
  url: https://www.vinaudit.com/vehicle-history-api
- filename: vinaudit-vehicle-specifications-openapi.yml
  format: yaml
  label: VINaudit Vehicle Specifications API
  slug: vinaudit-vehicle-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-vehicle-specifications-openapi.yml
- filename: vinaudit-vehicle-market-value-openapi.yml
  format: yaml
  label: VINaudit Vehicle Market Value API
  slug: vinaudit-vehicle-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-vehicle-market-value-openapi.yml
- filename: vinaudit-vehicle-ownership-cost-openapi.yml
  format: yaml
  label: VINaudit Vehicle Ownership Cost API
  slug: vinaudit-vehicle-ownership-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/openapi/vinaudit-vehicle-ownership-cost-openapi.yml
consequence_counts:
  physical: 1
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vinaudit Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getownershipcost.php
operation_count: 10
overview: 'VINaudit exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VINaudit
provider_slug: vinaudit
slug: vinaudit-agentic-access
source_filename: vinaudit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vinaudit-vehicle-history-openapi.yml, openapi/vinaudit-vehicle-market-value-openapi.yml,\n  openapi/vinaudit-vehicle-ownership-cost-openapi.yml, openapi/vinaudit-vehicle-specifications-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 7\n    acting: 3\n  by_consequence:\n    read: 7\n    write: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /query\n  method: get\n  operationId: queryVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query\n  method: post\n  operationId: queryVinPost\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pullreport\n  method: get\n  operationId: pullReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pullreport\n  method: post\n  operationId: pullReportPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /report\n  method: get\n  operationId: viewReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /marketvalue\n  method: get\n  operationId: getMarketValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getownershipcost.php\n  method: get\n  operationId: getOwnershipCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getownershipcost.php\n  method: post\n  operationId: getOwnershipCostPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /specifications\n  method: get\n  operationId: getVehicleSpecifications\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /selections\n  method: get\n  operationId: getVehicleSelections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vinaudit/refs/heads/main/agentic-access/vinaudit-agentic-access.yml
summary_line: 10 operations · 3 acting
tags:
- Vehicle History
- VIN Decoding
- Automotive
- NMVTIS
- Vehicle Specifications
- Market Value
- Recall Data
- REST
---
