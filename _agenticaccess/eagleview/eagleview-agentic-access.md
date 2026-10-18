---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 12
api_specs:
- filename: eagleview-order-adjustments-api-openapi.yml
  format: yaml
  label: EagleView Order Adjustments API
  slug: eagleview-order-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/openapi/eagleview-order-adjustments-api-openapi.yml
- filename: eagleview-order-status-api-openapi.yml
  format: yaml
  label: EagleView Order Status API
  slug: eagleview-order-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/openapi/eagleview-order-status-api-openapi.yml
- filename: eagleview-ordering-api-openapi.yml
  format: yaml
  label: EagleView Ordering API
  slug: eagleview-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/openapi/eagleview-ordering-api-openapi.yml
- filename: eagleview-retrieving-files-api-openapi.yml
  format: yaml
  label: EagleView Retrieving Files API
  slug: eagleview-retrieving-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/openapi/eagleview-retrieving-files-api-openapi.yml
consequence_counts:
  physical: 8
  read: 12
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Eagleview Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Product/SolarProductAvailability
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/Order/PlaceOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/Order/PlaceUpgradeOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/Order/PriceOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/Report/ApproveReportTypeChange
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/Report/CloseReport
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/Report/DenyReportTypeChange
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/Report/UpdateReportAddress
operation_count: 21
overview: 'EagleView exposes 21 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 1 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EagleView
provider_slug: eagleview
slug: eagleview-agentic-access
source_filename: eagleview-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/measurement-orders-v1-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 12\n    acting: 9\n  by_consequence:\n    read: 12\n    physical: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /GetAvailableProducts\n  method: get\n  operationId: GET /v2/Product/GetAvailableProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/Order/PriceOrder\n  method: post\n  operationId: POST /v2/Order/PriceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/Order/PlaceOrder\n  method: post\n  operationId: POST /v2/Order/PlaceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/Order/GetAccountDetails\n  method: get\n  operationId: GET /v3/Order/GetAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Product/SolarProductAvailability\n  method: post\n  operationId: POST/v1/Product/SolarProductAvailability\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/Product/GetReportUpgradeProducts\n  method: get\n  operationId: GET /v2/Product/GetReportUpgradeProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/Order/PlaceUpgradeOrder\n  method: post\n  operationId: POST /v2/Order/PlaceUpgradeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v3/Report/GetReport\n  method: get\n  operationId: GET /v3/Report/GetReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/Report/GetReports\n  method: post\n  operationId: POST /v3/Report/GetReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OrderStatusUpdate\n  method: get\n  operationId: GET /OrderStatusUpdate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /NeedToId\n  method: get\n  operationId: GET /NeedToId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/{reportId}/structure-waste-measurements\n  method: get\n\
  \  operationId: GET /v1/reports/{reportId}/structure-waste-measurements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/Report/UpdateReportAddress\n  method: post\n  operationId: POST /v2/Report/UpdateReportAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/Report/ApproveReportTypeChange\n  method: post\n  operationId: POST /v2/Report/ApproveReportTypeChange\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/Report/DenyReportTypeChange\n  method: post\n  operationId: POST /v2/Report/DenyReportTypeChange\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/Report/CloseReport\n  method: post\n  operationId: POST /v2/Report/CloseReport\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/File/GetReportFile\n  method: get\n\
  \  operationId: GET /v1/File/GetReportFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/File/GetReportFileAnyFormat\n  method: get\n  operationId: GET /v1/File/GetReportFileAnyFormat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FileDelivery\n  method: post\n  operationId: POST /FileDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /FileDeliveryConfirmation\n  method: get\n  operationId: GET /FileDeliveryConfirmation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v3/Report/{reportId}/file-links\n  method: get\n  operationId: GET /v3/Report/{reportId}/file-links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/agentic-access/eagleview-agentic-access.yml
summary_line: 21 operations · 9 acting
tags:
- Geospatial
- AerialImagery
- Data Analytics
- Real Estate
- Insurance
---
