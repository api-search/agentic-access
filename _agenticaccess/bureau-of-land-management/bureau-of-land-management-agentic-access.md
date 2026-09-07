---
acting_count: 0
action_class_counts:
  connected: 17
api_specs:
- filename: bureau-of-land-management-gbp-hub-search-openapi.json
  format: json
  label: BLM GBP Hub Search API (OGC API - Records)
  slug: blm-gbp-hub-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-land-management/refs/heads/main/openapi/bureau-of-land-management-gbp-hub-search-openapi.json
consequence_counts:
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bureau Of Land Management Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Bureau of Land Management exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bureau of Land Management
provider_slug: bureau-of-land-management
slug: bureau-of-land-management-agentic-access
source_filename: bureau-of-land-management-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: generated\nsource: openapi/bureau-of-land-management-gbp-hub-search-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 17\n  by_consequence:\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /api/search/v1/catalog\n  method: get\n  operationId: CatalogController_getSiteCatalog_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/collections\n  method: get\n  operationId: CollectionController_getSiteCollections_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/collections/{collectionId}\n  method: get\n  operationId: CollectionController_getSiteCollectionFromId_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/collections/{collectionId}/queryables\n  method: get\n  operationId: QueryableController_getSiteCollectionQueryables_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/collections/{collectionId}/items\n  method: get\n  operationId: OgcItemController_getSiteCollectionItems_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/collections/{collectionId}/items/{itemId}\n  method:\
  \ get\n  operationId: OgcItemController_getSiteCollectionItemById_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/collections/{collectionId}/items/{recordId}/related\n  method: get\n  operationId: OgcItemController_getRelatedOgcItemsById_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/collections/{collectionId}/items/{recordId}/connected\n  method: get\n  operationId: OgcItemController_getConnectedOgcItemsById_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/collections/{collectionId}/aggregations\n  method: get\n  operationId: OgcItemAggregationController_getAggregations_api/search/v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1\n  method: get\n  operationId: OgcRootController_getSiteRoot_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/conformance\n  method: get\n  operationId: OgcRootConformanceController_getApiConformance_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/rest/info\n  method: get\n  operationId: GeoserviceController_restInfo_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/rest/services/collections/{collectionId}/geoservice/FeatureServer\n\
  \  method: get\n  operationId: GeoserviceController_featureServer_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/rest/services/collections/{collectionId}/geoservice/FeatureServer/layers\n  method: get\n  operationId: GeoserviceController_featureLayers_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/rest/services/collections/{collectionId}/geoservice/FeatureServer/{layerIndex}\n  method: get\n  operationId: GeoserviceController_featureLayer_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/rest/services/collections/{collectionId}/geoservice/FeatureServer/{layerIndex}/info\n  method: get\n\
  \  operationId: GeoserviceController_featureLayerInfo_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/v1/rest/services/collections/{collectionId}/geoservice/FeatureServer/{layerIndex}/query\n  method: get\n  operationId: GeoserviceController_featureLayerQuery_api/search/v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-land-management/refs/heads/main/agentic-access/bureau-of-land-management-agentic-access.yml
summary_line: 17 operations
tags:
- Environment
- Federal-Government
- Land
- Resources
- GIS
- Geospatial
- Mining
- Public-Lands
- Open-Data
- OGC
- Cadastral
- Recreation
- Grazing
- ArcGIS
- DCAT
- Conservation
- Mapping
---
