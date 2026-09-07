---
acting_count: 50
action_class_counts:
  acting: 50
  connected: 32
api_specs:
- filename: dify-service-api-openapi.json
  format: json
  label: Dify
  slug: dify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/_original/dify-service-api-openapi.json
- filename: dify-chat-api-openapi.yml
  format: yaml
  label: Dify Chat Messages API
  slug: dify-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-chat-api-openapi.yml
- filename: dify-completion-api-openapi.yml
  format: yaml
  label: Dify Completion Messages API
  slug: dify-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-completion-api-openapi.yml
- filename: dify-conversations-api-openapi.yml
  format: yaml
  label: Dify Conversations API
  slug: dify-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-conversations-api-openapi.yml
- filename: dify-datasets-api-openapi.yml
  format: yaml
  label: Dify Knowledge Bases API
  slug: dify-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-datasets-api-openapi.yml
- filename: dify-files-api-openapi.yml
  format: yaml
  label: Dify Files API
  slug: dify-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-files-api-openapi.yml
- filename: dify-workflows-api-openapi.yml
  format: yaml
  label: Dify Workflow Runs API
  slug: dify-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-workflows-api-openapi.yml
- filename: dify-applications-api-openapi.yml
  format: yaml
  label: Dify Applications API
  slug: dify-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-applications-api-openapi.yml
- filename: dify-annotations-api-openapi.yml
  format: yaml
  label: Dify Annotations API
  slug: dify-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-annotations-api-openapi.yml
- filename: dify-audio-api-openapi.yml
  format: yaml
  label: Dify Audio API
  slug: dify-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-audio-api-openapi.yml
- filename: dify-feedback-api-openapi.yml
  format: yaml
  label: Dify Feedback API
  slug: dify-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-feedback-api-openapi.yml
- filename: dify-end-users-api-openapi.yml
  format: yaml
  label: Dify End Users API
  slug: dify-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-end-users-api-openapi.yml
- filename: dify-human-input-api-openapi.yml
  format: yaml
  label: Dify Human Input API
  slug: dify-human-input-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-human-input-api-openapi.yml
- filename: dify-documents-api-openapi.yml
  format: yaml
  label: Dify Documents API
  slug: dify-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-documents-api-openapi.yml
- filename: dify-chunks-api-openapi.yml
  format: yaml
  label: Dify Chunks API
  slug: dify-chunks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-chunks-api-openapi.yml
- filename: dify-tags-api-openapi.yml
  format: yaml
  label: Dify Knowledge Tags API
  slug: dify-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-tags-api-openapi.yml
- filename: dify-metadata-api-openapi.yml
  format: yaml
  label: Dify Metadata API
  slug: dify-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-metadata-api-openapi.yml
- filename: dify-models-api-openapi.yml
  format: yaml
  label: Dify Models API
  slug: dify-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-models-api-openapi.yml
- filename: dify-knowledge-pipeline-api-openapi.yml
  format: yaml
  label: Dify Knowledge Pipeline API
  slug: dify-knowledge-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-knowledge-pipeline-api-openapi.yml
consequence_counts:
  physical: 2
  read: 32
  safety-critical: 3
  write: 45
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Dify Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /chat-messages/{task_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /completion-messages/{task_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workflows/tasks/{task_id}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chat-messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /completion-messages
operation_count: 82
overview: 'Dify exposes 82 API operations that an AI agent could call, of which 50 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 45 write, 2 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dify
provider_slug: dify
slug: dify-agentic-access
source_filename: dify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: generated\nsource: openapi/dify-annotations-api-openapi.yml, openapi/dify-applications-api-openapi.yml,\n  openapi/dify-audio-api-openapi.yml, openapi/dify-chat-api-openapi.yml, openapi/dify-chunks-api-openapi.yml,\n  openapi/dify-completion-api-openapi.yml, openapi/dify-conversations-api-openapi.yml, openapi/dify-datasets-api-openapi.yml,\n  openapi/dify-documents-api-openapi.yml, openapi/dify-end-users-api-openapi.yml, openapi/dify-feedback-api-openapi.yml,\n  openapi/dify-files-api-openapi.yml, openapi/dify-human-input-api-openapi.yml, openapi/dify-knowledge-pipeline-api-openapi.yml,\n  openapi/dify-metadata-api-openapi.yml, openapi/dify-models-api-openapi.yml, openapi/dify-tags-api-openapi.yml,\n  openapi/dify-workflows-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per\
  \ deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 82\n  by_action_class:\n    acting: 50\n    connected: 32\n  by_consequence:\n    write: 45\n    read: 32\n    physical: 2\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /apps/annotations\n  method: post\n  operationId: createAnnotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/annotations\n  method: get\n  operationId: getAnnotationList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/annotations/{annotation_id}\n  method: put\n  operationId: updateAnnotation\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/annotations/{annotation_id}\n  method: delete\n  operationId: deleteAnnotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/annotation-reply/{action}\n  method: post\n  operationId: initialAnnotationReplySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/annotation-reply/{action}/status/{job_id}\n\
  \  method: get\n  operationId: getInitialAnnotationReplySettingsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info\n  method: get\n  operationId: getChatAppInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parameters\n  method: get\n  operationId: getChatAppParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta\n  method: get\n  operationId: getChatAppMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site\n  method: get\n  operationId: getChatWebAppSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audio-to-text\n  method: post\n  operationId: audioToText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text-to-audio\n  method: post\n  operationId: textToAudioChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat-messages\n  method: post\n  operationId: sendChatMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat-messages/{task_id}/stop\n  method: post\n  operationId: stopChatMessageGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /messages/{message_id}/suggested\n  method: get\n  operationId: getSuggestedQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/documents/{document_id}/segments\n  method: post\n  operationId: createSegments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/{document_id}/segments\n  method: get\n  operationId: listSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/documents/{document_id}/segments/{segment_id}\n  method: get\n  operationId: getSegmentDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/documents/{document_id}/segments/{segment_id}\n  method: post\n  operationId: updateSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/{document_id}/segments/{segment_id}\n  method: delete\n  operationId: deleteSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/{document_id}/segments/{segment_id}/child_chunks\n  method: post\n  operationId: createChildChunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/{document_id}/segments/{segment_id}/child_chunks\n\
  \  method: get\n  operationId: getChildChunks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/documents/{document_id}/segments/{segment_id}/child_chunks/{child_chunk_id}\n  method: patch\n  operationId: updateChildChunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/{document_id}/segments/{segment_id}/child_chunks/{child_chunk_id}\n  method: delete\n  operationId: deleteChildChunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /completion-messages\n  method: post\n  operationId: createCompletionMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /completion-messages/{task_id}/stop\n  method: post\n  operationId: stopGenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /conversations\n  method: get\n  operationId: getConversationsList\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages\n  method: get\n  operationId: getConversationHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/variables\n  method: get\n  operationId: getConversationVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/name\n  method: post\n  operationId: renameConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/variables/{variable_id}\n\
  \  method: put\n  operationId: updateChatConversationVariable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}\n  method: delete\n  operationId: deleteConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}\n  method: get\n  operationId: getDatasetDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}\n  method: patch\n  operationId: updateDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}\n  method: delete\n  operationId: deleteDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/retrieve\n  method: post\n  operationId: retrieveSegments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/document/create-by-text\n  method: post\n  operationId: createDocumentFromText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/document/create-by-file\n\
  \  method: post\n  operationId: createDocumentFromFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/documents/{document_id}\n  method: get\n  operationId: getDocumentDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/documents/{document_id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/{document_id}\n  method: patch\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/{document_id}/download\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/documents/{batch}/indexing-status\n  method: get\n  operationId: getDocumentIndexingStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/documents/{document_id}/update-by-text\n  method: post\n  operationId: updateDocumentByText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/{document_id}/update-by-file\n  method: post\n  operationId: updateDocumentByFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/download-zip\n  method: post\n  operationId: downloadDocumentsZip\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/status/{action}\n  method: patch\n  operationId: batchUpdateDocumentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /end-users/{end_user_id}\n  method: get\n  operationId: getEndUserChat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{message_id}/feedbacks\n  method: post\n  operationId: postChatMessageFeedback\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/feedbacks\n  method: get\n  operationId: getChatAppFeedbacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/upload\n  method: post\n  operationId: uploadChatFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}/preview\n  method: get\n  operationId: previewChatFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /form/human_input/{form_token}\n  method: get\n  operationId: getChatflowHumanInputForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /form/human_input/{form_token}\n  method: post\n  operationId: submitChatflowHumanInputForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/pipeline/file-upload\n  method: post\n  operationId: uploadPipelineFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/pipeline/datasource-plugins\n  method: get\n  operationId: listDatasourcePlugins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/pipeline/datasource/nodes/{node_id}/run\n  method: post\n  operationId: runDatasourceNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/pipeline/run\n  method: post\n  operationId: runPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/metadata\n  method: post\n  operationId: createMetadataField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/metadata\n  method: get\n  operationId: listMetadataFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/metadata/{metadata_id}\n  method: patch\n  operationId: updateMetadataField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/metadata/{metadata_id}\n  method: delete\n  operationId: deleteMetadataField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/metadata/built-in\n  method: get\n  operationId: getBuiltInMetadataFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/metadata/built-in/{action}\n  method: post\n  operationId: toggleBuiltInMetadataField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/documents/metadata\n  method: post\n  operationId: batchUpdateDocumentMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/current/models/model-types/{model_type}\n  method: get\n  operationId: getAvailableModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/tags\n  method: post\n  operationId: createKnowledgeTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/tags\n  method: get\n  operationId: getKnowledgeTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/tags\n  method: patch\n  operationId: updateKnowledgeTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/tags\n  method: delete\n  operationId: deleteKnowledgeTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /datasets/tags/binding\n  method: post\n  operationId: bindTagsToDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/tags/unbinding\n  method: post\n  operationId: unbindTagFromDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{dataset_id}/tags\n  method: get\n  operationId: queryDatasetTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/run/{workflow_run_id}\n  method:\
  \ get\n  operationId: getWorkflowRunDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/logs\n  method: get\n  operationId: getWorkflowLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow/{workflow_run_id}/events\n  method: get\n  operationId: streamWorkflowEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/run\n  method: post\n  operationId: executeWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /workflows/{workflow_id}/run\n  method: post\n  operationId: runWorkflowById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflows/tasks/{task_id}/stop\n  method: post\n  operationId: stopWorkflowTaskGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/agentic-access/dify-agentic-access.yml
summary_line: 82 operations · 50 acting · 3 human-in-the-loop
tags:
- Artificial Intelligence
- LLMOps
- Backend-as-a-Service
- Agents
- Workflows
- Knowledge Management
- RAG
- Model Context Protocol
- Low Code
- Open Source
---
