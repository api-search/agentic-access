---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: jones-lang-lasalle-assets-api-openapi.yml
  format: yaml
  label: Jones Lang LaSalle Assets API
  slug: jones-lang-lasalle-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jones-lang-lasalle/refs/heads/main/openapi/jones-lang-lasalle-assets-api-openapi.yml
- filename: jones-lang-lasalle-contacts-api-openapi.yml
  format: yaml
  label: Jones Lang LaSalle Contacts API
  slug: jones-lang-lasalle-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jones-lang-lasalle/refs/heads/main/openapi/jones-lang-lasalle-contacts-api-openapi.yml
- filename: jones-lang-lasalle-locations-api-openapi.yml
  format: yaml
  label: Jones Lang LaSalle Locations API
  slug: jones-lang-lasalle-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jones-lang-lasalle/refs/heads/main/openapi/jones-lang-lasalle-locations-api-openapi.yml
- filename: jones-lang-lasalle-work-orders-api-openapi.yml
  format: yaml
  label: Jones Lang LaSalle Work Orders API
  slug: jones-lang-lasalle-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jones-lang-lasalle/refs/heads/main/openapi/jones-lang-lasalle-work-orders-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jones Lang Lasalle Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /command/WorkOrder
operation_count: 5
overview: 'Jones Lang LaSalle exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jones Lang LaSalle
provider_slug: jones-lang-lasalle
slug: jones-lang-lasalle-agentic-access
source_filename: jones-lang-lasalle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/jones-lang-lasalle-assets-api-openapi.yml, openapi/jones-lang-lasalle-contacts-api-openapi.yml,\n  openapi/jones-lang-lasalle-locations-api-openapi.yml, openapi/jones-lang-lasalle-work-orders-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /query/Asset\n  method: post\n  operationId: queryAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/Contact\n  method: post\n  operationId: queryContacts\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/Location\n  method: post\n  operationId: queryLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/WorkOrder\n  method: post\n  operationId: queryWorkOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /command/WorkOrder\n  method: post\n  operationId: createWorkOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jones-lang-lasalle/refs/heads/main/agentic-access/jones-lang-lasalle-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Commercial Real Estate
- Facility Management
- Asset Management
- Work Orders
- Fortune 500
---
