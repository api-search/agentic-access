---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 32
api_specs:
- filename: jasper-da-com-attachments-api-openapi.yml
  format: yaml
  label: Jasper Attachments API
  slug: jasper-da-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-attachments-api-openapi.yml
- filename: jasper-da-com-audiences-api-openapi.yml
  format: yaml
  label: Jasper Audiences API
  slug: jasper-da-com-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-audiences-api-openapi.yml
- filename: jasper-da-com-command-api-openapi.yml
  format: yaml
  label: Jasper Command API
  slug: jasper-da-com-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-command-api-openapi.yml
- filename: jasper-da-com-context-sources-api-openapi.yml
  format: yaml
  label: Jasper Context Sources API
  slug: jasper-da-com-context-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-context-sources-api-openapi.yml
- filename: jasper-da-com-documents-api-openapi.yml
  format: yaml
  label: Jasper Documents API
  slug: jasper-da-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-documents-api-openapi.yml
- filename: jasper-da-com-geo-api-openapi.yml
  format: yaml
  label: Jasper GEO API
  slug: jasper-da-com-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-geo-api-openapi.yml
- filename: jasper-da-com-image-templates-api-openapi.yml
  format: yaml
  label: Jasper Image Templates API
  slug: jasper-da-com-image-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-image-templates-api-openapi.yml
- filename: jasper-da-com-images-api-openapi.yml
  format: yaml
  label: Jasper Images API
  slug: jasper-da-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-images-api-openapi.yml
- filename: jasper-da-com-knowledge-api-openapi.yml
  format: yaml
  label: Jasper Knowledge API
  slug: jasper-da-com-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-knowledge-api-openapi.yml
- filename: jasper-da-com-products-api-openapi.yml
  format: yaml
  label: Jasper Products API
  slug: jasper-da-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-products-api-openapi.yml
- filename: jasper-da-com-projects-api-openapi.yml
  format: yaml
  label: Jasper Projects API
  slug: jasper-da-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-projects-api-openapi.yml
- filename: jasper-da-com-styles-api-openapi.yml
  format: yaml
  label: Jasper Styles API
  slug: jasper-da-com-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-styles-api-openapi.yml
- filename: jasper-da-com-tasks-api-openapi.yml
  format: yaml
  label: Jasper Tasks API
  slug: jasper-da-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-tasks-api-openapi.yml
- filename: jasper-da-com-templates-api-openapi.yml
  format: yaml
  label: Jasper Templates API
  slug: jasper-da-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-templates-api-openapi.yml
- filename: jasper-da-com-usage-api-openapi.yml
  format: yaml
  label: Jasper Usage API
  slug: jasper-da-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-usage-api-openapi.yml
- filename: jasper-da-com-users-api-openapi.yml
  format: yaml
  label: Jasper Users API
  slug: jasper-da-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-users-api-openapi.yml
- filename: jasper-da-com-voices-api-openapi.yml
  format: yaml
  label: Jasper Voices API
  slug: jasper-da-com-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-voices-api-openapi.yml
consequence_counts:
  read: 32
  write: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jasper Da Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 65
overview: 'Jasper exposes 65 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read and 33 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jasper
provider_slug: jasper-da-com
slug: jasper-da-com-agentic-access
source_filename: jasper-da-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: generated\nsource: openapi/jasper-da-com-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    acting: 33\n    connected: 32\n  by_consequence:\n    write: 33\n    read: 32\n  human_in_the_loop_required: 0\noperations:\n- path: /beta/image-template/render\n  method: post\n  operationId: renderImageTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attachments\n  method: post\n  operationId: createAttachment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences\n  method: get\n  operationId: getAllAudiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/{audienceId}\n  method: get\n  operationId: getAudienceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/command\n  method: post\n  operationId: command\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/context-sources\n  method: post\n  operationId: createContextSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/context-sources/{sourceId}\n  method: get\n  operationId: getContextSourceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents\n  method: get\n  operationId: getAllDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{documentId}\n  method: get\n  operationId: getDocumentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{documentId}\n  method: patch\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/documents/{documentId}\n  method: delete\n  operationId: deleteDocumentById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/geo/analyses\n  method: get\n  operationId: listAnalyses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geo/analyses\n  method: post\n  operationId: createAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/geo/analyses/summary\n  method: get\n  operationId: listAnalysisSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geo/analyses/{configId}\n  method: get\n  operationId: getAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geo/analyses/{configId}\n  method: patch\n  operationId: updateAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/geo/analyses/{configId}\n  method: delete\n  operationId:\
  \ deleteAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/geo/analyses/{configId}/runs\n  method: get\n  operationId: listRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geo/analyses/{configId}/runs/{runId}\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geo/analyses/{configId}/runs/{runId}/claims\n  method: get\n  operationId: getRunClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geo/analyses/{configId}/runs/{runId}/recommendations\n  method: get\n  operationId: getRunRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geo/analyses/{configId}/trends\n  method: get\n  operationId: getTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/image/cleanup\n  method: post\n  operationId: cleanup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/image/decompose\n  method: post\n  operationId: decompose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/packshot-compositing\n  method: post\n  operationId: packshotCompositing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/remove-background\n  method: post\n  operationId: removeBackground\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/remove-text\n  method: post\n  operationId: removeText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/replace-background\n  method: post\n  operationId: replaceBackground\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/uncrop\n  method: post\n  operationId: uncrop\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/upscale\n  method: post\n  operationId: upscale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/knowledge\n  method: post\n  operationId: uploadKnowledgeDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/knowledge\n  method: get\n  operationId: getKnowledgeDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/knowledge/search\n  method: post\n  operationId: searchKnowledge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/knowledge/{knowledgeId}\n  method: get\n  operationId: getKnowledgeDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/knowledge/{knowledgeId}\n  method: patch\n  operationId: updateKnowledgeDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/knowledge/{knowledgeId}\n  method: delete\n  operationId: deleteKnowledgeDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/products\n  method: get\n  operationId: getAllProducts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/attributes\n  method: get\n  operationId: getProductAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{productId}\n  method: get\n  operationId: getProductById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{productId}\n  method: patch\n  operationId: updateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/products/{productId}\n  method: delete\n  operationId: deleteProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects\n  method: get\n  operationId: getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{id}\n  method: get\n  operationId: getProjectById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{id}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{id}\n  method: patch\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/styles\n  method: get\n  operationId: getStyle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/styles/{styleId}\n  method: get\n  operationId: getStyleById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tasks/{id}\n  method: get\n  operationId: getTaskById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/tasks/{id}/run\n  method: post\n  operationId: runTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tasks/{id}/run/stream\n  method: post\n  operationId: runTaskStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates\n  method: get\n  operationId: getAllTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates/{templateId}\n\
  \  method: get\n  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates/{templateId}/run\n  method: post\n  operationId: completeTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tones\n  method: post\n  operationId: createTone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tones\n  method: get\n\
  \  operationId: getAllTones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tones/{toneId}\n  method: get\n  operationId: getTone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tones/{toneId}\n  method: patch\n  operationId: updateTone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tones/{toneId}\n  method: delete\n  operationId: deleteTone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: get\n  operationId: getAllUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/jasper-da-com/agentic-access/jasper-da-com-agentic-access.yml
summary_line: 65 operations · 33 acting
tags:
- Artificial Intelligence
- Marketing
- Automation
- Content
- Platform
- Company
---
