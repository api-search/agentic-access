---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 19
api_specs:
- filename: drillerdb-com-conferences-api-openapi.yml
  format: yaml
  label: DrillerDB Conferences API
  slug: drillerdb-com-conferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-conferences-api-openapi.yml
- filename: drillerdb-com-contacts-api-openapi.yml
  format: yaml
  label: DrillerDB Contacts API
  slug: drillerdb-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-contacts-api-openapi.yml
- filename: drillerdb-com-documentation-api-openapi.yml
  format: yaml
  label: DrillerDB Documentation API
  slug: drillerdb-com-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-documentation-api-openapi.yml
- filename: drillerdb-com-driller-directory-api-openapi.yml
  format: yaml
  label: DrillerDB Driller directory API
  slug: drillerdb-com-driller-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-driller-directory-api-openapi.yml
- filename: drillerdb-com-enterprise-mcp-api-openapi.yml
  format: yaml
  label: DrillerDB Enterprise MCP API
  slug: drillerdb-com-enterprise-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-enterprise-mcp-api-openapi.yml
- filename: drillerdb-com-equipment-api-openapi.yml
  format: yaml
  label: DrillerDB Equipment API
  slug: drillerdb-com-equipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-equipment-api-openapi.yml
- filename: drillerdb-com-geocoding-api-openapi.yml
  format: yaml
  label: DrillerDB Geocoding API
  slug: drillerdb-com-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-geocoding-api-openapi.yml
- filename: drillerdb-com-inventory-api-openapi.yml
  format: yaml
  label: DrillerDB Inventory API
  slug: drillerdb-com-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-inventory-api-openapi.yml
- filename: drillerdb-com-invoices-api-openapi.yml
  format: yaml
  label: DrillerDB Invoices API
  slug: drillerdb-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-invoices-api-openapi.yml
- filename: drillerdb-com-platform-api-openapi.yml
  format: yaml
  label: DrillerDB Platform API
  slug: drillerdb-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-platform-api-openapi.yml
- filename: drillerdb-com-projects-api-openapi.yml
  format: yaml
  label: DrillerDB Projects API
  slug: drillerdb-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-projects-api-openapi.yml
- filename: drillerdb-com-well-data-api-openapi.yml
  format: yaml
  label: DrillerDB Well data API
  slug: drillerdb-com-well-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-well-data-api-openapi.yml
- filename: drillerdb-com-work-orders-api-openapi.yml
  format: yaml
  label: DrillerDB Work Orders API
  slug: drillerdb-com-work-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-work-orders-api-openapi.yml
consequence_counts:
  read: 19
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Drillerdb Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'DrillerDB exposes 20 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DrillerDB
provider_slug: drillerdb-com
slug: drillerdb-com-agentic-access
source_filename: drillerdb-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/drillerdb-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 19\n    acting: 1\n  by_consequence:\n    read: 19\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/well-depth-lookup\n  method: get\n  operationId: getWellDepthLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/driller-license-lookup\n  method: get\n  operationId: lookupDrillerLicense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /api/find-drillers/nearby\n  method: get\n  operationId: listNearbyDrillers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/geo/zip\n  method: get\n  operationId: geocodeZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  operationId: getPlatformStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calendar/all-conferences\n  method: get\n  operationId: downloadAllConferencesCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calendar/conference/{id}\n  method: get\n  operationId: downloadConferenceCalendar\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/{intWellKey}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects/{intWellKey}/invoices\n  method: get\n  operationId: listProjectInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/work-orders\n  method: get\n  operationId: listWorkOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/work-orders/{id}\n  method: get\n  operationId: getWorkOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contacts/{rolodexId}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/equipment\n  method: get\n  operationId: listEquipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/equipment/{equipmentId}\n  method: get\n  operationId:\
  \ getEquipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/inventory/items\n  method: get\n  operationId: listInventoryItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/inventory/items/{id}\n  method: get\n  operationId: getInventoryItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/openapi.json\n  method: get\n  operationId: getOpenApiDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: callEnterpriseMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - mcp:read:enterprise\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/drillerdb-com/agentic-access/drillerdb-com-agentic-access.yml
summary_line: 20 operations · 1 acting
tags:
- Water Well
- DrillingSoftware
- PumpService
- Project Management
- Software-as-a-Service
---
