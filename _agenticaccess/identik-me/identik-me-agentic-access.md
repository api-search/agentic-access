---
acting_count: 139
action_class_counts:
  acting: 139
  connected: 69
api_specs:
- filename: identik-me-document-api-openapi.yml
  format: yaml
  label: identik-me Document API
  slug: identik-me-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-document-api-openapi.yml
- filename: identik-me-document-fields-api-openapi.yml
  format: yaml
  label: identik-me Document Fields API
  slug: identik-me-document-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-document-fields-api-openapi.yml
- filename: identik-me-document-recipients-api-openapi.yml
  format: yaml
  label: identik-me Document Recipients API
  slug: identik-me-document-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-document-recipients-api-openapi.yml
- filename: identik-me-documents-api-openapi.yml
  format: yaml
  label: identik-me Documents API
  slug: identik-me-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-documents-api-openapi.yml
- filename: identik-me-embedding-api-openapi.yml
  format: yaml
  label: identik-me Embedding API
  slug: identik-me-embedding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-embedding-api-openapi.yml
- filename: identik-me-envelope-api-openapi.yml
  format: yaml
  label: identik-me Envelope API
  slug: identik-me-envelope-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-api-openapi.yml
- filename: identik-me-envelope-attachments-api-openapi.yml
  format: yaml
  label: identik-me Envelope Attachments API
  slug: identik-me-envelope-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-attachments-api-openapi.yml
- filename: identik-me-envelope-fields-api-openapi.yml
  format: yaml
  label: identik-me Envelope Fields API
  slug: identik-me-envelope-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-fields-api-openapi.yml
- filename: identik-me-envelope-items-api-openapi.yml
  format: yaml
  label: identik-me Envelope Items API
  slug: identik-me-envelope-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-items-api-openapi.yml
- filename: identik-me-envelope-recipients-api-openapi.yml
  format: yaml
  label: identik-me Envelope Recipients API
  slug: identik-me-envelope-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-recipients-api-openapi.yml
- filename: identik-me-firma-masiva-api-openapi.yml
  format: yaml
  label: identik-me Firma masiva API
  slug: identik-me-firma-masiva-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-firma-masiva-api-openapi.yml
- filename: identik-me-folder-api-openapi.yml
  format: yaml
  label: identik-me Folder API
  slug: identik-me-folder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-folder-api-openapi.yml
- filename: identik-me-representation-api-openapi.yml
  format: yaml
  label: identik-me Representation API
  slug: identik-me-representation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-representation-api-openapi.yml
- filename: identik-me-template-api-openapi.yml
  format: yaml
  label: identik-me Template API
  slug: identik-me-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-template-api-openapi.yml
- filename: identik-me-template-fields-api-openapi.yml
  format: yaml
  label: identik-me Template Fields API
  slug: identik-me-template-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-template-fields-api-openapi.yml
- filename: identik-me-template-recipients-api-openapi.yml
  format: yaml
  label: identik-me Template Recipients API
  slug: identik-me-template-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-template-recipients-api-openapi.yml
- filename: identik-me-templates-api-openapi.yml
  format: yaml
  label: identik-me Templates API
  slug: identik-me-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-templates-api-openapi.yml
consequence_counts:
  physical: 4
  read: 69
  safety-critical: 2
  write: 133
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Identik Me Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /representation/authority/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /representation/authority/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/documents/{id}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/documents/{id}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/documents/{id}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/documents/{id}/send
operation_count: 208
overview: 'identik-me exposes 208 API operations that an AI agent could call, of which 139 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 69 read, 133 write, 4 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: identik-me
provider_slug: identik-me
slug: identik-me-agentic-access
source_filename: identik-me-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/electronica-v1-openapi.json, openapi/firma-docs-openapi-v2.json, openapi/firma-v1-openapi.json,\n  openapi/firma-v2-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 208\n  by_action_class:\n    connected: 69\n    acting: 139\n  by_consequence:\n    read: 69\n    write: 133\n    physical: 4\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /api/v1/documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/download\n  method: get\n  operationId: downloadSignedDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates\n  method: post\n  operationId: createTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates\n  method: get\n  operationId: getTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/{id}\n  method: delete\n  operationId: deleteTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{id}\n\
  \  method: get\n  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/{templateId}/create-document\n  method: post\n  operationId: createDocumentFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{templateId}/generate-document\n  method: post\n  operationId: generateDocumentFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/send\n\
  \  method: post\n  operationId: sendDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/resend\n  method: post\n  operationId: resendDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/recipients\n  method: post\n  operationId: createRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/recipients/{recipientId}\n  method: patch\n  operationId: updateRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/recipients/{recipientId}\n  method: delete\n  operationId: deleteRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/fields\n  method: post\n  operationId:\
  \ createField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/fields/{fieldId}\n  method: patch\n  operationId: updateField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/fields/{fieldId}\n  method: delete\n  operationId: deleteField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api/v2/envelope/{envelopeId}/audit-log\n  method: get\n  operationId: getEnvelopeAuditLogV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/document/{documentId}/download\n  method: get\n  operationId: downloadDocumentV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/document/{documentId}/certificate\n  method: get\n  operationId: downloadDocumentCertificateV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /envelope/{envelopeId}/audit-log\n  method: get\n  operationId: envelope-auditLog-find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /document/{documentId}\n  method: get\n  operationId: document-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document\n  method: get\n  operationId: document-find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document/create\n  method: post\n  operationId: document-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/update\n  method: post\n  operationId: document-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/delete\n  method: post\n  operationId: document-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/distribute\n  method: post\n  operationId: document-distribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/redistribute\n  method: post\n  operationId: document-redistribute\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/{documentId}/download\n  method: get\n  operationId: document-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document/field/create\n  method: post\n  operationId: field-createDocumentField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/field/create-many\n  method: post\n  operationId: field-createDocumentFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/field/update\n  method: post\n  operationId: field-updateDocumentField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/field/delete\n  method: post\n  operationId: field-deleteDocumentField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/recipient/create\n  method: post\n  operationId:\
  \ recipient-createDocumentRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/recipient/update\n  method: post\n  operationId: recipient-updateDocumentRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/recipient/delete\n  method: post\n  operationId: recipient-deleteDocumentRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/{documentId}/representation/evidence\n  method: get\n  operationId: representationApi-listEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /representation/config\n  method: get\n  operationId: representationApi-config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /representation/terms/accept\n  method: post\n  operationId: representationApi-acceptTerms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /representation/entity\n  method: get\n  operationId:\
  \ representationApi-listEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /representation/entity/{entityId}\n  method: get\n  operationId: representationApi-getEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /representation/entity/create\n  method: post\n  operationId: representationApi-createApiEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /representation/entity/update\n  method: post\n  operationId: representationApi-updateApiEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /representation/entity/{entityId}/documents\n  method: get\n  operationId: representationApi-listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /representation/document/{documentId}\n  method: get\n  operationId: representationApi-getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /representation/document/upload\n  method: post\n  operationId: representationApi-uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /representation/document/retry\n  method: post\n  operationId: representationApi-retryDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /representation/document/delete\n  method: post\n  operationId: representationApi-deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /representation/entity/{entityId}/authorities\n  method: get\n  operationId: representationApi-listAuthorities\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /representation/authority/create\n  method: post\n  operationId: representationApi-addAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /representation/authority/confirm\n  method: post\n  operationId: representationApi-confirmApiAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /representation/authority/revoke\n  method: post\n  operationId: representationApi-revokeApiAuthority\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /document/{documentId}/representation\n  method: get\n  operationId: representationApi-getEnvelope\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document/representation/configure\n  method: post\n  operationId: representationApi-configureEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/representation/assign\n  method: post\n  operationId:\
  \ representationApi-assignRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/representation/confirm\n  method: post\n  operationId: representationApi-confirmRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/create\n  method: post\n  operationId: batchApi-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /batch/{batchId}/start\n  method: post\n  operationId: batchApi-start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/{batchId}\n  method: get\n  operationId: batchApi-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch\n  method: get\n  operationId: batchApi-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/{batchId}/reauthorize\n  method: post\n  operationId: batchApi-reauthorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/{batchId}/cancel\n  method: post\n  operationId: batchApi-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template\n  method: get\n  operationId: template-findTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /template/{templateId}\n  method: get\n  operationId: template-getTemplateById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /template/create\n  method: post\n  operationId: template-createTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/update\n  method: post\n  operationId: template-updateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/delete\n  method: post\n  operationId: template-deleteTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/use\n  method: post\n  operationId: template-createDocumentFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/{documentId}/representation/evidence/{evidenceId}/download\n  method: get\n  operationId: representationApi-downloadEnvelopeEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /representation/document/{documentId}/download\n  method: get\n  operationId: representationApi-downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /document/{documentId}/certificate\n  method: get\n  operationId: downloadDocumentCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/download\n  method: get\n  operationId: downloadSignedDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates\n  method: post\n  operationId: createTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /api/v1/templates\n  method: get\n  operationId: getTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/{id}\n  method: delete\n  operationId: deleteTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{id}\n  method: get\n  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/{templateId}/create-document\n  method: post\n  operationId: createDocumentFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{templateId}/generate-document\n  method: post\n  operationId: generateDocumentFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/send\n  method: post\n  operationId: sendDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/documents/{id}/resend\n  method: post\n  operationId: resendDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/recipients\n  method: post\n  operationId: createRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/recipients/{recipientId}\n  method: patch\n  operationId: updateRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/recipients/{recipientId}\n  method: delete\n  operationId: deleteRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/fields\n  method: post\n  operationId: createField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/fields/{fieldId}\n  method: patch\n  operationId: updateField\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}/fields/{fieldId}\n  method: delete\n  operationId: deleteField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/envelope/{envelopeId}/audit-log\n  method: get\n  operationId: getEnvelopeAuditLogV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/document/{documentId}/download\n  method: get\n  operationId: downloadDocumentV2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/document/{documentId}/certificate\n  method: get\n  operationId: downloadDocumentCertificateV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /envelope/attachment\n  method: get\n  operationId: envelope-attachment-find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /envelope/attachment/create\n  method: post\n  operationId: envelope-attachment-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /envelope/attachment/update\n\
  \  method: post\n  operationId: envelope-attachment-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /envelope/attachment/delete\n  method: post\n  operationId: envelope-attachment-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /envelope/item/create-many\n  method: post\n  operationId: envelope-item-createMany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /envelope/item/update-many\n  method: post\n  operationId: envelope-item-updateMany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /envelope/item/delete\n  method: post\n  operationId: envelope-item-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /envelope/item/{envelopeItemId}/download\n  method: get\n  operationId: envelope-item-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (64 KB total) ---\n# Full source: https://artifacts.apis.io/identik-me/agentic-access/identik-me-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/identik-me/agentic-access/identik-me-agentic-access.yml
summary_line: 208 operations · 139 acting · 2 human-in-the-loop
tags:
- Company
- Digital Signature
- Document Automation
- Argentina
---
