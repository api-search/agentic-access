---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 15
api_specs:
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Pipelines API
  slug: vectorize-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Retrieval API
  slug: vectorize-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Connectors API
  slug: vectorize-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize File Upload API
  slug: vectorize-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Extraction (Iris) API
  slug: vectorize-extraction-iris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Deep Research API
  slug: vectorize-deep-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
consequence_counts:
  read: 15
  safety-critical: 1
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Vectorize Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /org/{organizationId}/pipelines/{pipelineId}/stop
operation_count: 37
overview: 'Vectorize exposes 37 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 21 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vectorize
provider_slug: vectorize-io
slug: vectorize-io-agentic-access
source_filename: vectorize-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vectorize-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    acting: 22\n    connected: 15\n  by_consequence:\n    write: 21\n    read: 15\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /org/{organizationId}/pipelines\n  method: post\n  operationId: createPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/pipelines\n  method: get\n  operationId: getPipelines\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/pipelines/{pipelineId}\n  method: get\n  operationId: getPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/pipelines/{pipelineId}\n  method: delete\n  operationId: deletePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/pipelines/{pipelineId}/start\n  method: post\n  operationId: startPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/pipelines/{pipelineId}/stop\n  method: post\n  operationId: stopPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/{organizationId}/pipelines/{pipelineId}/retrieval\n  method: post\n  operationId: retrieveDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/pipelines/{pipelineId}/deep-research\n\
  \  method: post\n  operationId: startDeepResearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/pipelines/{pipelineId}/deep-research/{researchId}\n  method: get\n  operationId: getDeepResearchResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/pipelines/{pipelineId}/events\n  method: get\n  operationId: getPipelineEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/pipelines/{pipelineId}/metrics\n  method: get\n  operationId: getPipelineMetrics\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/connectors/sources\n  method: post\n  operationId: createSourceConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/sources\n  method: get\n  operationId: getSourceConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/connectors/sources/{sourceConnectorId}\n  method: get\n  operationId: getSourceConnector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /org/{organizationId}/connectors/sources/{sourceConnectorId}\n  method: patch\n  operationId: updateSourceConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/sources/{sourceConnectorId}\n  method: delete\n  operationId: deleteSourceConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/sources/{sourceConnectorId}/users\n  method: post\n  operationId: addUserToSourceConnector\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/sources/{sourceConnectorId}/users\n  method: patch\n  operationId: updateUserInSourceConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/sources/{sourceConnectorId}/users\n  method: delete\n  operationId: deleteUserFromSourceConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/destinations\n  method: post\n  operationId: createDestinationConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/destinations\n  method: get\n  operationId: getDestinationConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/connectors/destinations/{destinationConnectorId}\n  method: get\n  operationId: getDestinationConnector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/connectors/destinations/{destinationConnectorId}\n\
  \  method: patch\n  operationId: updateDestinationConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/destinations/{destinationConnectorId}\n  method: delete\n  operationId: deleteDestinationConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/aiplatforms\n  method: post\n  operationId: createAIPlatformConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/aiplatforms\n  method: get\n  operationId: getAIPlatformConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/connectors/aiplatforms/{aiPlatformConnectorId}\n  method: get\n  operationId: getAIPlatformConnector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/connectors/aiplatforms/{aiPlatformConnectorId}\n  method: patch\n  operationId: updateAIPlatformConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/connectors/aiplatforms/{aiPlatformConnectorId}\n  method: delete\n  operationId: deleteAIPlatformConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/files\n  method: post\n  operationId: startFileUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/uploads/{connectorId}/files\n  method: get\n  operationId: getUploadFilesFromConnector\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/uploads/{connectorId}/files\n  method: put\n  operationId: startFileUploadToConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/uploads/{connectorId}/files/{fileName}\n  method: delete\n  operationId: deleteFileFromConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/extraction\n  method: post\n  operationId: startExtraction\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{organizationId}/extraction/{extractionId}\n  method: get\n  operationId: getExtractionResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/workspaces\n  method: get\n  operationId: getWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{organizationId}/workspaces/{workspaceId}\n  method: get\n  operationId: getWorkspaceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/agentic-access/vectorize-io-agentic-access.yml
summary_line: 37 operations · 22 acting · 1 human-in-the-loop
tags:
- AI
- RAG
- Vectorization
- Embeddings
- Retrieval
- Vector Database
---
