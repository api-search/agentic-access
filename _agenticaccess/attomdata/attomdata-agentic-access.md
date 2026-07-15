---
acting_count: 0
action_class_counts:
  connected: 47
api_specs:
- filename: attom-property-api-openapi.yml
  format: yaml
  label: ATTOM Property API
  slug: attom-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-property-api-openapi.yml
- filename: attom-area-api-openapi.yml
  format: yaml
  label: ATTOM Area API
  slug: attom-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-area-api-openapi.yml
- filename: attom-poi-api-openapi.yml
  format: yaml
  label: ATTOM POI API
  slug: attom-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-poi-api-openapi.yml
- filename: attom-community-api-openapi.yml
  format: yaml
  label: ATTOM Community API
  slug: attom-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-community-api-openapi.yml
- filename: attom-parcel-tiles-api-openapi.yml
  format: yaml
  label: ATTOM Parcel Tiles API
  slug: attom-parcel-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/openapi/attom-parcel-tiles-api-openapi.yml
consequence_counts:
  read: 47
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Attomdata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 47
overview: 'ATTOM exposes 47 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 47 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ATTOM
provider_slug: attomdata
slug: attomdata-agentic-access
source_filename: attomdata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/attom-area-api-openapi.yml, openapi/attom-community-api-openapi.yml, openapi/attom-parcel-tiles-api-openapi.yml,\n  openapi/attom-poi-api-openapi.yml, openapi/attom-property-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 47\n  by_consequence:\n    read: 47\n  human_in_the_loop_required: 0\noperations:\n- path: /areaapi/area/boundary/detail\n  method: get\n  operationId: getBoundaryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /areaapi/area/hierarchy/lookup\n  method: get\n  operationId: getHierarchyLookup\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /areaapi/area/state/lookup\n  method: get\n  operationId: getStateLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /areaapi/area/county/lookup\n  method: get\n  operationId: getCountyLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /areaapi/area/cbsa/lookup\n  method: get\n  operationId: getCbsaLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /areaapi/area/geoid/lookup\n  method: get\n  operationId: getGeoIdLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /areaapi/area/geoId/legacyLookup\n  method: get\n  operationId: getGeoCodeLegacyLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/location/lookup\n  method: get\n  operationId: getLocationLookupV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4.0.0/neighborhood/community\n  method: get\n  operationId: getNeighborhoodCommunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/location/lookup\n  method: get\n  operationId: getLocationLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parceltileapi/v1/tile/{z}/{x}/{y}\n\
  \  method: get\n  operationId: getParcelTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/neighborhood/poi\n  method: get\n  operationId: searchPois\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/neighborhood/poi/categorylookup\n  method: get\n  operationId: lookupPoiCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/address\n  method: get\n  operationId: searchPropertyAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/snapshot\n  method: get\n  operationId: getPropertySnapshot\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/detail\n  method: get\n  operationId: getPropertyDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/detailwithschools\n  method: get\n  operationId: getPropertyDetailWithSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/detailmortgage\n  method: get\n  operationId: getPropertyDetailMortgage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/detailowner\n  method: get\n  operationId: getPropertyDetailOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /property/detailmortgageowner\n  method: get\n  operationId: getPropertyDetailMortgageOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/basicprofile\n  method: get\n  operationId: getPropertyBasicProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/basichistory\n  method: get\n  operationId: getPropertyBasicHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/expandedprofile\n  method: get\n  operationId: getPropertyExpandedProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/expandedhistory\n\
  \  method: get\n  operationId: getPropertyExpandedHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/buildingpermits\n  method: get\n  operationId: getPropertyBuildingPermits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/id\n  method: get\n  operationId: searchPropertyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transportationnoise\n  method: get\n  operationId: getTransportationNoise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enumerations/detail\n  method: get\n  operationId: getEnumerationsDetail\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assessment/snapshot\n  method: get\n  operationId: getAssessmentSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assessment/detail\n  method: get\n  operationId: getAssessmentDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assessmenthistory/detail\n  method: get\n  operationId: getAssessmentHistoryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attomavm/detail\n  method: get\n  operationId: getAttomAvmDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /avm/snapshot\n  method: get\n  operationId: getAvmSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /avm/detail\n  method: get\n  operationId: getAvmDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /avmhistory/detail\n  method: get\n  operationId: getAvmHistoryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valuation/rentalavm\n  method: get\n  operationId: getRentalAvm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valuation/homeequity\n  method: get\n  operationId: getHomeEquity\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sale/snapshot\n  method: get\n  operationId: getSaleSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sale/detail\n  method: get\n  operationId: getSaleDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saleshistory/snapshot\n  method: get\n  operationId: getSalesHistorySnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saleshistory/detail\n  method: get\n  operationId: getSalesHistoryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /salescomparables/address/{street}/{citystatezip}\n  method: get\n  operationId: getSalesComparables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/salestrend\n  method: get\n  operationId: getSalesTrend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /allevents/snapshot\n  method: get\n  operationId: getAllEventsSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /allevents/detail\n  method: get\n  operationId: getAllEventsDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /preforeclosure/details\n  method: get\n  operationId: getPreforeclosureDetails\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /school/snapshot\n  method: get\n  operationId: getSchoolSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attomdata/refs/heads/main/agentic-access/attomdata-agentic-access.yml
summary_line: 47 operations
tags:
- Real Estate
- Property Data
- Property Intelligence
- Mortgage
- Assessment
- AVM
- Foreclosure
- Transactions
- Owner Data
- Building Permits
- Geospatial
- Boundaries
- Demographics
- Neighborhood
- POI
- Insurance
- Mortgage Technology
- PropTech
---
