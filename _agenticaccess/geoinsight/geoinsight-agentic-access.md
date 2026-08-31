---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: geoinsight-collection-id-api-openapi.yml
  format: yaml
  label: GeoInsight Collection ID API
  slug: geoinsight-collection-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-collection-id-api-openapi.yml
- filename: geoinsight-collections-api-openapi.yml
  format: yaml
  label: GeoInsight Collections API
  slug: geoinsight-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-collections-api-openapi.yml
- filename: geoinsight-data-api-openapi.yml
  format: yaml
  label: GeoInsight Data API
  slug: geoinsight-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-data-api-openapi.yml
- filename: geoinsight-dggrs-id-api-openapi.yml
  format: yaml
  label: GeoInsight DGGRS ID API
  slug: geoinsight-dggrs-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-dggrs-id-api-openapi.yml
- filename: geoinsight-dggs-api-openapi.yml
  format: yaml
  label: GeoInsight DGGS API
  slug: geoinsight-dggs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-dggs-api-openapi.yml
- filename: geoinsight-items-api-openapi.yml
  format: yaml
  label: GeoInsight Items API
  slug: geoinsight-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-items-api-openapi.yml
- filename: geoinsight-root-api-openapi.yml
  format: yaml
  label: GeoInsight Root API
  slug: geoinsight-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-root-api-openapi.yml
- filename: geoinsight-zone-id-api-openapi.yml
  format: yaml
  label: GeoInsight Zone ID API
  slug: geoinsight-zone-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-zone-id-api-openapi.yml
- filename: geoinsight-zones-api-openapi.yml
  format: yaml
  label: GeoInsight Zones API
  slug: geoinsight-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-zones-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Geoinsight Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'GeoInsight exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GeoInsight
provider_slug: geoinsight
slug: geoinsight-agentic-access
source_filename: geoinsight-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-20'\nmethod: generated\nsource: openapi/geoinsight-ogc-api-dggs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: root_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}\n  method: get\n  operationId: collection_id_utoipa_doc\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/dggs\n  method: get\n  operationId: collection_id_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/dggs/{dggrs_id}\n  method: get\n  operationId: collection_id_dggrs_id_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/dggs/{dggrs_id}/zones\n  method: get\n  operationId: collection_id_dggrs_id_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/dggs/{dggrs_id}/zones/{zone_id}\n \
  \ method: get\n  operationId: collection_id_dggrs_id_zone_id_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/dggs/{dggrs_id}/zones/{zone_id}/data\n  method: get\n  operationId: collection_id_dggrs_id_zone_id_data_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/items\n  method: get\n  operationId: items_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/items/{feature_id}\n  method: get\n  operationId: item_id_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /dggs\n  method: get\n  operationId: utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dggs/{dggrs_id}\n  method: get\n  operationId: dggrs_id_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dggs/{dggrs_id}/zones\n  method: get\n  operationId: dggrs_id_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dggs/{dggrs_id}/zones/{zone_id}\n  method: get\n  operationId: dggrs_id_zone_id_utoipa_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/agentic-access/geoinsight-agentic-access.yml
summary_line: 14 operations
tags:
- Geospatial
- DGGS
- Discrete Global Grid System
- Earth Observation
- Remote Sensing
- Spatial Data
- GIS
- Artificial Intelligence
- Machine-Learning
- Analysis-ready data
- Spatial Tokens
- Sentinel-2
- Copernicus
- OGC
- STAC
- GeoParquet
- H3
---
