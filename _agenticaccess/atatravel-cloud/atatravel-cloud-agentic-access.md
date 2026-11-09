---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: atatravel-cloud-buildings-api-openapi.yml
  format: yaml
  label: ATA Travel Buildings API
  slug: atatravel-cloud-buildings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atatravel-cloud/openapi/atatravel-cloud-buildings-api-openapi.yml
- filename: atatravel-cloud-commercial-api-openapi.yml
  format: yaml
  label: ATA Travel Commercial API
  slug: atatravel-cloud-commercial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atatravel-cloud/openapi/atatravel-cloud-commercial-api-openapi.yml
- filename: atatravel-cloud-discovery-api-openapi.yml
  format: yaml
  label: ATA Travel Discovery API
  slug: atatravel-cloud-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atatravel-cloud/openapi/atatravel-cloud-discovery-api-openapi.yml
- filename: atatravel-cloud-properties-api-openapi.yml
  format: yaml
  label: ATA Travel Properties API
  slug: atatravel-cloud-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atatravel-cloud/openapi/atatravel-cloud-properties-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atatravel Cloud Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'ATA Travel exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ATA Travel
provider_slug: atatravel-cloud
slug: atatravel-cloud-agentic-access
source_filename: atatravel-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/atatravel-cloud-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /public/stays/discovery-context\n  method: get\n  operationId: getPublicDiscoveryContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/stays/properties\n  method: get\n  operationId: listPublicProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/stays/discover\n\
  \  method: get\n  operationId: discoverPublicStays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/stays/buildings\n  method: get\n  operationId: listPublicBuildings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/stays/buildings/{slug}\n  method: get\n  operationId: getPublicBuilding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/stays/buildings/{slug}/stays\n  method: get\n  operationId: listPublicBuildingStays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/stays/properties/{publicToken}\n  method: get\n  operationId: getPublicProperty\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/stays/properties/{publicToken}/calendar\n  method: get\n  operationId: getPublicPropertyCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/pricing-catalog\n  method: get\n  operationId: getPublicPricingCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/atatravel-cloud/agentic-access/atatravel-cloud-agentic-access.yml
summary_line: 9 operations
tags:
- Travel
- Artificial Intelligence
- Booking
- Accommodation
- Software-as-a-Service
- NoCommission
---
