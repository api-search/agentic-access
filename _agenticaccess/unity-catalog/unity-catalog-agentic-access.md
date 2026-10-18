---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 21
api_specs:
- filename: unity-catalog-catalogs-api-openapi.yml
  format: yaml
  label: Unity Catalog Catalogs API
  slug: unity-catalog-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-catalogs-api-openapi.yml
- filename: unity-catalog-credentials-api-openapi.yml
  format: yaml
  label: Unity Catalog Credentials API
  slug: unity-catalog-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-credentials-api-openapi.yml
- filename: unity-catalog-deltacommits-api-openapi.yml
  format: yaml
  label: Unity Catalog Delta Commits API
  slug: unity-catalog-deltacommits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-deltacommits-api-openapi.yml
- filename: unity-catalog-external-locations-api-openapi.yml
  format: yaml
  label: Unity Catalog External Locations API
  slug: unity-catalog-external-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-external-locations-api-openapi.yml
- filename: unity-catalog-functions-api-openapi.yml
  format: yaml
  label: Unity Catalog Functions API
  slug: unity-catalog-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-functions-api-openapi.yml
- filename: unity-catalog-grants-api-openapi.yml
  format: yaml
  label: Unity Catalog Grants API
  slug: unity-catalog-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-grants-api-openapi.yml
- filename: unity-catalog-metastores-api-openapi.yml
  format: yaml
  label: Unity Catalog Metastores API
  slug: unity-catalog-metastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-metastores-api-openapi.yml
- filename: unity-catalog-schemas-api-openapi.yml
  format: yaml
  label: Unity Catalog Schemas API
  slug: unity-catalog-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-schemas-api-openapi.yml
- filename: unity-catalog-tables-api-openapi.yml
  format: yaml
  label: Unity Catalog Tables API
  slug: unity-catalog-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-tables-api-openapi.yml
- filename: unity-catalog-temporarycredentials-api-openapi.yml
  format: yaml
  label: Unity Catalog Temporary Credentials API
  slug: unity-catalog-temporarycredentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-temporarycredentials-api-openapi.yml
- filename: unity-catalog-volumes-api-openapi.yml
  format: yaml
  label: Unity Catalog Volumes API
  slug: unity-catalog-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-volumes-api-openapi.yml
- filename: unity-catalog-model-versions-api-openapi.yml
  format: yaml
  label: Unity Catalog Model Versions API
  slug: unity-catalog-model-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-model-versions-api-openapi.yml
- filename: unity-catalog-registered-models-api-openapi.yml
  format: yaml
  label: Unity Catalog Registered Models API
  slug: unity-catalog-registered-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-registered-models-api-openapi.yml
consequence_counts:
  physical: 1
  read: 21
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Unity Catalog Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delta/preview/commits
operation_count: 54
overview: 'Unity Catalog exposes 54 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 32 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Unity Catalog
provider_slug: unity-catalog
slug: unity-catalog-agentic-access
source_filename: unity-catalog-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/unitycatalog-all.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    acting: 33\n    connected: 21\n  by_consequence:\n    write: 32\n    read: 21\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /catalogs\n  method: post\n  operationId: createCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs\n  method: get\n  operationId: listCatalogs\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{name}\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{name}\n  method: patch\n  operationId: updateCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/{name}\n  method: delete\n  operationId: deleteCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /schemas\n  method: post\n  operationId: createSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas\n  method: get\n  operationId: listSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/{full_name}\n  method: get\n  operationId: getSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/{full_name}\n  method: patch\n  operationId: updateSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas/{full_name}\n  method: delete\n  operationId: deleteSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /staging-tables\n  method: post\n  operationId: createStagingTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables\n  method: post\n  operationId: createTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables\n  method: get\n  operationId: listTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables/{full_name}\n  method: get\n  operationId: getTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables/{full_name}\n  method: delete\n  operationId: deleteTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /volumes\n  method: post\n  operationId: createVolume\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /volumes\n  method: get\n  operationId: listVolumes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volumes/{name}\n  method: get\n  operationId: getVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volumes/{name}\n  method: patch\n  operationId: updateVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /volumes/{name}\n  method: delete\n  operationId: deleteVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /temporary-model-version-credentials\n  method: post\n  operationId: generateTemporaryModelVersionCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /temporary-table-credentials\n  method: post\n  operationId: generateTemporaryTableCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /temporary-volume-credentials\n  method: post\n  operationId: generateTemporaryVolumeCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /functions\n  method: post\n  operationId: createFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /functions\n  method: get\n  operationId: listFunctions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /functions/{name}\n  method: get\n  operationId: getFunction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /functions/{name}\n  method: delete\n  operationId: deleteFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: post\n  operationId: createRegisteredModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /models\n  method: get\n  operationId: listRegisteredModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{full_name}\n  method: get\n  operationId: getRegisteredModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{full_name}\n  method: patch\n  operationId: updateRegisteredModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{full_name}\n  method: delete\n  operationId: deleteRegisteredModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/versions\n  method: post\n  operationId: createModelVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{full_name}/versions\n  method: get\n  operationId: listModelVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{full_name}/versions/{version}\n  method: get\n  operationId: getModelVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /models/{full_name}/versions/{version}\n  method: patch\n  operationId: updateModelVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{full_name}/versions/{version}\n  method: delete\n  operationId: deleteModelVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{full_name}/versions/{version}/finalize\n  method: patch\n  operationId: finalizeModelVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /temporary-path-credentials\n  method: post\n  operationId: generateTemporaryPathCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /permissions/{securable_type}/{full_name}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /permissions/{securable_type}/{full_name}\n  method: patch\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metastore_summary\n  method: get\n  operationId: summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials\n  method: post\n  operationId: createCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credentials\n  method: get\n  operationId: listCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials/{name}\n  method: get\n  operationId: getCredential\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials/{name}\n  method: patch\n  operationId: updateCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credentials/{name}\n  method: delete\n  operationId: deleteCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external-locations\n  method: post\n  operationId: createExternalLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external-locations\n  method: get\n  operationId: listExternalLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-locations/{name}\n  method: get\n  operationId: getExternalLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-locations/{name}\n  method: delete\n  operationId: deleteExternalLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /external-locations/{name}\n  method: patch\n  operationId: updateExternalLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delta/preview/commits\n  method: get\n  operationId: getCommits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delta/preview/commits\n  method: post\n  operationId: commit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/agentic-access/unity-catalog-agentic-access.yml
summary_line: 54 operations · 33 acting
tags:
- Data
- Artificial Intelligence
- Catalog
- Governance
- Multi-Modal
---
