---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 28
api_specs:
- filename: microsoft-word-body-api-openapi.yml
  format: yaml
  label: Microsoft Word Body API
  slug: microsoft-word-body-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-body-api-openapi.yml
- filename: microsoft-word-checkout-api-openapi.yml
  format: yaml
  label: Microsoft Word Checkout API
  slug: microsoft-word-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-checkout-api-openapi.yml
- filename: microsoft-word-comments-api-openapi.yml
  format: yaml
  label: Microsoft Word Comments API
  slug: microsoft-word-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-comments-api-openapi.yml
- filename: microsoft-word-content-api-openapi.yml
  format: yaml
  label: Microsoft Word Content API
  slug: microsoft-word-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-content-api-openapi.yml
- filename: microsoft-word-content-controls-api-openapi.yml
  format: yaml
  label: Microsoft Word Content Controls API
  slug: microsoft-word-content-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-content-controls-api-openapi.yml
- filename: microsoft-word-documents-api-openapi.yml
  format: yaml
  label: Microsoft Word Documents API
  slug: microsoft-word-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-documents-api-openapi.yml
- filename: microsoft-word-drive-items-api-openapi.yml
  format: yaml
  label: Microsoft Word Drive Items API
  slug: microsoft-word-drive-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-drive-items-api-openapi.yml
- filename: microsoft-word-headers-and-footers-api-openapi.yml
  format: yaml
  label: Microsoft Word Headers And Footers API
  slug: microsoft-word-headers-and-footers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-headers-and-footers-api-openapi.yml
- filename: microsoft-word-images-api-openapi.yml
  format: yaml
  label: Microsoft Word Images API
  slug: microsoft-word-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-images-api-openapi.yml
- filename: microsoft-word-paragraphs-api-openapi.yml
  format: yaml
  label: Microsoft Word Paragraphs API
  slug: microsoft-word-paragraphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-paragraphs-api-openapi.yml
- filename: microsoft-word-permissions-api-openapi.yml
  format: yaml
  label: Microsoft Word Permissions API
  slug: microsoft-word-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-permissions-api-openapi.yml
- filename: microsoft-word-properties-api-openapi.yml
  format: yaml
  label: Microsoft Word Properties API
  slug: microsoft-word-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-properties-api-openapi.yml
- filename: microsoft-word-search-api-openapi.yml
  format: yaml
  label: Microsoft Word Search API
  slug: microsoft-word-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-search-api-openapi.yml
- filename: microsoft-word-sections-api-openapi.yml
  format: yaml
  label: Microsoft Word Sections API
  slug: microsoft-word-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-sections-api-openapi.yml
- filename: microsoft-word-styles-api-openapi.yml
  format: yaml
  label: Microsoft Word Styles API
  slug: microsoft-word-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-styles-api-openapi.yml
- filename: microsoft-word-tables-api-openapi.yml
  format: yaml
  label: Microsoft Word Tables API
  slug: microsoft-word-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-tables-api-openapi.yml
- filename: microsoft-word-thumbnails-api-openapi.yml
  format: yaml
  label: Microsoft Word Thumbnails API
  slug: microsoft-word-thumbnails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-thumbnails-api-openapi.yml
- filename: microsoft-word-versions-api-openapi.yml
  format: yaml
  label: Microsoft Word Versions API
  slug: microsoft-word-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-versions-api-openapi.yml
consequence_counts:
  physical: 2
  read: 28
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Word Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /me/drive/items/{item-id}/checkin
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /me/drive/items/{item-id}/checkout
operation_count: 55
overview: 'Microsoft Word exposes 55 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 25 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Word
provider_slug: microsoft-word
slug: microsoft-word-agentic-access
source_filename: microsoft-word-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-word-graph-api.yaml, openapi/microsoft-word-javascript-api.yaml, openapi/microsoft-word-open-xml-sdk.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    connected: 28\n    acting: 27\n  by_consequence:\n    read: 28\n    write: 25\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /me/drive/items/{item-id}\n  method: get\n  operationId: getDriveItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/drive/items/{item-id}\n  method: patch\n  operationId: updateDriveItem\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}\n  method: delete\n  operationId: deleteDriveItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/children\n  method: get\n  operationId: listChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/drive/items/{item-id}/children\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/content\n  method: get\n  operationId: downloadContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/drive/items/{item-id}/content\n  method: put\n  operationId: uploadContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/copy\n  method: post\n  operationId: copyDriveItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/move\n  method: patch\n  operationId: moveDriveItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/permissions\n  method: get\n  operationId: listPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/drive/items/{item-id}/invite\n  method: post\n  operationId: addPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/createLink\n  method: post\n  operationId: createSharingLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/versions\n  method: get\n  operationId: listVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/drive/items/{item-id}/thumbnails\n  method: get\n  operationId: listThumbnails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/drive/root/search(q='{search-text}')\n\
  \  method: get\n  operationId: searchDriveItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/drive/items/{item-id}/checkin\n  method: post\n  operationId: checkinDriveItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/checkout\n  method: post\n  operationId: checkoutDriveItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/createUploadSession\n  method: post\n  operationId: createUploadSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/preview\n  method: post\n  operationId: previewDriveItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/drive/items/{item-id}/delta\n  method: get\n  operationId: trackChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/body\n  method: get\n  operationId: getBody\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/body/insertText\n  method: post\n  operationId: insertText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/body/insertHtml\n  method: post\n  operationId: insertHtml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/paragraphs\n  method: get\n  operationId: listParagraphs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/paragraphs/{paragraph-id}\n  method: get\n  operationId: getParagraph\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/paragraphs/{paragraph-id}\n  method: delete\n  operationId: deleteParagraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/contentControls\n  method: get\n  operationId: listContentControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/contentControls/{control-id}\n  method: get\n  operationId: getContentControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/tables\n  method: get\n  operationId:\
  \ listTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/tables\n  method: post\n  operationId: insertTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/sections\n  method: get\n  operationId: listSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/properties\n\
  \  method: get\n  operationId: getDocumentProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/properties\n  method: patch\n  operationId: updateDocumentProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/body/search\n  method: post\n  operationId: searchDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/styles\n  method:\
  \ get\n  operationId: listStyles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/save\n  method: post\n  operationId: saveDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: post\n  operationId: createWordDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}\n  method: get\n  operationId: getWordDocument\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}\n  method: delete\n  operationId: deleteWordDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/body\n  method: get\n  operationId: getDocumentBody\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/paragraphs\n  method: get\n  operationId: listDocumentParagraphs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/paragraphs\n  method:\
  \ post\n  operationId: addParagraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/tables\n  method: get\n  operationId: listDocumentTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/tables\n  method: post\n  operationId: addTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/styles\n  method: get\n  operationId: listDocumentStyles\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/headers\n  method: get\n  operationId: listHeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/footers\n  method: get\n  operationId: listFooters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/images\n  method: get\n  operationId: listImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/images\n  method: post\n  operationId: addImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/properties\n  method: get\n  operationId: getOpenXmlProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}/properties\n  method: patch\n  operationId: updateOpenXmlProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document-id}/convert\n  method: post\n  operationId: convertDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/agentic-access/microsoft-word-agentic-access.yml
summary_line: 55 operations · 27 acting
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
---
