---
acting_count: 0
action_class_counts:
  connected: 37
api_specs:
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Property API
  slug: attom-data-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Assessment API
  slug: attom-data-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM AVM & Valuation API
  slug: attom-data-valuation-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Sales & Deed API
  slug: attom-data-sales-deed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Mortgage API
  slug: attom-data-mortgage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Area & Boundary API
  slug: attom-data-area-boundary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM School API
  slug: attom-data-school-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Community & Neighborhood API
  slug: attom-data-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM POI API
  slug: attom-data-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Transportation Noise API
  slug: attom-data-transportation-noise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM AllEvents & Snapshot API
  slug: attom-data-allevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
- filename: attom-data-openapi.yml
  format: yaml
  label: ATTOM Home Equity API
  slug: attom-data-home-equity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/openapi/attom-data-openapi.yml
consequence_counts:
  read: 37
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Attom Data Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'ATTOM exposes 37 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ATTOM
provider_slug: attom-data
slug: attom-data-agentic-access
source_filename: attom-data-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/attom-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 37\n  by_consequence:\n    read: 37\n  human_in_the_loop_required: 0\noperations:\n- path: /propertyapi/v1.0.0/property/id\n  method: get\n  operationId: getPropertyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/basicprofile\n  method: get\n  operationId: getPropertyBasicProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/detail\n\
  \  method: get\n  operationId: getPropertyDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/expandedprofile\n  method: get\n  operationId: getPropertyExpandedProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/address\n  method: get\n  operationId: getPropertyAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/snapshot\n  method: get\n  operationId: getPropertySnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/detailowner\n  method:\
  \ get\n  operationId: getPropertyDetailOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/buildingpermits\n  method: get\n  operationId: getPropertyBuildingPermits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/detailmortgage\n  method: get\n  operationId: getPropertyDetailMortgage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/detailmortgageowner\n  method: get\n  operationId: getPropertyDetailMortgageOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/property/detailwithschools\n\
  \  method: get\n  operationId: getPropertyDetailWithSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/assessment/detail\n  method: get\n  operationId: getAssessmentDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/assessment/snapshot\n  method: get\n  operationId: getAssessmentSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/assessmenthistory/detail\n  method: get\n  operationId: getAssessmentHistoryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/avm/snapshot\n\
  \  method: get\n  operationId: getAvmSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/attomavm/detail\n  method: get\n  operationId: getAttomAvmDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/avmhistory/detail\n  method: get\n  operationId: getAvmHistoryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/valuation/rentalavm\n  method: get\n  operationId: getRentalAvm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/valuation/homeequity\n  method: get\n  operationId: getHomeEquity\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/sale/detail\n  method: get\n  operationId: getSaleDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/sale/snapshot\n  method: get\n  operationId: getSaleSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/saleshistory/detail\n  method: get\n  operationId: getSalesHistoryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/saleshistory/basichistory\n  method: get\n  operationId: getSalesHistoryBasic\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/saleshistory/expandedhistory\n  method: get\n  operationId: getSalesHistoryExpanded\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/transaction/salestrend\n  method: get\n  operationId: getSalesTrend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/allevents/detail\n  method: get\n  operationId: getAllEventsDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/allevents/snapshot\n  method: get\n  operationId: getAllEventsSnapshot\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/school/search\n  method: get\n  operationId: getSchoolSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/school/profile\n  method: get\n  operationId: getSchoolProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyapi/v1.0.0/school/district\n  method: get\n  operationId: getSchoolDistrict\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /areaapi/v2.0.0/geography/lookup\n  method: get\n  operationId: getAreaGeographyLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /areaapi/v2.0.0/hierarchy/lookup\n  method: get\n  operationId: getAreaHierarchyLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /areaapi/v2.0.0/boundary/detail\n  method: get\n  operationId: getAreaBoundaryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/neighborhood/community\n  method: get\n  operationId: getCommunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/neighborhood/poi\n  method: get\n  operationId: getPoiSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/neighborhood/poi/category/lookup\n\
  \  method: get\n  operationId: getPoiCategoryLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transportationnoise\n  method: get\n  operationId: getTransportationNoise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attom-data/refs/heads/main/agentic-access/attom-data-agentic-access.yml
summary_line: 37 operations
tags:
- Property Data
- Real Estate
- Location Data
- Valuation
- AVM
- Assessment
- Mortgage
- Neighborhood
---
