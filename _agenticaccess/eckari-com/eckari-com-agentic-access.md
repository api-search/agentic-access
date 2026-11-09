---
acting_count: 0
action_class_counts:
  connected: 24
api_specs:
- filename: eckari-com-company-information-api-openapi.yml
  format: yaml
  label: Eckari Company Information API
  slug: eckari-com-company-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-company-information-api-openapi.yml
- filename: eckari-com-domain-intelligence-api-openapi.yml
  format: yaml
  label: Eckari Domain Intelligence API
  slug: eckari-com-domain-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-domain-intelligence-api-openapi.yml
- filename: eckari-com-foreign-exchange-api-openapi.yml
  format: yaml
  label: Eckari Foreign Exchange API
  slug: eckari-com-foreign-exchange-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-foreign-exchange-api-openapi.yml
- filename: eckari-com-location-api-openapi.yml
  format: yaml
  label: Eckari Location API
  slug: eckari-com-location-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-location-api-openapi.yml
- filename: eckari-com-logistics-api-openapi.yml
  format: yaml
  label: Eckari Logistics API
  slug: eckari-com-logistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-logistics-api-openapi.yml
- filename: eckari-com-weather-api-openapi.yml
  format: yaml
  label: Eckari Weather API
  slug: eckari-com-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eckari-com/openapi/eckari-com-weather-api-openapi.yml
consequence_counts:
  read: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Eckari Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Eckari exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Eckari
provider_slug: eckari-com
slug: eckari-com-agentic-access
source_filename: eckari-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/eckari-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 24\n  by_consequence:\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/companies/uk/{company_number}/accounts\n  method: get\n  operationId: company_uk_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/uk/{company_number}/charges\n  method: get\n  operationId: company_uk_charges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/companies/uk/{company_number}/directors\n  method: get\n  operationId: company_uk_directors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/uk/{company_number}/filings\n  method: get\n  operationId: company_uk_filings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/uk/{company_number}/owners\n  method: get\n  operationId: company_uk_owners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/uk/{company_number}\n  method: get\n  operationId: company_uk_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/uk/{company_number}/registered-office\n\
  \  method: get\n  operationId: company_uk_registered_office\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/uk/search\n  method: get\n  operationId: company_uk_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/uk/{company_number}/status\n  method: get\n  operationId: company_uk_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/us/{id}/filings\n  method: get\n  operationId: company_us_filings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/us/{id}/filings/latest\n  method: get\n  operationId: company_us_filings_latest\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/us/{id}\n  method: get\n  operationId: company_us_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/us/resolve\n  method: get\n  operationId: company_us_resolve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}/expiry\n  method: get\n  operationId: domain_expiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}/registration\n  method: get\n  operationId: domain_registration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/lei/{lei}\n  method: get\n  operationId: entity_lei_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/lei/search\n  method: get\n  operationId: entity_lei_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fx/reference-rate\n  method: get\n  operationId: fx_reference_rate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations/us/geocode\n  method: get\n  operationId: location_us_geocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations/us/geographies\n\
  \  method: get\n  operationId: location_us_geographies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels/detect-carrier\n  method: get\n  operationId: parcel_detect_carrier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather/us/alerts\n  method: get\n  operationId: weather_us_alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather/us/forecast\n  method: get\n  operationId: weather_us_forecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather/us/observation\n  method: get\n  operationId: weather_us_observation\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/eckari-com/agentic-access/eckari-com-agentic-access.yml
summary_line: 24 operations
tags:
- Company Records
- Legal Entities
- Domain Data
- Weather
- Location
- Real-World Data
---
