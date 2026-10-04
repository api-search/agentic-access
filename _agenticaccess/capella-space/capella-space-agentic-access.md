---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: capella-space-collects-api-openapi.yml
  format: yaml
  label: Capella Space Collects API
  slug: capella-space-collects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-collects-api-openapi.yml
- filename: capella-space-keys-api-openapi.yml
  format: yaml
  label: Capella Space Keys API
  slug: capella-space-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-keys-api-openapi.yml
- filename: capella-space-orders-api-openapi.yml
  format: yaml
  label: Capella Space Orders API
  slug: capella-space-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-orders-api-openapi.yml
- filename: capella-space-repeatrequests-api-openapi.yml
  format: yaml
  label: Capella Space RepeatRequests API
  slug: capella-space-repeatrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-repeatrequests-api-openapi.yml
- filename: capella-space-tasking-api-openapi.yml
  format: yaml
  label: Capella Space Tasking API
  slug: capella-space-tasking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-tasking-api-openapi.yml
- filename: capella-space-tiles-api-openapi.yml
  format: yaml
  label: Capella Space Tiles API
  slug: capella-space-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-tiles-api-openapi.yml
consequence_counts:
  physical: 2
  read: 9
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Capella Space Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/review
operation_count: 16
overview: 'Capella Space exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Capella Space
provider_slug: capella-space
slug: capella-space-agentic-access
source_filename: capella-space-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/capella-space-collects-api-openapi.yml, openapi/capella-space-keys-api-openapi.yml,\n  openapi/capella-space-orders-api-openapi.yml, openapi/capella-space-repeatrequests-api-openapi.yml,\n  openapi/capella-space-tasking-api-openapi.yml, openapi/capella-space-tiles-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 9\n    acting: 7\n  by_consequence:\n    read: 9\n    write: 5\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /collects/list/{taskingrequestId}\n  method: get\n  operationId: getCollectsListByTaskingrequestId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /keys\n  method: post\n  operationId: postKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: post\n  operationId: postOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/review\n  method: post\n  operationId: postOrdersReview\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n \
  \     exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/download\n  method: get\n  operationId: getOrdersByOrderIdDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repeat-requests\n  method: post\n  operationId: postRepeatRequests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repeat-requests/{repeatrequestId}\n  method: get\n  operationId: getRepeatRequestsByRepeatrequestId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /repeat-requests/{repeatrequestId}/status\n  method: get\n  operationId: getRepeatRequestsByRepeatrequestIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repeat-requests/{repeatrequestId}/status\n  method: post\n  operationId: postRepeatRequestsByRepeatrequestIdStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repeat-requests/search\n  method: post\n  operationId: postRepeatRequestsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /task\n  method: post\n  operationId: postTask\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /task/{taskingrequestId}\n  method: get\n  operationId: getTaskByTaskingrequestId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /task/{taskingrequestId}/status\n  method: get\n  operationId: getTaskByTaskingrequestIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /task/{taskingrequestId}/status\n  method: post\n  operationId: postTaskByTaskingrequestIdStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/search\n  method: post\n  operationId: postTasksSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiles/list/{taskingrequestId}\n  method: get\n  operationId: getTilesListByTaskingrequestId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/agentic-access/capella-space-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- Synthetic Aperture Radar
- SAR
- Earth Observation
- Satellite Imagery
- Geospatial
- STAC
- Remote Sensing
- Tasking
- Catalog
- Satellite
---
