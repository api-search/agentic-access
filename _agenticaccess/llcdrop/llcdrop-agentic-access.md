---
acting_count: 0
action_class_counts:
  connected: 30
api_specs:
- filename: llcdrop-account-api-openapi.yml
  format: yaml
  label: LLCDrop Account API
  slug: llcdrop-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-account-api-openapi.yml
- filename: llcdrop-businesses-api-openapi.yml
  format: yaml
  label: LLCDrop Businesses API
  slug: llcdrop-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-businesses-api-openapi.yml
- filename: llcdrop-counties-and-stats-api-openapi.yml
  format: yaml
  label: LLCDrop Counties and stats API
  slug: llcdrop-counties-and-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-counties-and-stats-api-openapi.yml
- filename: llcdrop-datasets-api-openapi.yml
  format: yaml
  label: LLCDrop Datasets API
  slug: llcdrop-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-datasets-api-openapi.yml
- filename: llcdrop-filings-api-openapi.yml
  format: yaml
  label: LLCDrop Filings API
  slug: llcdrop-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-filings-api-openapi.yml
- filename: llcdrop-parcels-api-openapi.yml
  format: yaml
  label: LLCDrop Parcels API
  slug: llcdrop-parcels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-parcels-api-openapi.yml
- filename: llcdrop-reference-lists-api-openapi.yml
  format: yaml
  label: LLCDrop Reference lists API
  slug: llcdrop-reference-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-reference-lists-api-openapi.yml
consequence_counts:
  read: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Llcdrop Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'LLCDrop exposes 30 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LLCDrop
provider_slug: llcdrop
slug: llcdrop-agentic-access
source_filename: llcdrop-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/llcdrop-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 30\n  by_consequence:\n    read: 30\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/me\n  method: get\n  operationId: me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/businesses\n  method: get\n  operationId: businessesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/businesses/by-document/{document_number}\n  method: get\n  operationId:\
  \ businessByDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/businesses/{id}\n  method: get\n  operationId: businessById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/businesses/{id}/officers\n  method: get\n  operationId: businessOfficers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/businesses/{id}/parcels\n  method: get\n  operationId: businessParcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/parcels\n  method: get\n  operationId: parcelsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/parcels/{key}\n  method: get\n  operationId: parcelByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/leads/enrich\n  method: get\n  operationId: leadEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/filings/daily\n  method: get\n  operationId: dailyIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/filings/daily/{date}\n  method: get\n  operationId: dailyFilings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/counties\n  method: get\n  operationId:\
  \ counties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/counties/{key}\n  method: get\n  operationId: county\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/stats\n  method: get\n  operationId: stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/industries\n  method: get\n  operationId: industries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/entity-types\n  method: get\n  operationId: entityTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/fl/websites/search\n  method: get\n  operationId: websitesSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/websites/by-entity/{entityId}\n  method: get\n  operationId: websitesByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/property-sales/search\n  method: get\n  operationId: propertySalesSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/property-sales/by-entity/{entityId}\n  method: get\n  operationId: propertySalesByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/property-transfers/search\n\
  \  method: get\n  operationId: propertyTransfersSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/property-transfers/by-entity/{entityId}\n  method: get\n  operationId: propertyTransfersByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/workforce/search\n  method: get\n  operationId: workforceSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/workforce/by-entity/{entityId}\n  method: get\n  operationId: workforceByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/ppp/search\n  method: get\n  operationId: pppSearch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/ppp/by-entity/{entityId}\n  method: get\n  operationId: pppByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/sba/search\n  method: get\n  operationId: sbaSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/sba/by-entity/{entityId}\n  method: get\n  operationId: sbaByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fl/fmcsa/search\n  method: get\n  operationId: fmcsaSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/fl/fmcsa/by-entity/{entityId}\n  method: get\n  operationId: fmcsaByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/llcdrop/agentic-access/llcdrop-agentic-access.yml
summary_line: 30 operations
tags:
- Lead Generation
- Business Data
- Marketing
- Real Estate
---
