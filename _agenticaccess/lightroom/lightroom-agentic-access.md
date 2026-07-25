---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 20
api_specs:
- filename: lightroom-album-assets-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Album Assets API
  slug: lightroom-album-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-album-assets-api-openapi.yml
- filename: lightroom-albums-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Albums API
  slug: lightroom-albums-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-albums-api-openapi.yml
- filename: lightroom-assets-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Assets API
  slug: lightroom-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-assets-api-openapi.yml
- filename: lightroom-auto-straighten-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Auto Straighten API
  slug: lightroom-auto-straighten-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-auto-straighten-api-openapi.yml
- filename: lightroom-auto-tone-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Auto Tone API
  slug: lightroom-auto-tone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-auto-tone-api-openapi.yml
- filename: lightroom-catalog-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Catalog API
  slug: lightroom-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-catalog-api-openapi.yml
- filename: lightroom-edit-image-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Edit Image API
  slug: lightroom-edit-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-edit-image-api-openapi.yml
- filename: lightroom-health-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Health API
  slug: lightroom-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-health-api-openapi.yml
- filename: lightroom-master-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Master API
  slug: lightroom-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-master-api-openapi.yml
- filename: lightroom-presets-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Presets API
  slug: lightroom-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-presets-api-openapi.yml
- filename: lightroom-renditions-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Renditions API
  slug: lightroom-renditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-renditions-api-openapi.yml
- filename: lightroom-xmp-api-openapi.yml
  format: yaml
  label: Adobe Lightroom XMP API
  slug: lightroom-xmp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-xmp-api-openapi.yml
consequence_counts:
  read: 20
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Lightroom Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lrService/presets
operation_count: 37
overview: 'Adobe Lightroom exposes 37 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 16 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Adobe Lightroom
provider_slug: lightroom
slug: lightroom-agentic-access
source_filename: lightroom-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lightroom-albums-openapi.yml, openapi/lightroom-assets-openapi.yml, openapi/lightroom-catalog-openapi.yml,\n  openapi/lightroom-firefly-services-openapi.yml, openapi/lightroom-services-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 20\n    acting: 17\n  by_consequence:\n    read: 20\n    write: 16\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /catalogs/{catalog_id}/albums\n  method: get\n  operationId: listAlbums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path:\
  \ /catalogs/{catalog_id}/albums/{album_id}\n  method: get\n  operationId: getAlbum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}\n  method: put\n  operationId: createOrUpdateAlbum\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}\n  method: delete\n  operationId: deleteAlbum\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}/assets\n  method: get\n  operationId: listAlbumAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}/assets\n  method: put\n  operationId: addAssetsToAlbum\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}/assets/{asset_id}\n  method: delete\n  operationId: removeAssetFromAlbum\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}\n  method: put\n  operationId: createOrUpdateAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}/master\n  method: put\n  operationId: uploadMaster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}/xmp/develop\n  method: get\n  operationId: getDevelopXmp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}/xmp/develop\n  method: put\n  operationId: putDevelopXmp\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}/renditions/{rendition_type}\n  method: get\n  operationId: getRendition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /health\n  method: get\n  operationId: getHealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalog\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}\n  method: get\n  operationId: getCatalogById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /lrService/autoTone\n  method: post\n  operationId: autoTone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - firefly_api\n- path: /lrService/autoStraighten\n  method: post\n  operationId: autoStraighten\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - firefly_api\n- path: /lrService/presets\n  method: post\n  operationId: applyPresets\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - firefly_api\n- path: /lrService/edit\n  method: post\n  operationId: editImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - firefly_api\n- path: /health\n  method: get\n  operationId: getHealthCheck\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalog\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}\n  method: get\n  operationId: getCatalogById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets\n  method: get\n  operationId: listCatalogAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}\n  method: put\n  operationId: createRevisionForAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}/master\n  method: put\n  operationId: uploadMasterAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path:\
  \ /catalogs/{catalog_id}/assets/{asset_id}/xmp/develop\n  method: get\n  operationId: getAssetDevelopXmp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}/xmp/develop\n  method: put\n  operationId: putAssetDevelopXmp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/assets/{asset_id}/renditions/{rendition_type}\n  method: get\n  operationId: getAssetRendition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n   \
  \ - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums\n  method: get\n  operationId: listAlbums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}\n  method: get\n  operationId: getAlbum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}\n  method: put\n  operationId: createOrUpdateAlbum\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}\n\
  \  method: delete\n  operationId: deleteAlbum\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}/assets\n  method: get\n  operationId: listAlbumAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - lr_partner_apis\n- path: /catalogs/{catalog_id}/albums/{album_id}/assets\n  method: put\n  operationId: addAssetsToAlbum\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - lr_partner_apis\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/agentic-access/lightroom-agentic-access.yml
summary_line: 37 operations · 17 acting · 1 human-in-the-loop
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
---
