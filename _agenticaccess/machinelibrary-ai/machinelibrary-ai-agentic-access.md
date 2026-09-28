---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 24
api_specs:
- filename: machinelibrary-ai-documents-api-openapi.yml
  format: yaml
  label: Space Frontiers Documents API
  slug: machinelibrary-ai-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-documents-api-openapi.yml
- filename: machinelibrary-ai-payments-api-openapi.yml
  format: yaml
  label: Space Frontiers Payments API
  slug: machinelibrary-ai-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-payments-api-openapi.yml
- filename: machinelibrary-ai-raw-document-downloads-api-openapi.yml
  format: yaml
  label: Space Frontiers Raw document downloads API
  slug: machinelibrary-ai-raw-document-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-raw-document-downloads-api-openapi.yml
- filename: machinelibrary-ai-recognition-api-openapi.yml
  format: yaml
  label: Space Frontiers Recognition API
  slug: machinelibrary-ai-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-recognition-api-openapi.yml
- filename: machinelibrary-ai-search-api-openapi.yml
  format: yaml
  label: Space Frontiers Search API
  slug: machinelibrary-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-search-api-openapi.yml
- filename: machinelibrary-ai-conversations-api-openapi.yml
  format: yaml
  label: Space Frontiers Conversations API
  slug: machinelibrary-ai-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-conversations-api-openapi.yml
consequence_counts:
  physical: 2
  read: 24
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Machinelibrary Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payments/mpp/top-up
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payments/mpp/top-up
operation_count: 42
overview: 'Space Frontiers exposes 42 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 16 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Space Frontiers
provider_slug: machinelibrary-ai
slug: machinelibrary-ai-agentic-access
source_filename: machinelibrary-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: generated\nsource: openapi/machinelibrary-ai-conversations-api-openapi.json, openapi/machinelibrary-ai-conversations-api-openapi.yml,\n  openapi/machinelibrary-ai-documents-api-openapi.yml, openapi/machinelibrary-ai-payments-api-openapi.yml,\n  openapi/machinelibrary-ai-raw-document-downloads-api-openapi.yml, openapi/machinelibrary-ai-recognition-api-openapi.yml,\n  openapi/machinelibrary-ai-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 24\n    acting: 18\n  by_consequence:\n    read: 24\n    write: 16\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/conversations/\n  method: get\n  operationId: listConversations\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conversations/\n  method: post\n  operationId: createConversationTurn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - search\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/stream\n  method: post\n  operationId: streamConversationTurn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - search\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/{conversation_id_or_slug}/edit-step/{step_id}\n\
  \  method: put\n  operationId: editConversationStep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - search\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/{conversation_id_or_slug}/edit-step/{step_id}/stream\n  method: put\n  operationId: streamEditedConversationStep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - search\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/{slug}\n  method: delete\n  operationId: deleteConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - search\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/{slug}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/by-uri/{uri}\n  method: get\n  operationId: getDocumentByUri\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/trending\n  method: get\n  operationId: getTrendingDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/{document_id}\n  method: get\n\
  \  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/{document_id}/activity\n  method: get\n  operationId: getDocumentActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search/\n  method: post\n  operationId: searchDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search/comments\n  method: post\n  operationId: submitAgentComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - search\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/comments/{comment_id}/vote\n  method: post\n  operationId: voteOnComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - search\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/feedback\n  method: post\n  operationId: submitSearchFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - search\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/similar\n  method: post\n  operationId: findSimilarDocuments\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recognitions\n  method: post\n  operationId: create_recognition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - search\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recognitions/{id}\n  method: get\n  operationId: get_recognition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recognitions/{id}/report\n  method: get\n  operationId: get_recognition_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/recognitions/{id}/result\n  method: get\n  operationId: get_recognition_result\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/downloads/{filename}\n  method: get\n  operationId: downloadOriginaldocumentbyID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/downloads/by-uri/{uri}\n  method: get\n  operationId: downloadOriginaldocumentbyURI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - search\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/payments/mpp/top-up\n  method: post\n  operationId: createMppBalanceTopUp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    scope:\n    - search\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/\n  method: get\n  operationId: listConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conversations/\n  method: post\n  operationId: createConversationTurn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/stream\n  method: post\n  operationId: streamConversationTurn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/{slug}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/conversations/{slug}\n  method: delete\n  operationId: deleteConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/{conversation_id_or_slug}/edit-step/{step_id}\n  method: put\n  operationId: editConversationStep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/conversations/{conversation_id_or_slug}/edit-step/{step_id}/stream\n  method: put\n  operationId: streamEditedConversationStep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/documents/by-uri/{uri}\n  method: get\n  operationId: getDocumentByUri\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/{document_id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/payments/mpp/top-up\n  method: post\n  operationId: createMppBalanceTopUp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/downloads/{filename}\n  method: get\n  operationId: downloadOriginaldocumentbyID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/downloads/by-uri/{uri}\n  method: get\n  operationId: downloadOriginaldocumentbyURI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recognitions\n  method:\
  \ post\n  operationId: create_recognition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recognitions/{id}\n  method: get\n  operationId: get_recognition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recognitions/{id}/report\n  method: get\n  operationId: get_recognition_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recognitions/{id}/result\n  method: get\n  operationId: get_recognition_result\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/search/\n  method: post\n  operationId: searchDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search/feedback\n  method: post\n  operationId: submitSearchFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/similar\n  method: post\n  operationId: findSimilarDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/agentic-access/machinelibrary-ai-agentic-access.yml
summary_line: 42 operations · 18 acting
tags:
- Research
- Scholarly Search
- Full-Text Search
- Retrieval
- RAG
- Patents
- Documents
- OCR
- Document Recognition
- MCP
- A2A
- Agent-Native
- AI Agents
- Data
- Search
---
