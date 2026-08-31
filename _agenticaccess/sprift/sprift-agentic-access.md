---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 24
api_specs:
- filename: sprift-home-api-openapi.yml
  format: yaml
  label: Sprift Home API
  slug: sprift-home-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-home-api-openapi.yml
- filename: sprift-insider-api-openapi.yml
  format: yaml
  label: Sprift Insider API
  slug: sprift-insider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-insider-api-openapi.yml
- filename: sprift-property-api-openapi.yml
  format: yaml
  label: Sprift Property API
  slug: sprift-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-property-api-openapi.yml
- filename: sprift-property-v2-api-openapi.yml
  format: yaml
  label: Sprift Property V2 API
  slug: sprift-property-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-property-v2-api-openapi.yml
- filename: sprift-search-api-openapi.yml
  format: yaml
  label: Sprift Search API
  slug: sprift-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-search-api-openapi.yml
- filename: sprift-share-api-openapi.yml
  format: yaml
  label: Sprift Share API
  slug: sprift-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-share-api-openapi.yml
- filename: sprift-user-api-openapi.yml
  format: yaml
  label: Sprift User API
  slug: sprift-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-user-api-openapi.yml
consequence_counts:
  read: 24
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sprift Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Sprift exposes 27 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sprift
provider_slug: sprift
slug: sprift-agentic-access
source_filename: sprift-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/sprift-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 24\n    acting: 3\n  by_consequence:\n    read: 24\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: HomePage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/login\n  method: post\n  operationId: Login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /user/logout\n  method: get\n  operationId: Logout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: SearchProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/postcode/{postcode}\n  method: get\n  operationId: SearchPropertiesByPostcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/myproperties\n  method: get\n  operationId: SearchMyProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/search\n  method: post\n  operationId:\
  \ SpriftPropertyReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /property/{propertyID}\n  method: get\n  operationId: PropertyDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{uprn}/tv\n  method: get\n  operationId: PropertyDetails-Tv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/maps\n  method: get\n  operationId: PropertyDetails-Maps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/tpo\n\
  \  method: get\n  operationId: PropertyDetails-TPO\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/listedbuildings\n  method: get\n  operationId: PropertyDetails-LB\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/recentlysold\n  method: get\n  operationId: PropertyDetails-RS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/currentlyforsale\n  method: get\n  operationId: PropertyDetails-CFS-UO\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{uprn}/{status}\n  method: get\n  operationId: PropertyDetails-Comparables\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{uprn}/materialinformation\n  method: get\n  operationId: PropertyDetails-MaterialInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{uprn}/search\n  method: get\n  operationId: Property-RawData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{uprn}/propertyid\n  method: get\n  operationId: Property-ID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/priceestimate\n  method: get\n  operationId: Property-Price-Estimate\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/counciltax\n  method: get\n  operationId: Property-Council-Tax\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/epc\n  method: get\n  operationId: Property-EPC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/school\n  method: get\n  operationId: Property-Nearby-School\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/transport\n  method: get\n  operationId: Property-Nearby-Transport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{propertyID}/streetviewmap\n  method: get\n  operationId: PropertyDetails-StreetViewMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /share\n  method: post\n  operationId: ShareReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insider/{outcode}\n  method: get\n  operationId: InsiderActivePropertiesResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insider/{outcode}/withdrawn\n  method: get\n  operationId: InsiderWithdrawnPropertiesResult\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/agentic-access/sprift-agentic-access.yml
summary_line: 27 operations · 3 acting
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Property Listings
- Valuation
- AVM
- Land Registry
- Conveyancing
- Rentals
- Mortgage
---
