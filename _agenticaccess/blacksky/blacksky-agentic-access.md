---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 38
api_specs:
- filename: blacksky-budgets-api-openapi.yml
  format: yaml
  label: BlackSky Budgets API
  slug: blacksky-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-budgets-api-openapi.yml
- filename: blacksky-catalog-api-openapi.yml
  format: yaml
  label: BlackSky Catalog API
  slug: blacksky-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-catalog-api-openapi.yml
- filename: blacksky-data-management-api-openapi.yml
  format: yaml
  label: BlackSky Data management API
  slug: blacksky-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-data-management-api-openapi.yml
- filename: blacksky-eulas-api-openapi.yml
  format: yaml
  label: BlackSky EULAs API
  slug: blacksky-eulas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-eulas-api-openapi.yml
- filename: blacksky-geometries-api-openapi.yml
  format: yaml
  label: BlackSky Geometries API
  slug: blacksky-geometries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-geometries-api-openapi.yml
- filename: blacksky-glossary-api-openapi.yml
  format: yaml
  label: BlackSky Glossary API
  slug: blacksky-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-glossary-api-openapi.yml
- filename: blacksky-orders-api-openapi.yml
  format: yaml
  label: BlackSky Orders API
  slug: blacksky-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-orders-api-openapi.yml
- filename: blacksky-processing-api-openapi.yml
  format: yaml
  label: BlackSky Processing API
  slug: blacksky-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-processing-api-openapi.yml
- filename: blacksky-tasking-api-openapi.yml
  format: yaml
  label: BlackSky Tasking API
  slug: blacksky-tasking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-tasking-api-openapi.yml
consequence_counts:
  physical: 7
  read: 38
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blacksky Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/estimate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/validation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/orders/{order-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/{order-id}/cancellation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/tasking/orders/feasibility
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/tasking/{order-id}/extensions
operation_count: 57
overview: 'BlackSky exposes 57 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 12 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BlackSky
provider_slug: blacksky
slug: blacksky-agentic-access
source_filename: blacksky-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/blacksky-up42-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 38\n    acting: 19\n  by_consequence:\n    read: 38\n    write: 12\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /catalog/hosts/{host-name}/stac/search\n  method: post\n  operationId: searchByHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{host-name}/image/{image-id}/quicklook\n  method: get\n  operationId: getQuicklookImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{host-name}/image/{image-id}/thumbnail\n  method: get\n  operationId: getThumbnailImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/schema/{data-product-id}\n  method: get\n  operationId: getJSONSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/stac\n  method: get\n  operationId: getSASLandingPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/stac/collections\n  method: get\n  operationId: getSASCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/stac/collections/{collection-id}\n\
  \  method: get\n  operationId: getSASCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/stac/collections/{collection-id}\n  method: delete\n  operationId: deleteSASCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/stac/collections/{collection-id}/items\n  method: get\n  operationId: getSASItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/stac/collections/{collection-id}/items/{item-id}\n  method: get\n  operationId: getSASItem\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/stac/collections/{collection-id}/items/{item-id}\n  method: patch\n  operationId: patchSASItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/stac/queryables\n  method: get\n  operationId: getSASQueryables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/stac/search\n  method: post\n  operationId: postSASSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/{asset-id}/download-url\n  method: post\n  operationId:\
  \ generateDownloadUrlExternal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/budgets\n  method: get\n  operationId: listBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account\n    - budget.r\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/budgets/settings\n  method: get\n  operationId: getBudgetSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account\n    - budget.r\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/budgets/{budget-id}\n  method: get\n  operationId: getBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - account\n    - budget.r\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/budgets/{budget-id}/usage\n  method: get\n  operationId: getBudgetUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account\n    - budget.r\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/collections\n  method: get\n  operationId: listCollectionsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/collections/{collection-name}\n  method: get\n  operationId: getCollectionV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coverage/orders/{order-id}\n  method: get\n  operationId: getOrderCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/data-products\n  method: get\n  operationId: listDataProductsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/data-products/{data-product-name}\n  method: get\n  operationId: getDataProductV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/eulas\n  method: get\n  operationId: listEulasV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/eulas/{eula-id}\n  method: get\n  operationId: getEulaV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/eulas/{eula-id}/documents\n  method: get\n  operationId: listEulaDocumentsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/eulas/{eula-id}/documents/{eula-document-id}\n  method: get\n  operationId: getEulaDocumentV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/eulas/{eula-id}/documents/{eula-document-id}\n  method: patch\n  operationId: acceptEulaDocumentV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account\n    - eula.w\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders\n  method: get\n\
  \  operationId: listOrdersV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders\n  method: post\n  operationId: createV2OrderUnderWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/estimate\n  method: post\n  operationId: estimateV2Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v2/orders/validation\n  method: post\n  operationId: validateV2Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{order-id}\n  method: get\n  operationId: getOrderV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/{order-id}\n  method: patch\n  operationId: patchOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/orders/{order-id}/cancellation\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/processing/jobs\n  method: get\n  operationId: processing.getJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/processing/jobs/{job-id}\n  method: get\n  operationId: processing.getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/processing/processes\n  method: get\n  operationId: processing.getProcesses\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/processing/processes/{process-id}\n  method: get\n  operationId: processing.getProcess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/processing/processes/{process-id}/cost\n  method: post\n  operationId: processing.evaluate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/processing/processes/{process-id}/execution\n  method: post\n  operationId: processing.execute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/processing/processes/{process-id}/validation\n  method: post\n  operationId: processing.validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/providers\n  method: get\n  operationId: listProvidersV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/providers/{provider-name}\n  method: get\n  operationId: getProviderV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/spatial/geometries\n\
  \  method: get\n  operationId: listGeometries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/spatial/geometries\n  method: post\n  operationId: addGeometry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/spatial/geometries/{geometry-id}\n  method: get\n  operationId: getGeometry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/spatial/geometries/{geometry-id}\n  method: delete\n  operationId: deleteGeometry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/spatial/geometries/{geometry-id}\n  method: patch\n  operationId: patchGeometry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasking/feasibility-studies\n  method: get\n  operationId: listTaskingFeasibilityStudies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasking/feasibility-studies/{feasibility-study-id}\n  method: patch\n  operationId: updateTaskingFeasibilityStudy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasking/orders/feasibility\n  method: post\n  operationId: checkOrderFeasibility\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasking/orders/opportunities\n  method: post\n  operationId: listV2TaskingOrderOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasking/quotation\n  method: get\n  operationId: listTaskingQuotation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasking/quotation/{quotation-id}\n  method: patch\n  operationId: updateTaskingQuotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasking/{order-id}/extensions\n  method: get\n  operationId: getOrderAcquisitionDateExtensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasking/{order-id}/extensions\n  method: post\n  operationId: createExtensionRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/agentic-access/blacksky-agentic-access.yml
summary_line: 57 operations · 19 acting
tags:
- Earth Observation
- Satellite Imagery
- Remote Sensing
- Geospatial Intelligence
- Space
- ISR
- Intelligence Surveillance Reconnaissance
- Tasking
- AI Analytics
- Object Detection
- Defense
- Monitoring
- Spectra
- Gen-3
- NYSE BKSY
---
