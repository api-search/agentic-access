---
acting_count: 63
action_class_counts:
  acting: 63
  connected: 26
api_specs:
- filename: configure8-catalog-entities-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entities API
  slug: configure8-catalog-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entities-api-openapi.yml
- filename: configure8-catalog-relations-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Relations API
  slug: configure8-catalog-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-relations-api-openapi.yml
- filename: configure8-deployments-api-openapi.yml
  format: yaml
  label: Configure8 Deployments API
  slug: configure8-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-deployments-api-openapi.yml
- filename: configure8-scorecards-api-openapi.yml
  format: yaml
  label: Configure8 Scorecards API
  slug: configure8-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-scorecards-api-openapi.yml
- filename: configure8-users-api-openapi.yml
  format: yaml
  label: Configure8 Users API
  slug: configure8-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-users-api-openapi.yml
- filename: configure8-catalog-entity-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entity API
  slug: configure8-catalog-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entity-api-openapi.yml
- filename: configure8-catalog-entity-batch-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entity Batch API
  slug: configure8-catalog-entity-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entity-batch-api-openapi.yml
- filename: configure8-catalog-entity-metadata-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entity Metadata API
  slug: configure8-catalog-entity-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entity-metadata-api-openapi.yml
- filename: configure8-catalog-relation-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Relation API
  slug: configure8-catalog-relation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-relation-api-openapi.yml
- filename: configure8-credential-api-openapi.yml
  format: yaml
  label: Configure8 Credential API
  slug: configure8-credential-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-credential-api-openapi.yml
- filename: configure8-deployment-api-openapi.yml
  format: yaml
  label: Configure8 Deployment API
  slug: configure8-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-deployment-api-openapi.yml
- filename: configure8-module-settings-api-openapi.yml
  format: yaml
  label: Configure8 Module Settings API
  slug: configure8-module-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-module-settings-api-openapi.yml
- filename: configure8-private-scim-api-openapi.yml
  format: yaml
  label: Configure8 Private SCIM API
  slug: configure8-private-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-private-scim-api-openapi.yml
- filename: configure8-scim-api-openapi.yml
  format: yaml
  label: Configure8 SCIM API
  slug: configure8-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-scim-api-openapi.yml
- filename: configure8-scorecard-api-openapi.yml
  format: yaml
  label: Configure8 Scorecard API
  slug: configure8-scorecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-scorecard-api-openapi.yml
- filename: configure8-sync-api-openapi.yml
  format: yaml
  label: Configure8 Sync API
  slug: configure8-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-sync-api-openapi.yml
- filename: configure8-templates-api-openapi.yml
  format: yaml
  label: Configure8 Templates API
  slug: configure8-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-templates-api-openapi.yml
consequence_counts:
  physical: 1
  read: 26
  safety-critical: 50
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 50
kind: agentic-access
layout: agentic-access
method: generated
name: Configure8 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/scim
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/scim
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /public/v1/catalog/batch/entities
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/batch/entities/resource
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/application
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/application/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/base
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/base/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/environment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/environment/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/library
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/library/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/manifest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/manifest/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/person
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/person/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/repository
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/repository/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/resource
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/resource/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/service
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/service/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v1/catalog/entities/system
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /public/v1/catalog/entities/system/{id}
operation_count: 89
overview: 'Configure8 exposes 89 API operations that an AI agent could call, of which 63 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 12 write, 1 physical, and 50 safety-critical.


  50 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Configure8
provider_slug: configure8
slug: configure8-agentic-access
source_filename: configure8-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/configure8-catalog-entities-api-openapi.yml, openapi/configure8-catalog-entity-api-openapi.yml,\n  openapi/configure8-catalog-entity-batch-api-openapi.yml, openapi/configure8-catalog-entity-metadata-api-openapi.yml,\n  openapi/configure8-catalog-relation-api-openapi.yml, openapi/configure8-catalog-relations-api-openapi.yml,\n  openapi/configure8-credential-api-openapi.yml, openapi/configure8-deployment-api-openapi.yml,\n  openapi/configure8-deployments-api-openapi.yml, openapi/configure8-module-settings-api-openapi.yml,\n  openapi/configure8-private-scim-api-openapi.yml, openapi/configure8-scim-api-openapi.yml,\n  openapi/configure8-scorecard-api-openapi.yml, openapi/configure8-scorecards-api-openapi.yml,\n  openapi/configure8-sync-api-openapi.yml, openapi/configure8-templates-api-openapi.yml, openapi/configure8-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically\
  \ from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 89\n  by_action_class:\n    acting: 63\n    connected: 26\n  by_consequence:\n    write: 12\n    read: 26\n    safety-critical: 50\n    physical: 1\n  human_in_the_loop_required: 50\noperations:\n- path: /catalog/entities\n  method: post\n  operationId: queryCatalogEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/entities/{id}\n  method: get\n  operationId: getCatalogEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/entities/{id}\n\
  \  method: patch\n  operationId: updateCatalogEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/entities/{id}\n  method: delete\n  operationId: deleteCatalogEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/entities/service\n  method: post\n  operationId: createServiceEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/entities/resource\n  method: post\n  operationId: createResourceEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/entities/person\n  method: post\n  operationId: createPersonEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/entities/system\n  method: post\n  operationId: createSystemEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/entities/environment\n  method: post\n  operationId: createEnvironmentEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/catalog/entities\n  method: post\n  operationId: CatalogEntityController_getCatalogEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/{id}\n  method:\
  \ get\n  operationId: CatalogEntityController_getCatalogEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/catalog/entities/{id}\n  method: delete\n  operationId: CatalogEntityController_deleteCatalogEntityById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/person\n  method: post\n  operationId: CatalogEntityController_createPersonEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/resource/{id}\n  method: patch\n  operationId: CatalogEntityController_updateResourceEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/service/{id}\n  method: patch\n  operationId: CatalogEntityController_updateServiceEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/person/{id}\n\
  \  method: patch\n  operationId: CatalogEntityController_updatePersonEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/resource\n  method: post\n  operationId: CatalogEntityController_createCatalogResourceEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/library\n  method: post\n  operationId: CatalogEntityController_createCatalogLibrary\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/repository\n  method: post\n  operationId: CatalogEntityController_createCatalogRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/repository/{id}\n  method: patch\n  operationId: CatalogEntityController_updateRepositoryEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/environment\n  method: post\n  operationId: CatalogEntityController_createCatalogEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/service\n  method: post\n  operationId: CatalogEntityController_createServiceEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /public/v1/catalog/entities/system\n  method: post\n  operationId: CatalogEntityController_createCatalogSystemEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/application\n  method: post\n  operationId: CatalogEntityController_createCatalogApplicationEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/application/{id}\n  method: patch\n  operationId:\
  \ CatalogEntityController_updateApplicationEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/manifest\n  method: post\n  operationId: CatalogEntityController_createCatalogManifestEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/environment/{id}\n  method: patch\n  operationId: CatalogEntityController_updateCatalogEnvironmentEntity\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/manifest/{id}\n  method: patch\n  operationId: CatalogEntityController_updateCatalogManifestEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/system/{id}\n  method: patch\n  operationId: CatalogEntityController_updateCatalogSystemEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/library/{id}\n  method: patch\n  operationId: CatalogEntityController_updateCatalogLibraryEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/entities/base\n  method: post\n  operationId: CatalogEntityController_createCatalogBase\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /public/v1/catalog/entities/base/{id}\n  method: patch\n  operationId: CatalogEntityController_updateCatalogBaseEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/batch/entities/resource\n  method: post\n  operationId: CatalogEntityBatchController_createCatalogEntitiesBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/batch/entities\n  method: delete\n  operationId:\
  \ CatalogEntityBatchController_deleteCatalogEntitiesBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/metadata/{id}\n  method: get\n  operationId: CatalogEntityMetadataController_getCatalogEntityMetadataById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/catalog/metadata/{id}\n  method: put\n  operationId: CatalogEntityMetadataController_updateCatalogEntityMetadataById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n  \
  \    proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/relations\n  method: get\n  operationId: CatalogRelationController_getCatalogEntityRelations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/catalog/relations\n  method: post\n  operationId: CatalogRelationController_createCatalogEntityRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/catalog/relations\n  method: delete\n  operationId: CatalogRelationController_deleteCatalogRelationById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /catalog/relations\n  method: get\n  operationId: listCatalogRelations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/relations\n  method: post\n  operationId: createCatalogRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/relations/{id}\n  method: delete\n  operationId: deleteCatalogRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/credentials\n  method: get\n  operationId: CredentialController_getCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/credentials\n  method: post\n  operationId: CredentialController_createCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/credentials/{id}\n  method: put\n  operationId: CredentialController_updateCredential\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/credentials/{id}\n  method: delete\n  operationId: CredentialController_deleteCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/deployments\n  method: post\n  operationId: DeploymentController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/deployments\n  method: get\n  operationId: DeploymentController_getDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/deployments/{id}\n  method: patch\n  operationId: DeploymentController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/deployments/{id}\n  method: delete\n  operationId: DeploymentController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /deployments\n  method: post\n  operationId: recordDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/module-settings/{id}\n  method: get\n  operationId: ModuleSettingsController_getModuleSettingById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/module-settings\n  method: post\n  operationId: ModuleSettingsController_createModuleSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/scim\n  method: patch\n  operationId: ScimController_updateScimConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/scim\n  method: delete\n  operationId: ScimController_deleteScimConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/v1/scim\n  method: get\n  operationId: ScimController_getScimConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/scim/Users/{id}\n  method: get\n  operationId: SCIMController_getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/scim/Users/{id}\n  method: put\n  operationId: SCIMController_putUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v2/scim/Users/{id}\n  method: patch\n  operationId: SCIMController_patchUser\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v2/scim/Users/{id}\n  method: delete\n  operationId: SCIMController_deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v2/scim/Users\n  method: get\n  operationId: SCIMController_getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/scim/Users\n  method: post\n  operationId: SCIMController_createUser\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v2/scim/Groups\n  method: get\n  operationId: SCIMController_getGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/scim/Groups\n  method: post\n  operationId: SCIMController_createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v2/scim/Groups/{id}\n  method:\
  \ get\n  operationId: SCIMController_getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/scim/Groups/{id}\n  method: put\n  operationId: SCIMController_putGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v2/scim/Groups/{id}\n  method: patch\n  operationId: SCIMController_patchGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /public/v2/scim/Groups/{id}\n  method: delete\n  operationId: SCIMController_deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v2/scim/ServiceProviderConfig\n  method: get\n  operationId: SCIMController_getServiceProviderConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/scim/ResourceTypes\n  method: get\n  operationId: SCIMController_getResourceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/scim/Schemas\n  method: get\n  operationId: SCIMController_getSchemas\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/scim/Schemas/{schema}\n  method: get\n  operationId: SCIMController_getSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/scorecards/{id}/run\n  method: post\n  operationId: ScorecardController_createScorecardSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/scorecards\n  method: get\n  operationId: ScorecardController_getScorecards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/scorecards/{id}/metrics\n  method: get\n  operationId: ScorecardController_getMetricsByScorecardId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/scorecards/{id}/results\n  method: get\n  operationId: ScorecardController_getScorecardMetricResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/scorecards/{id}\n  method: put\n  operationId: ScorecardController_updateScorecardById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /public/v1/scorecards/{id}\n  method: get\n  operationId: ScorecardController_getScorecardDefinitionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards\n  method: get\n  operationId: listScorecards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards/{id}\n  method: get\n  operationId: getScorecard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/sync/services/diff\n  method: post\n  operationId: SyncController_getServiceDiff\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/sync/services\n  method: post\n  operationId: SyncController_applyServiceDiff\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/templates\n  method: get\n  operationId: TemplateController_getAllTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method:\
  \ patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/users/{id}\n  method: patch\n  operationId: UserController_updateUserById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /public/v1/users/{id}\n  method: delete\n  operationId: UserController_deleteUserById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v1/users\n  method: get\n  operationId: UserController_getAllUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/agentic-access/configure8-agentic-access.yml
summary_line: 89 operations · 63 acting · 50 human-in-the-loop
tags:
- Catalog
- Cloud Cost
- Developer Experience
- DevOps
- Internal Developer Portal
- Platform Engineering
- Scorecards
- Self-Service
- Service Catalog
- SRE
---
