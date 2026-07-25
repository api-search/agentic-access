---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 28
api_specs:
- filename: akeneo-asset-manager-api-openapi.yml
  format: yaml
  label: Akeneo Asset Manager API
  slug: akeneo-asset-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-asset-manager-api-openapi.yml
- filename: akeneo-attributes-api-openapi.yml
  format: yaml
  label: Akeneo Attributes API
  slug: akeneo-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-attributes-api-openapi.yml
- filename: akeneo-authentication-api-openapi.yml
  format: yaml
  label: Akeneo Authentication API
  slug: akeneo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-authentication-api-openapi.yml
- filename: akeneo-catalogs-api-openapi.yml
  format: yaml
  label: Akeneo Catalogs API
  slug: akeneo-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-catalogs-api-openapi.yml
- filename: akeneo-categories-api-openapi.yml
  format: yaml
  label: Akeneo Categories API
  slug: akeneo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-categories-api-openapi.yml
- filename: akeneo-channels-api-openapi.yml
  format: yaml
  label: Akeneo Channels API
  slug: akeneo-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-channels-api-openapi.yml
- filename: akeneo-currencies-api-openapi.yml
  format: yaml
  label: Akeneo Currencies API
  slug: akeneo-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-currencies-api-openapi.yml
- filename: akeneo-families-api-openapi.yml
  format: yaml
  label: Akeneo Families API
  slug: akeneo-families-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-families-api-openapi.yml
- filename: akeneo-locales-api-openapi.yml
  format: yaml
  label: Akeneo Locales API
  slug: akeneo-locales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-locales-api-openapi.yml
- filename: akeneo-media-files-api-openapi.yml
  format: yaml
  label: Akeneo Media Files API
  slug: akeneo-media-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-media-files-api-openapi.yml
- filename: akeneo-product-models-api-openapi.yml
  format: yaml
  label: Akeneo Product Models API
  slug: akeneo-product-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-product-models-api-openapi.yml
- filename: akeneo-products-api-openapi.yml
  format: yaml
  label: Akeneo Products API
  slug: akeneo-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-products-api-openapi.yml
- filename: akeneo-reference-entities-api-openapi.yml
  format: yaml
  label: Akeneo Reference Entities API
  slug: akeneo-reference-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-reference-entities-api-openapi.yml
- filename: akeneo-system-api-openapi.yml
  format: yaml
  label: Akeneo System API
  slug: akeneo-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-system-api-openapi.yml
- filename: akeneo-workflows-api-openapi.yml
  format: yaml
  label: Akeneo Workflows API
  slug: akeneo-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-workflows-api-openapi.yml
consequence_counts:
  read: 28
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Akeneo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 54
overview: 'Akeneo exposes 54 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read and 26 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Akeneo
provider_slug: akeneo
slug: akeneo-agentic-access
source_filename: akeneo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/akeneo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    acting: 26\n    connected: 28\n  by_consequence:\n    write: 26\n    read: 28\n  human_in_the_loop_required: 0\noperations:\n- path: /api/oauth/v1/token\n  method: post\n  operationId: requestToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1\n  method: get\n  operationId: apiEntry\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/system-information\n  method: get\n  operationId: getSystemInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/products\n  method: patch\n  operationId: bulkUpsertProducts\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/products/{code}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/products/{code}\n  method: patch\n  operationId: upsertProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/products/{code}\n  method: delete\n  operationId: deleteProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/products-uuid\n  method: get\n  operationId: listProductsByUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/products-uuid\n  method: post\n  operationId: createProductByUuid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/products-uuid\n  method: patch\n  operationId: bulkUpsertProductsByUuid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/products-uuid/{uuid}\n  method: get\n  operationId: getProductByUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/products-uuid/{uuid}\n  method: patch\n  operationId: upsertProductByUuid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/products-uuid/{uuid}\n  method: delete\n  operationId: deleteProductByUuid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/product-models\n  method: get\n  operationId: listProductModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/product-models\n  method: post\n  operationId: createProductModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/product-models\n  method: patch\n  operationId: bulkUpsertProductModels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/product-models/{code}\n  method: get\n  operationId: getProductModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/product-models/{code}\n  method: patch\n  operationId: upsertProductModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/product-models/{code}\n  method: delete\n  operationId: deleteProductModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/families\n  method: get\n  operationId: listFamilies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/families\n  method: post\n  operationId: createFamily\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/families/{code}\n  method: get\n  operationId: getFamily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/families/{code}\n  method: patch\n  operationId: upsertFamily\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/families/{code}\n  method: delete\n  operationId: deleteFamily\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/attributes\n  method: get\n  operationId: listAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/attributes\n  method: post\n  operationId: createAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/attributes/{code}\n  method: get\n  operationId: getAttribute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/attributes/{code}\n  method: patch\n  operationId: upsertAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/rest/v1/categories\n  method: post\n  operationId: createCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/categories/{code}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/categories/{code}\n  method: patch\n  operationId: upsertCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/channels\n  method: get\n  operationId:\
  \ listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/channels\n  method: post\n  operationId: createChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/locales\n  method: get\n  operationId: listLocales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/currencies\n  method: get\n  operationId: listCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/media-files\n  method:\
  \ get\n  operationId: listMediaFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/media-files\n  method: post\n  operationId: createMediaFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/media-files/{code}\n  method: get\n  operationId: getMediaFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/media-files/{code}/download\n  method: get\n  operationId: downloadMediaFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/rest/v1/reference-entities\n  method: get\n  operationId: listReferenceEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/reference-entities/{code}\n  method: get\n  operationId: getReferenceEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/reference-entities/{code}\n  method: patch\n  operationId: upsertReferenceEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/asset-families\n  method: get\n  operationId: listAssetFamilies\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/asset-families/{code}\n  method: get\n  operationId: getAssetFamily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/catalogs\n  method: get\n  operationId: listCatalogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/catalogs\n  method: post\n  operationId: createCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/catalogs/{id}\n  method: get\n  operationId: getCatalog\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/catalogs/{id}\n  method: patch\n  operationId: updateCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/catalogs/{id}\n  method: delete\n  operationId: deleteCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rest/v1/workflows\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/v1/workflows/{uuid}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/agentic-access/akeneo-agentic-access.yml
summary_line: 54 operations · 26 acting
tags:
- Product Information Management
- PIM
- Product Data
- Catalog Management
- Commerce
- Retail
---
