---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: dumpstercontrols-io-customers-api-openapi.yml
  format: yaml
  label: Dumpster Controls Customers API
  slug: dumpstercontrols-io-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-customers-api-openapi.yml
- filename: dumpstercontrols-io-estimates-api-openapi.yml
  format: yaml
  label: Dumpster Controls Estimates API
  slug: dumpstercontrols-io-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-estimates-api-openapi.yml
- filename: dumpstercontrols-io-junk-jobs-api-openapi.yml
  format: yaml
  label: Dumpster Controls Junk Jobs API
  slug: dumpstercontrols-io-junk-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-junk-jobs-api-openapi.yml
- filename: dumpstercontrols-io-leads-api-openapi.yml
  format: yaml
  label: Dumpster Controls Leads API
  slug: dumpstercontrols-io-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-leads-api-openapi.yml
- filename: dumpstercontrols-io-orders-api-openapi.yml
  format: yaml
  label: Dumpster Controls Orders API
  slug: dumpstercontrols-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-orders-api-openapi.yml
- filename: dumpstercontrols-io-sizes-api-openapi.yml
  format: yaml
  label: Dumpster Controls Sizes API
  slug: dumpstercontrols-io-sizes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpstercontrols-io/openapi/dumpstercontrols-io-sizes-api-openapi.yml
consequence_counts:
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dumpstercontrols Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Dumpster Controls exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dumpster Controls
provider_slug: dumpstercontrols-io
slug: dumpstercontrols-io-agentic-access
source_filename: dumpstercontrols-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dumpstercontrols-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_number}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sizes\n  method: get\n  operationId:\
  \ listSizes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates\n  method: get\n  operationId: listEstimates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /junk-jobs\n  method: get\n  operationId: listJunkJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: get\n  operationId: listLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /leads\n  method: post\n  operationId: createLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/dumpstercontrols-io/agentic-access/dumpstercontrols-io-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- Dumpster Controls
- Waste Management
- Software-as-a-Service
- Logistics
- FreeSoftware
---
