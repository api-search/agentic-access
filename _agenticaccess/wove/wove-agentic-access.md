---
acting_count: 48
action_class_counts:
  acting: 48
  connected: 37
api_specs:
- filename: wove-authentication-api-openapi.yml
  format: yaml
  label: Wove Authentication API
  slug: wove-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-authentication-api-openapi.yml
- filename: wove-documents-api-openapi.yml
  format: yaml
  label: Wove Documents API
  slug: wove-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-documents-api-openapi.yml
- filename: wove-query-bank-api-openapi.yml
  format: yaml
  label: Wove Query Bank API
  slug: wove-query-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-query-bank-api-openapi.yml
- filename: wove-rates-api-openapi.yml
  format: yaml
  label: Wove Rates API
  slug: wove-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-rates-api-openapi.yml
- filename: wove-shipments-api-openapi.yml
  format: yaml
  label: Wove Shipments API
  slug: wove-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-shipments-api-openapi.yml
- filename: wove-sources-api-openapi.yml
  format: yaml
  label: Wove Sources API
  slug: wove-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-sources-api-openapi.yml
- filename: wove-tariffs-api-openapi.yml
  format: yaml
  label: Wove Tariffs API
  slug: wove-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-tariffs-api-openapi.yml
- filename: wove-testing-api-openapi.yml
  format: yaml
  label: Wove Testing API
  slug: wove-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-testing-api-openapi.yml
- filename: wove-tms-organizations-api-openapi.yml
  format: yaml
  label: Wove TMS Organizations API
  slug: wove-tms-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-tms-organizations-api-openapi.yml
- filename: wove-webhooks-api-openapi.yml
  format: yaml
  label: Wove Webhooks API
  slug: wove-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/openapi/wove-webhooks-api-openapi.yml
consequence_counts:
  physical: 27
  read: 37
  safety-critical: 1
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Wove Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/external/auth/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/external/shipments/{shipmentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/external/shipments/{shipmentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/containers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/external/shipments/{shipmentId}/containers/{containerId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/external/shipments/{shipmentId}/containers/{containerId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/external/shipments/{shipmentId}/details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/documents/analyze-types
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/documents/cross-validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/documents/merge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/documents/upload-multi
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/documents/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}/extract
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}/extracted-data
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/external/shipments/{shipmentId}/items/{itemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/external/shipments/{shipmentId}/items/{itemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/items/{itemId}/move
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/external/shipments/{shipmentId}/packages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/external/shipments/{shipmentId}/packages/{packageId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/external/shipments/{shipmentId}/packages/{packageId}
operation_count: 85
overview: 'Wove exposes 85 API operations that an AI agent could call, of which 48 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 20 write, 27 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wove
provider_slug: wove
slug: wove-agentic-access
source_filename: wove-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/wove-authentication-api-openapi.yml, openapi/wove-documents-api-openapi.yml,\n  openapi/wove-query-bank-api-openapi.yml, openapi/wove-rates-api-openapi.yml, openapi/wove-shipments-api-openapi.yml,\n  openapi/wove-sources-api-openapi.yml, openapi/wove-tariffs-api-openapi.yml, openapi/wove-testing-api-openapi.yml,\n  openapi/wove-tms-organizations-api-openapi.yml, openapi/wove-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 85\n  by_action_class:\n    acting: 48\n    connected: 37\n  by_consequence:\n    write: 20\n    safety-critical: 1\n    read: 37\n    physical: 27\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/external/auth/token\n  method:\
  \ post\n  operationId: postApiV1ExternalAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/auth/revoke\n  method: post\n  operationId: postApiV1ExternalAuthRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/documents\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdDocumentsByDocumentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}\n  method: put\n  operationId: putApiV1ExternalShipmentsByShipmentIdDocumentsByDocumentId\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}\n  method: delete\n  operationId: deleteApiV1ExternalShipmentsByShipmentIdDocumentsByDocumentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}/download\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdDocumentsByDocumentIdDownload\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}/extraction\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdDocumentsByDocumentIdExtraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}/extract\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdDocumentsByDocumentIdExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}/extracted-data\n\
  \  method: put\n  operationId: putApiV1ExternalShipmentsByShipmentIdDocumentsByDocumentIdExtractedData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents/{documentId}/history\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdDocumentsByDocumentIdHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/documents/validate\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdDocumentsValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents/cross-validate/{jobId}\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdDocumentsCrossValidateByJobId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/documents/merge/{jobId}\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdDocumentsMergeByJobId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/documents/cross-validate\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdDocumentsCrossValidate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents/merge\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdDocumentsMerge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents/analyze-types\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdDocumentsAnalyzeTypes\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/documents/upload-multi\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdDocumentsUploadMulti\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/entities/{entityType}/{entityId}/documents\n  method: get\n  operationId: getApiV1ExternalEntitiesByEntityTypeByEntityIdDocuments\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/entities/{entityType}/{entityId}/documents\n  method: post\n  operationId: postApiV1ExternalEntitiesByEntityTypeByEntityIdDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/entities/{entityType}/{entityId}/documents/multi\n  method: post\n  operationId: postApiV1ExternalEntitiesByEntityTypeByEntityIdDocumentsMulti\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/entities/{entityType}/{entityId}/documents/{documentId}\n\
  \  method: get\n  operationId: getApiV1ExternalEntitiesByEntityTypeByEntityIdDocumentsByDocumentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/entities/{entityType}/{entityId}/documents/{documentId}\n  method: put\n  operationId: putApiV1ExternalEntitiesByEntityTypeByEntityIdDocumentsByDocumentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/entities/{entityType}/{entityId}/documents/{documentId}\n  method: delete\n  operationId: deleteApiV1ExternalEntitiesByEntityTypeByEntityIdDocumentsByDocumentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/entities/{entityType}/{entityId}/documents/{documentId}/download\n  method: get\n  operationId: getApiV1ExternalEntitiesByEntityTypeByEntityIdDocumentsByDocumentIdDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/entities/{entityType}/{entityId}/documents/{documentId}/preview\n  method: get\n  operationId: getApiV1ExternalEntitiesByEntityTypeByEntityIdDocumentsByDocumentIdPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/entities/{entityType}/{entityId}/documents/{documentId}/history\n  method: get\n  operationId: getApiV1ExternalEntitiesByEntityTypeByEntityIdDocumentsByDocumentIdHistory\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/documents/guess-type\n  method: post\n  operationId: postApiV1ExternalDocumentsGuessType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/query-bank/sources\n  method: get\n  operationId: getApiV1ExternalQueryBankSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/query-bank/sources\n  method: post\n  operationId: postApiV1ExternalQueryBankSources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/query-bank/sources/{sourceId}\n  method: delete\n  operationId: deleteApiV1ExternalQueryBankSourcesBySourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/rates/query\n  method: post\n  operationId: postApiV1ExternalRatesQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments\n  method: get\n  operationId: getApiV1ExternalShipments\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments\n  method: post\n  operationId: postApiV1ExternalShipments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}\n  method: put\n  operationId: putApiV1ExternalShipmentsByShipmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}\n  method: delete\n  operationId: deleteApiV1ExternalShipmentsByShipmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/details\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/details\n\
  \  method: put\n  operationId: putApiV1ExternalShipmentsByShipmentIdDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/events\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/validation-items\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdValidationItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/validation-items/{itemId}\n\
  \  method: put\n  operationId: putApiV1ExternalShipmentsByShipmentIdValidationItemsByItemId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/validation-items/bulk-update\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdValidationItemsBulkUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/jobs\n  method: get\n\
  \  operationId: getApiV1ExternalShipmentsByShipmentIdJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/containers\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdContainers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/containers\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdContainers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/containers/{containerId}\n\
  \  method: put\n  operationId: putApiV1ExternalShipmentsByShipmentIdContainersByContainerId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/containers/{containerId}\n  method: delete\n  operationId: deleteApiV1ExternalShipmentsByShipmentIdContainersByContainerId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/packages\n  method: get\n\
  \  operationId: getApiV1ExternalShipmentsByShipmentIdPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/packages\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdPackages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/packages/{packageId}\n  method: put\n  operationId: putApiV1ExternalShipmentsByShipmentIdPackagesByPackageId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/packages/{packageId}\n  method: delete\n  operationId: deleteApiV1ExternalShipmentsByShipmentIdPackagesByPackageId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/packages/{packageId}/move\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdPackagesByPackageIdMove\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/items\n  method: get\n  operationId: getApiV1ExternalShipmentsByShipmentIdItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/shipments/{shipmentId}/items\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/items/{itemId}\n  method: put\n  operationId: putApiV1ExternalShipmentsByShipmentIdItemsByItemId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/items/{itemId}\n  method: delete\n  operationId: deleteApiV1ExternalShipmentsByShipmentIdItemsByItemId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/shipments/{shipmentId}/items/{itemId}/move\n  method: post\n  operationId: postApiV1ExternalShipmentsByShipmentIdItemsByItemIdMove\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/sources/upload\n  method: post\n  operationId: postApiV1ExternalSourcesUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/sources/{sourceId}/process\n  method: post\n  operationId: postApiV1ExternalSourcesBySourceIdProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/sources\n  method: get\n  operationId: getApiV1ExternalSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/sources/{sourceId}\n  method: get\n  operationId: getApiV1ExternalSourcesBySourceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/tariffs/lookup\n  method: get\n  operationId: getApiV1ExternalTariffsLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/tariffs/search\n  method: get\n  operationId: getApiV1ExternalTariffsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/tariffs/batch-lookup\n  method: post\n  operationId: postApiV1ExternalTariffsBatchLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/test/ping\n  method: get\n  operationId: getApiV1ExternalTestPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/test/rate-limit-status\n  method: get\n  operationId: getApiV1ExternalTestRateLimitStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/test/protected\n  method:\
  \ get\n  operationId: getApiV1ExternalTestProtected\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - shipments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/test/api-usage-status\n  method: get\n  operationId: getApiV1ExternalTestApiUsageStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/tms/organizations\n  method: get\n  operationId: getApiV1ExternalTmsOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/tms/organizations\n  method: post\n  operationId: postApiV1ExternalTmsOrganizations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/tms/organizations/{organizationId}\n  method: get\n  operationId: getApiV1ExternalTmsOrganizationsByOrganizationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/tms/organizations/{organizationId}\n  method: put\n  operationId: putApiV1ExternalTmsOrganizationsByOrganizationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/tms/organizations/{organizationId}\n  method: delete\n  operationId: deleteApiV1ExternalTmsOrganizationsByOrganizationId\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/tms/organizations/import\n  method: post\n  operationId: postApiV1ExternalTmsOrganizationsImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/tms/organizations/import/{jobId}\n  method: get\n  operationId: getApiV1ExternalTmsOrganizationsImportByJobId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/webhooks\n  method: get\n  operationId:\
  \ getApiV1ExternalWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/webhooks\n  method: post\n  operationId: postApiV1ExternalWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/webhooks/{webhookId}\n  method: get\n  operationId: getApiV1ExternalWebhooksByWebhookId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/external/webhooks/{webhookId}\n  method: put\n  operationId: putApiV1ExternalWebhooksByWebhookId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/webhooks/{webhookId}\n  method: delete\n  operationId: deleteApiV1ExternalWebhooksByWebhookId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/webhooks/{webhookId}/test\n  method: post\n  operationId: postApiV1ExternalWebhooksByWebhookIdTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/external/webhooks/test\n  method: post\n  operationId: postApiV1ExternalWebhooksTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/external/webhooks/{webhookId}/deliveries\n  method: get\n  operationId: getApiV1ExternalWebhooksByWebhookIdDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/agentic-access/wove-agentic-access.yml
summary_line: 85 operations · 48 acting · 1 human-in-the-loop
tags:
- Company
---
