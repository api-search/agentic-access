---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: iec-cim-customers-api-openapi.yml
  format: yaml
  label: iec-cim Customers API
  slug: iec-cim-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-customers-api-openapi.yml
- filename: iec-cim-metering-api-openapi.yml
  format: yaml
  label: iec-cim Metering API
  slug: iec-cim-metering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-metering-api-openapi.yml
- filename: iec-cim-network-assets-api-openapi.yml
  format: yaml
  label: iec-cim Network Assets API
  slug: iec-cim-network-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-network-assets-api-openapi.yml
- filename: iec-cim-outages-api-openapi.yml
  format: yaml
  label: iec-cim Outages API
  slug: iec-cim-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-outages-api-openapi.yml
- filename: iec-cim-work-orders-api-openapi.yml
  format: yaml
  label: iec-cim Work Orders API
  slug: iec-cim-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/openapi/iec-cim-work-orders-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Iec Cim Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'iec-cim exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: iec-cim
provider_slug: iec-cim
slug: iec-cim-agentic-access
source_filename: iec-cim-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/iec-cim-61968-distribution-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{mRID}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meters\n  method: get\n  operationId: listMeters\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meters/{mRID}/readings\n  method: get\n  operationId: getMeterReadings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outages\n  method: get\n  operationId: listOutages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outages/{mRID}\n  method: get\n  operationId: getOutage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /work-orders\n\
  \  method: get\n  operationId: listWorkOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/agentic-access/iec-cim-agentic-access.yml
summary_line: 8 operations
tags: []
---
