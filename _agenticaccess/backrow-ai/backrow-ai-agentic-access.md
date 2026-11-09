---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 25
api_specs:
- filename: backrow-ai-chat-api-openapi.yml
  format: yaml
  label: Backrow Chat API
  slug: backrow-ai-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-chat-api-openapi.yml
- filename: backrow-ai-credit-transactions-api-openapi.yml
  format: yaml
  label: Backrow Credit Transactions API
  slug: backrow-ai-credit-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-credit-transactions-api-openapi.yml
- filename: backrow-ai-diaries-api-openapi.yml
  format: yaml
  label: Backrow Diaries API
  slug: backrow-ai-diaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-diaries-api-openapi.yml
- filename: backrow-ai-documents-api-openapi.yml
  format: yaml
  label: Backrow Documents API
  slug: backrow-ai-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-documents-api-openapi.yml
- filename: backrow-ai-flashcards-api-openapi.yml
  format: yaml
  label: Backrow Flashcards API
  slug: backrow-ai-flashcards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-flashcards-api-openapi.yml
- filename: backrow-ai-health-api-openapi.yml
  format: yaml
  label: Backrow Health API
  slug: backrow-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-health-api-openapi.yml
- filename: backrow-ai-knowledge-state-api-openapi.yml
  format: yaml
  label: Backrow Knowledge State API
  slug: backrow-ai-knowledge-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-knowledge-state-api-openapi.yml
- filename: backrow-ai-lessons-api-openapi.yml
  format: yaml
  label: Backrow Lessons API
  slug: backrow-ai-lessons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-lessons-api-openapi.yml
- filename: backrow-ai-match-video-api-openapi.yml
  format: yaml
  label: Backrow Match Video API
  slug: backrow-ai-match-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-match-video-api-openapi.yml
- filename: backrow-ai-notes-api-openapi.yml
  format: yaml
  label: Backrow Notes API
  slug: backrow-ai-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-notes-api-openapi.yml
- filename: backrow-ai-paths-api-openapi.yml
  format: yaml
  label: Backrow Paths API
  slug: backrow-ai-paths-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-paths-api-openapi.yml
- filename: backrow-ai-pricing-api-openapi.yml
  format: yaml
  label: Backrow Pricing API
  slug: backrow-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-pricing-api-openapi.yml
- filename: backrow-ai-profile-api-openapi.yml
  format: yaml
  label: Backrow Profile API
  slug: backrow-ai-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-profile-api-openapi.yml
- filename: backrow-ai-quizzes-api-openapi.yml
  format: yaml
  label: Backrow Quizzes API
  slug: backrow-ai-quizzes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-quizzes-api-openapi.yml
- filename: backrow-ai-recommendations-api-openapi.yml
  format: yaml
  label: Backrow Recommendations API
  slug: backrow-ai-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-recommendations-api-openapi.yml
- filename: backrow-ai-recordings-api-openapi.yml
  format: yaml
  label: Backrow Recordings API
  slug: backrow-ai-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-recordings-api-openapi.yml
- filename: backrow-ai-tools-api-openapi.yml
  format: yaml
  label: Backrow Tools API
  slug: backrow-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-tools-api-openapi.yml
- filename: backrow-ai-webhooks-api-openapi.yml
  format: yaml
  label: Backrow Webhooks API
  slug: backrow-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backrow-ai/openapi/backrow-ai-webhooks-api-openapi.yml
consequence_counts:
  physical: 5
  read: 25
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Backrow Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chat
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /lessons/{id}/transform
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /notes/{id}/transform
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /recordings
operation_count: 43
overview: 'Backrow exposes 43 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 13 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Backrow
provider_slug: backrow-ai
slug: backrow-ai-agentic-access
source_filename: backrow-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/backrow-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 25\n    acting: 18\n  by_consequence:\n    read: 25\n    write: 13\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId:\
  \ getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paths\n  method: get\n  operationId: getPaths\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paths\n  method: post\n  operationId: postPaths\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paths/{id}\n  method: get\n  operationId: getPathsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paths/{id}/quizzes\n  method: get\n  operationId: getPathsByIdQuizzes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recommendations\n  method: get\n  operationId: getRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit-transactions\n  method: get\n  operationId: getCreditTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /match-video\n  method: post\n  operationId: postMatchVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /webhooks\n  method: post\n  operationId: postWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhooksById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /knowledge-state\n  method: get\n  operationId: getKnowledgeState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quizzes/submit\n  method: post\n  operationId: postQuizzesSubmit\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notes\n  method: get\n  operationId: getNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notes\n  method: post\n  operationId: postNotes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notes/{id}\n  method: get\n  operationId: getNotesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /notes/{id}\n  method: delete\n  operationId: deleteNotesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notes/{id}/transform\n  method: post\n  operationId: postNotesByIdTransform\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /diaries\n  method: post\n  operationId: postDiaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /diaries\n  method: get\n  operationId: getDiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diaries/{id}\n  method: get\n  operationId: getDiariesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lessons/transformations/catalog\n  method: get\n  operationId: getLessonsTransformationsCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lessons\n  method: get\n  operationId: getLessons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lessons/{id}/transformations\n\
  \  method: get\n  operationId: getLessonsByIdTransformations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lessons/{id}/transform\n  method: post\n  operationId: postLessonsByIdTransform\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools\n  method: get\n  operationId: getTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/run\n  method: post\n  operationId: postToolsRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat\n  method: post\n  operationId: postChat\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings/upload-url\n  method: post\n  operationId: postRecordingsUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings\n  method: post\n  operationId: postRecordings\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings\n  method: get\n  operationId: getRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordings/{id}\n  method: get\n  operationId: getRecordingsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/upload-url\n  method: post\n  operationId: postDocumentsUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: post\n  operationId: postDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}\n  method: get\n  operationId: getDocumentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flashcards/decks\n  method: get\n  operationId: getFlashcardsDecks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flashcards/decks\n  method: post\n  operationId: postFlashcardsDecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flashcards/decks/{id}/cards\n  method: post\n  operationId: postFlashcardsDecksByIdCards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flashcards/due\n  method: get\n  operationId: getFlashcardsDue\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flashcards/review\n  method: post\n  operationId: postFlashcardsReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/backrow-ai/agentic-access/backrow-ai-agentic-access.yml
summary_line: 43 operations · 18 acting
tags:
- Artificial Intelligence
- Productivity
- Education
- Knowledge Management
- Software-as-a-Service
---
