---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 16
api_specs:
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Shops API
  slug: tekmetric-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Customers API
  slug: tekmetric-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Vehicles API
  slug: tekmetric-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Repair Orders API
  slug: tekmetric-repair-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Jobs API
  slug: tekmetric-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Employees API
  slug: tekmetric-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Appointments API
  slug: tekmetric-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Inventory API
  slug: tekmetric-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Canned Jobs API
  slug: tekmetric-canned-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
consequence_counts:
  read: 16
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tekmetric Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Tekmetric exposes 17 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tekmetric
provider_slug: tekmetric
slug: tekmetric-agentic-access
source_filename: tekmetric-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tekmetric-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 1\n    connected: 16\n  by_consequence:\n    write: 1\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops\n  method: get\n  operationId: listShops\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/{id}\n  method: get\n  operationId: getShop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles\n  method: get\n  operationId: listVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{id}\n  method: get\n  operationId: getVehicle\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repair-orders\n  method: get\n  operationId: listRepairOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repair-orders/{id}\n  method: get\n  operationId: getRepairOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees\n  method:\
  \ get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{id}\n  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments\n  method: get\n  operationId: listAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/{id}\n  method: get\n  operationId: getAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory\n  method: get\n  operationId: listInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /canned-jobs\n  method: get\n  operationId: listCannedJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/agentic-access/tekmetric-agentic-access.yml
summary_line: 17 operations · 1 acting
tags:
- Automotive
- Auto Repair
- Shop Management
- Fleet
- Vertical SaaS
---
