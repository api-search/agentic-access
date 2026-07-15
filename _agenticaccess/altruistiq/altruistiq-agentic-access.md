---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 15
api_specs:
- filename: altruistiq-openapi.yml
  format: yaml
  label: Altruistiq Datasource API
  slug: altruistiq-datasource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-openapi.yml
- filename: altruistiq-openapi.yml
  format: yaml
  label: Altruistiq PACT API
  slug: altruistiq-pact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-openapi.yml
consequence_counts:
  read: 15
  safety-critical: 25
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 25
kind: agentic-access
layout: agentic-access
method: generated
name: Altruistiq Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/public/v1/facilities/bulk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/public/v1/facilities/{facilityId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/public/v1/facilities/{facilityId}/persistent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/public/v1/facilities/{facilityId}/versions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/public/v1/facilities/{facilityId}/versions/{versionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/public/v1/facilities/{facilityId}/versions/{versionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/public/v1/product-structure-inputs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/public/v1/product-structure-inputs/bulk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/public/v1/product-structure-inputs/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/public/v1/product-structure-inputs/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/public/v1/product-structures
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/public/v1/product-structures/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/public/v1/product-structures/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/public/v1/product-structures/{structureId}/inputs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/public/v1/product-structures/{structureId}/inputs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/public/v1/product-structures/{structureId}/inputs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/public/v1/products
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/public/v1/products
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/public/v1/products
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/public/v1/products/bulk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/public/v1/products/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/public/v1/products/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/public/v1/products/{productId}/structures
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/public/v1/products/{productId}/structures
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/public/v1/products/{productId}/structures
operation_count: 44
overview: 'Altruistiq exposes 44 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 4 write, and 25 safety-critical.


  25 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Altruistiq
provider_slug: altruistiq
slug: altruistiq-agentic-access
source_filename: altruistiq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/altruistiq-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    acting: 29\n    connected: 15\n  by_consequence:\n    write: 4\n    read: 15\n    safety-critical: 25\n  human_in_the_loop_required: 25\noperations:\n- path: /api/public/v1/oauth2/token\n  method: post\n  operationId: getOauth2Token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/v1/datasource/{dataSourceId}/upload\n  method: get\n  operationId:\
  \ startMultipartUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/datasource/{dataSourceId}/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/v1/datasource/{dataSourceId}/upload/{uploadId}/file/{fileId}/complete\n  method: post\n  operationId: completeFileUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/v1/export\n  method:\
  \ post\n  operationId: createExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/v1/export/{exportId}\n  method: get\n  operationId: getDownloadUrls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/products\n  method: post\n  operationId: PublicProductController.createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/products\n\
  \  method: get\n  operationId: PublicProductsController.bulkGetProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/products\n  method: patch\n  operationId: PublicProductsController.bulkUpdateProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/products\n  method: delete\n  operationId: PublicProductsController.bulkDeleteProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/products/{id}\n  method: get\n  operationId: PublicProductController.getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/products/{id}\n  method: patch\n  operationId: PublicProductController.updateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/products/{id}\n  method: delete\n  operationId: PublicProductController.deleteProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n   \
  \   exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/products/bulk\n  method: post\n  operationId: PublicProductsController.bulkCreateProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/product-structures\n  method: post\n  operationId: PublicStructureController.createSingleStructure\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/public/v1/product-structures/{id}\n  method: get\n  operationId: PublicStructureController.getSingleStructure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/product-structures/{id}\n  method: patch\n  operationId: PublicStructureController.updateSingleStructure\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/product-structures/{id}\n  method: delete\n  operationId: PublicStructureController.deleteSingleStructure\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/products/{productId}/structures\n  method: post\n  operationId: PublicStructuresController.bulkCreateStructures\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/products/{productId}/structures\n  method: get\n  operationId: PublicStructuresController.bulkGetStructures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/products/{productId}/structures\n  method: patch\n  operationId: PublicStructuresController.bulkUpdateStructures\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/products/{productId}/structures\n  method: delete\n  operationId: PublicStructuresController.bulkDeleteStructures\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/product-structure-inputs\n  method: post\n  operationId: PublicStructureInputController.createSingleStructureInput\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/product-structure-inputs/{id}\n  method: get\n  operationId: PublicStructureInputController.getSingleStructureInput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/product-structure-inputs/{id}\n  method: patch\n  operationId: PublicStructureInputController.updateSingleStructureInput\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/product-structure-inputs/{id}\n\
  \  method: delete\n  operationId: PublicStructureInputController.deleteSingleStructureInput\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/product-structures/{structureId}/inputs\n  method: post\n  operationId: PublicStructureInputsController.bulkCreateStructureInputs\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/product-structures/{structureId}/inputs\n  method: get\n  operationId: PublicStructureInputsController.bulkGetStructureInputs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/product-structures/{structureId}/inputs\n  method: patch\n  operationId: PublicStructureInputsController.bulkUpdateStructureInputs\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/product-structures/{structureId}/inputs\n  method: delete\n  operationId: PublicStructureInputsController.bulkDeleteStructureInputs\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/product-structure-inputs/bulk\n  method: post\n  operationId: PublicStructureInputsController.bulkCreateInputs\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/facilities/\n  method: get\n  operationId: FacilitiesPublicController.getFacilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/facilities/{facilityId}\n  method: get\n  operationId: FacilitiesPublicController.getFacility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/facilities/{facilityId}\n  method: delete\n  operationId: FacilitiesPublicController.deleteFacility\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/facilities/{facilityId}/versions/{versionId}\n  method: get\n  operationId: FacilitiesPublicController.getFacilityVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/facilities/{facilityId}/versions/{versionId}\n  method: delete\n  operationId: FacilitiesPublicController.deleteFacilityVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/facilities/{facilityId}/versions/{versionId}\n  method: patch\n  operationId: FacilitiesPublicController.updateFacilityVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/facilities/bulk\n  method: post\n  operationId: FacilitiesPublicController.bulkInsertFacilities\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n  \
  \    purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/facilities/{facilityId}/persistent\n  method: patch\n  operationId: FacilitiesPublicController.updateFacilityPersistent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/public/v1/facilities/{facilityId}/versions\n  method: post\n  operationId: FacilitiesPublicController.createFacilityVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/public/v1/facilities/types\n  method: get\n  operationId: FacilitiesPublicController.getFacilityTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/location/countries\n  method: get\n  operationId: LocationController.getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/location/countries/{countryCode}/subdivisions\n  method: get\n  operationId: LocationController.getCountrySubdivisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/organization/\n  method: get\n  operationId: OrganizationPublicController.getOrganization\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/agentic-access/altruistiq-agentic-access.yml
summary_line: 44 operations · 29 acting · 25 human-in-the-loop
tags:
- Sustainability
- Climate
- Carbon Accounting
- Emissions
- Greenhouse Gas
- Scope 3
- Product Carbon Footprint
- Corporate Carbon Footprint
- Supply Chain
- FMCG
- Food and Beverage
- ESG
- CSRD
- SBTi
- PACT
- Sustainability Intelligence
---
