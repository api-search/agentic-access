---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 38
api_specs:
- filename: docsmint-com-admin-api-openapi.yml
  format: yaml
  label: docsmint-com Admin API
  slug: docsmint-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-admin-api-openapi.yml
- filename: docsmint-com-attachments-api-openapi.yml
  format: yaml
  label: docsmint-com Attachments API
  slug: docsmint-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-attachments-api-openapi.yml
- filename: docsmint-com-auth-api-openapi.yml
  format: yaml
  label: docsmint-com Auth API
  slug: docsmint-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-auth-api-openapi.yml
- filename: docsmint-com-categories-api-openapi.yml
  format: yaml
  label: docsmint-com Categories API
  slug: docsmint-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-categories-api-openapi.yml
- filename: docsmint-com-csrf-token-api-openapi.yml
  format: yaml
  label: docsmint-com Csrf Token API
  slug: docsmint-com-csrf-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-csrf-token-api-openapi.yml
- filename: docsmint-com-documents-api-openapi.yml
  format: yaml
  label: docsmint-com Documents API
  slug: docsmint-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-documents-api-openapi.yml
- filename: docsmint-com-folders-api-openapi.yml
  format: yaml
  label: docsmint-com Folders API
  slug: docsmint-com-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-folders-api-openapi.yml
- filename: docsmint-com-graph-api-openapi.yml
  format: yaml
  label: docsmint-com Graph API
  slug: docsmint-com-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-graph-api-openapi.yml
- filename: docsmint-com-health-api-openapi.yml
  format: yaml
  label: docsmint-com Health API
  slug: docsmint-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-health-api-openapi.yml
- filename: docsmint-com-keys-api-openapi.yml
  format: yaml
  label: docsmint-com Keys API
  slug: docsmint-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-keys-api-openapi.yml
- filename: docsmint-com-plugins-api-openapi.yml
  format: yaml
  label: docsmint-com Plugins API
  slug: docsmint-com-plugins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-plugins-api-openapi.yml
- filename: docsmint-com-search-api-openapi.yml
  format: yaml
  label: docsmint-com Search API
  slug: docsmint-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-search-api-openapi.yml
- filename: docsmint-com-share-api-openapi.yml
  format: yaml
  label: docsmint-com Share API
  slug: docsmint-com-share-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-share-api-openapi.yml
- filename: docsmint-com-tags-api-openapi.yml
  format: yaml
  label: docsmint-com Tags API
  slug: docsmint-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-tags-api-openapi.yml
- filename: docsmint-com-trash-api-openapi.yml
  format: yaml
  label: docsmint-com Trash API
  slug: docsmint-com-trash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-trash-api-openapi.yml
- filename: docsmint-com-webhooks-api-openapi.yml
  format: yaml
  label: docsmint-com Webhooks API
  slug: docsmint-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsmint-com/openapi/docsmint-com-webhooks-api-openapi.yml
consequence_counts:
  read: 38
  write: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Docsmint Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 82
overview: 'docsmint-com exposes 82 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read and 44 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: docsmint-com
provider_slug: docsmint-com
slug: docsmint-com-agentic-access
source_filename: docsmint-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/docsmint-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 82\n  by_action_class:\n    connected: 38\n    acting: 44\n  by_consequence:\n    read: 38\n    write: 44\n  human_in_the_loop_required: 0\noperations:\n- path: /api/health\n  method: get\n  operationId: getApiHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/csrf-token\n  method: get\n  operationId: getApiCsrf-token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/update-user\n  method:\
  \ post\n  operationId: postApiAuthUpdateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/change-email\n  method: post\n  operationId: postApiAuthChangeEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tags\n  method: get\n  operationId: getApiTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tags\n  method: post\n  operationId: postApiTags\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tags/{id}\n  method: patch\n  operationId: patchApiTagsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tags/{id}\n  method: delete\n  operationId: deleteApiTagsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/tags\n  method: post\n  operationId:\
  \ postApiDocumentsByIdTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/tags/{tagId}\n  method: delete\n  operationId: deleteApiDocumentsByIdTagsByTagId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/categories\n  method: get\n  operationId: getApiCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/categories\n  method: post\n  operationId: postApiCategories\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/categories/{id}\n  method: patch\n  operationId: patchApiCategoriesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/categories/{id}\n  method: delete\n  operationId: deleteApiCategoriesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/attachments/presign\n\
  \  method: post\n  operationId: postApiDocumentsByIdAttachmentsPresign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/attachments/confirm\n  method: post\n  operationId: postApiDocumentsByIdAttachmentsConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/attachments\n  method: post\n  operationId: postApiDocumentsByIdAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/attachments\n  method: get\n  operationId: getApiDocumentsByIdAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/attachments/{id}\n  method: delete\n  operationId: deleteApiAttachmentsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/attachments/{id}/raw\n  method: get\n  operationId: getApiAttachmentsByIdRaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/attachments/remote-image\n\
  \  method: get\n  operationId: getApiAttachmentsRemote-image\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/share/\n  method: post\n  operationId: postApiShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/share/\n  method: get\n  operationId: getApiShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/share/{token}\n  method: get\n  operationId: getApiShareByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/share/{id}\n\
  \  method: delete\n  operationId: deleteApiShareById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/share/{id}\n  method: patch\n  operationId: patchApiShareById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/share/{id}/guests\n  method: post\n  operationId: postApiShareByIdGuests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/share/{id}/guests/{email}\n  method: delete\n  operationId: deleteApiShareByIdGuestsByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/share/{token}/folders/{folderId}\n  method: get\n  operationId: getApiShareByTokenFoldersByFolderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/share/{token}/documents/{docId}\n  method: get\n  operationId: getApiShareByTokenDocumentsByDocId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/\n  method: get\n  operationId: getApiSearch\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/suggest\n  method: get\n  operationId: getApiSearchSuggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents\n  method: get\n  operationId: getApiDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents\n  method: post\n  operationId: postApiDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/cursor\n  method: get\n  operationId:\
  \ getApiDocumentsCursor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents/{id}/pipeline\n  method: get\n  operationId: getApiDocumentsByIdPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents/{id}/pipeline/retry-warnings\n  method: post\n  operationId: retryDocumentPipelineWarnings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/knowledge-summary\n  method: get\n  operationId: getApiDocumentsByIdKnowledgeSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents/{id}/index-status\n  method: get\n  operationId: getApiDocumentsByIdIndexStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents/{id}/index/refresh\n  method: post\n  operationId: postApiDocumentsByIdIndexRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}\n  method: get\n  operationId: getApiDocumentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents/{id}\n  method: patch\n  operationId: patchApiDocumentsById\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}\n  method: delete\n  operationId: deleteApiDocumentsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/duplicate\n  method: post\n  operationId: postApiDocumentsByIdDuplicate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api/trash\n  method: get\n  operationId: getApiTrash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trash/documents/{id}/restore\n  method: post\n  operationId: postApiTrashDocumentsByIdRestore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/trash/documents/{id}\n  method: delete\n  operationId: deleteApiTrashDocumentsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/export\n\
  \  method: get\n  operationId: getApiDocumentsByIdExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents/import\n  method: post\n  operationId: postApiDocumentsImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/folders/{id}\n  method: get\n  operationId: getApiFoldersById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/folders/{id}\n  method: patch\n  operationId: patchApiFoldersById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/folders/{id}\n  method: delete\n  operationId: deleteApiFoldersById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/folders/\n  method: get\n  operationId: getApiFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/folders/\n  method: post\n  operationId: postApiFolders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/versions/\n  method: get\n  operationId: getApiDocumentsByIdVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents/{id}/versions/\n  method: post\n  operationId: postApiDocumentsByIdVersions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/versions/{vid}\n  method: get\n  operationId: getApiDocumentsByIdVersionsByVid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents/{id}/versions/{vid}/restore\n  method: post\n\
  \  operationId: postApiDocumentsByIdVersionsByVidRestore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/versions/diff\n  method: get\n  operationId: getApiDocumentsByIdVersionsDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/storage\n  method: post\n  operationId: postApiWebhooksStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/graph/entities\n  method: get\n  operationId:\
  \ getApiGraphEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/graph/related/{docId}\n  method: get\n  operationId: getApiGraphRelatedByDocId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/graph/search\n  method: post\n  operationId: postApiGraphSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys/global\n  method: post\n  operationId: postApiKeysGlobal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/categories/{id}/keys\n  method: post\n  operationId: postApiCategoriesByIdKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys/{id}/secret\n  method: get\n  operationId: getApiKeysByIdSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: get\n  operationId: getApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys/{id}\n  method: delete\n  operationId: deleteApiKeysById\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/plugins/\n  method: get\n  operationId: getApiPlugins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/plugins/{name}\n  method: get\n  operationId: getApiPluginsByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents/{id}/publish\n  method: post\n  operationId: postApiDocumentsByIdPublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/documents/{id}/unpublish\n  method: post\n  operationId: postApiDocumentsByIdUnpublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/reindex/{docId}\n  method: post\n  operationId: postApiAdminReindexByDocId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/embedding-stats\n  method: get\n  operationId: getApiAdminEmbedding-stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/health/embeddings\n  method: get\n  operationId: getApiAdminHealthEmbeddings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/reindex/model\n  method: post\n  operationId: postApiAdminReindexModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/graph/stats\n  method: get\n  operationId: getApiAdminGraphStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/reindex/folder/{folderId}\n  method: post\n  operationId: postApiAdminReindexFolderByFolderId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/reindex/tag/{tagId}\n  method: post\n  operationId: postApiAdminReindexTagByTagId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/audit\n  method: get\n  operationId: getApiAdminAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/audit/{resourceType}/{resourceId}\n  method: get\n  operationId: getApiAdminAuditByResourceTypeByResourceId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/metrics\n  method: get\n  operationId: getApiAdminMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/docsmint-com/agentic-access/docsmint-com-agentic-access.yml
summary_line: 82 operations · 44 acting
tags:
- Artificial Intelligence
- Document Management
- Knowledge Base
- Software-as-a-Service
- Collaboration
---
