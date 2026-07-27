---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 61
api_specs:
- filename: ordnance-survey-ngd-features-openapi.json
  format: json
  label: OS NGD API - Features
  slug: os-ngd-api-features
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-ngd-features-openapi.json
- filename: ordnance-survey-ngd-tiles-openapi.json
  format: json
  label: OS NGD API - Tiles
  slug: os-ngd-api-tiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-ngd-tiles-openapi.json
- filename: ordnance-survey-downloads-openapi.yaml
  format: yaml
  label: OS Downloads API
  slug: os-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-downloads-openapi.yaml
- filename: ordnance-survey-osnet-openapi.yaml
  format: yaml
  label: OS Net API
  slug: os-net-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-osnet-openapi.yaml
- filename: ordnance-survey-places-openapi.json
  format: json
  label: OS Places API
  slug: os-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-places-openapi.json
- filename: ordnance-survey-names-openapi.json
  format: json
  label: OS Names API
  slug: os-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-names-openapi.json
- filename: ordnance-survey-linked-identifiers-openapi.json
  format: json
  label: OS Linked Identifiers API
  slug: os-linked-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-linked-identifiers-openapi.json
- filename: ordnance-survey-features-wfs-openapi.json
  format: json
  label: OS Features API
  slug: os-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-features-wfs-openapi.json
- filename: ordnance-survey-maps-openapi.json
  format: json
  label: OS Maps API
  slug: os-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-maps-openapi.json
- filename: ordnance-survey-vector-tile-openapi.json
  format: json
  label: OS Vector Tile API
  slug: os-vector-tile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-vector-tile-openapi.json
consequence_counts:
  read: 61
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ordnance Survey Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 62
overview: 'Ordnance Survey exposes 62 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 61 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ordnance Survey
provider_slug: ordnance-survey
slug: ordnance-survey-agentic-access
source_filename: ordnance-survey-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/ordnance-survey-downloads-openapi.yaml, openapi/ordnance-survey-features-wfs-openapi.json,\n  openapi/ordnance-survey-linked-identifiers-openapi.json, openapi/ordnance-survey-maps-openapi.json,\n  openapi/ordnance-survey-names-openapi.json, openapi/ordnance-survey-ngd-features-openapi.json,\n  openapi/ordnance-survey-ngd-tiles-openapi.json, openapi/ordnance-survey-osnet-openapi.yaml,\n  openapi/ordnance-survey-places-openapi.json, openapi/ordnance-survey-vector-tile-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 62\n  by_action_class:\n    connected: 61\n    acting: 1\n  by_consequence:\n    read: 61\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path:\
  \ /products\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productId}/downloads\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productId}/images/{index}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataPackages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataPackages/{dataPackageId}\n \
  \ method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataPackages/{dataPackageId}/versions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataPackages/{dataPackageId}/versions/{versionId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataPackages/{dataPackageId}/versions/{versionId}/downloads\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wfs\n  method: get\n  operationId: GetFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /wfs/archive/{year}\n  method: get\n  operationId: GetArchiveFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /featureTypes/{featureType}/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /identifierTypes/{identifierType}/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /identifiers/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /productVersionInfo/{correlationMethod}\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /wmts\n  method: get\n  operationId: getWMTSTileData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zxy/{layer}/{z}/{x}/{y}.png\n  method: get\n  operationId: getZXYTileData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /find\n  method: get\n  operationId: findAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nearest\n  method: get\n  operationId: nearestAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /\n  method: get\n  operationId: getLandingPageResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conformance\n  method: get\n  operationId: getConformanceResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: getAllCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}\n  method: get\n  operationId: getCollectionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/schema\n  method: get\n  operationId: getSchema\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/queryables\n  method: get\n  operationId: getCollectionQueryables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/items\n  method: get\n  operationId: getItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/items/{featureId}\n  method: get\n  operationId: getItemById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getLandingPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /conformance\n  method: get\n  operationId: getConformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: getCollectionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tilematrixsets\n  method: get\n  operationId: getTileMatrixSetsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tilematrixsets/{tileMatrixSetId}\n  method: get\n  operationId: getTileMatrixSet\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/tiles\n  method: get\n  operationId: .collection.vector.getTileSetsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/tiles/{tileMatrixSetId}\n  method: get\n  operationId: .collection.vector.getTileSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/tiles/{tileMatrixSetId}/{tileMatrix}/{tileRow}/{tileCol}\n  method: get\n  operationId: .collection.vector.getTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/tiles/{tileMatrix}/{tileRow}/{tileCol}\n\
  \  method: get\n  operationId: 3857.collection.vector.getTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/styles\n  method: get\n  operationId: getStylesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/styles/{styleId}\n  method: get\n  operationId: getStyleRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/styles/{styleId}/{resourceBaseName}/**\n  method: get\n  operationId: getStyleResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations\n  method: get\n  operationId:\
  \ Get Stations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/health\n  method: get\n  operationId: Get Network Health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{stationId}\n  method: get\n  operationId: Get Station\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{stationId}/health\n  method: get\n  operationId: Get Station Health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{stationId}/log\n  method: get\n  operationId: Get Station Logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{stationId}/rinex\n  method: get\n  operationId: Get station data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rinex\n  method: get\n  operationId: Get Rinex Data Years\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rinex/{year}\n  method: get\n  operationId: Get Rinex Data Days\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rinex/{year}/{dayOfYear}\n  method: get\n  operationId: Get Rinex Data Files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rinex/{year}/{dayOfYear}/{filename}\n\
  \  method: get\n  operationId: GetRinexFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bbox\n  method: get\n  operationId: getBbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /find\n  method: get\n  operationId: getFind\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nearest\n  method: get\n  operationId: getNearest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /polygon\n  method: post\n  operationId: postPolygon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postcode\n  method: get\n  operationId: getPostcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /radius\n  method: get\n  operationId: getRadius\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uprn\n  method: get\n  operationId: getUPRN\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vts\n  method: get\n  operationId: getServiceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vts/resources/styles\n  method:\
  \ get\n  operationId: discoverStyles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vts/{layer-name}/resources/styles\n  method: get\n  operationId: discoverOverlayStyles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vts/tile/{z}/{y}/{x}.pbf\n  method: get\n  operationId: getTileData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vts/{layer-name}/tile/{z}/{y}/{x}.pbf\n  method: get\n  operationId: getOverlayTileData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/agentic-access/ordnance-survey-agentic-access.yml
summary_line: 62 operations · 1 acting
tags:
- Real Estate
- United Kingdom
- Land Registry
- Geospatial
- Addressing
- Open Data
- Property Data
- PropTech
- Government
- Mapping
- OGC
- UPRN
- National Mapping
- GNSS
- Vector Tiles
---
