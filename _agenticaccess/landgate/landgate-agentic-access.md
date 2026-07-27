---
acting_count: 0
action_class_counts:
  connected: 27
api_specs:
- filename: landgate-slip-public-arcgis-openapi.yml
  format: yaml
  label: SLIP Public Services (ArcGIS REST)
  slug: slip-public-arcgis-rest-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-slip-public-arcgis-openapi.yml
- filename: landgate-slip-public-ogc-openapi.yml
  format: yaml
  label: SLIP Public OGC Web Services (WMS / WFS)
  slug: slip-public-ogc-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-slip-public-ogc-openapi.yml
- filename: landgate-data-wa-ckan-openapi.yml
  format: yaml
  label: Data WA CKAN Action API
  slug: data-wa-ckan-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-data-wa-ckan-openapi.yml
consequence_counts:
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Landgate Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Landgate exposes 27 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Landgate
provider_slug: landgate
slug: landgate-agentic-access
source_filename: landgate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/landgate-data-wa-ckan-openapi.yml, openapi/landgate-slip-public-arcgis-openapi.yml,\n  openapi/landgate-slip-public-ogc-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 27\n  by_consequence:\n    read: 27\n  human_in_the_loop_required: 0\noperations:\n- path: /api/3/action/status_show\n  method: get\n  operationId: ckanStatusShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/package_list\n  method: get\n  operationId: ckanPackageList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/package_search\n  method: get\n  operationId: ckanPackageSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/package_show\n  method: get\n  operationId: ckanPackageShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/current_package_list_with_resources\n  method: get\n  operationId: ckanCurrentPackageListWithResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/organization_list\n  method: get\n  operationId: ckanOrganizationList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /api/3/action/organization_show\n  method: get\n  operationId: ckanOrganizationShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/group_list\n  method: get\n  operationId: ckanGroupList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/tag_list\n  method: get\n  operationId: ckanTagList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/license_list\n  method: get\n  operationId: ckanLicenseList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/vocabulary_list\n  method:\
  \ get\n  operationId: ckanVocabularyList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/resource_search\n  method: get\n  operationId: ckanResourceSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/package_autocomplete\n  method: get\n  operationId: ckanPackageAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/format_autocomplete\n  method: get\n  operationId: ckanFormatAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3/action/help_show\n  method: get\n  operationId: ckanHelpShow\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog.jsonld\n  method: get\n  operationId: getDataWaDcatCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info\n  method: get\n  operationId: getSlipServerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: get\n  operationId: listSlipRootServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{folder}\n  method: get\n  operationId: listSlipFolderServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /services/{folder}/{service}/MapServer\n  method: get\n  operationId: getSlipMapService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{folder}/{service}/MapServer/legend\n  method: get\n  operationId: getSlipMapServiceLegend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{folder}/{service}/MapServer/{layerId}\n  method: get\n  operationId: getSlipLayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{folder}/{service}/MapServer/{layerId}/query\n  method: get\n  operationId: querySlipLayerFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /services/{folder}/{service}/MapServer/identify\n  method: get\n  operationId: identifySlipFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{folder}/{service}/MapServer/export\n  method: get\n  operationId: exportSlipMapImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{folder}/{service}/MapServer/WMSServer\n  method: get\n  operationId: slipWmsRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{folder}/{service}/MapServer/WFSServer\n  method: get\n  operationId: slipWfsRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/agentic-access/landgate-agentic-access.yml
summary_line: 27 operations
tags:
- Real Estate
- Australia
- Land Registry
- Title
- Valuation
- Property Data
- Open Data
- Geospatial
- Government
- Conveyancing
- PropTech
---
