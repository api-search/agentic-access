---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 20
api_specs:
- filename: civitai-blobs-api-openapi.yml
  format: yaml
  label: Civitai Blobs API
  slug: civitai-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-blobs-api-openapi.yml
- filename: civitai-creators-api-openapi.yml
  format: yaml
  label: Civitai Creators API
  slug: civitai-creators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-creators-api-openapi.yml
- filename: civitai-enums-api-openapi.yml
  format: yaml
  label: Civitai Enums API
  slug: civitai-enums-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-enums-api-openapi.yml
- filename: civitai-images-api-openapi.yml
  format: yaml
  label: Civitai Images API
  slug: civitai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-images-api-openapi.yml
- filename: civitai-models-api-openapi.yml
  format: yaml
  label: Civitai Models API
  slug: civitai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-models-api-openapi.yml
- filename: civitai-modelversions-api-openapi.yml
  format: yaml
  label: Civitai ModelVersions API
  slug: civitai-modelversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-modelversions-api-openapi.yml
- filename: civitai-permissions-api-openapi.yml
  format: yaml
  label: Civitai Permissions API
  slug: civitai-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-permissions-api-openapi.yml
- filename: civitai-tags-api-openapi.yml
  format: yaml
  label: Civitai Tags API
  slug: civitai-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-tags-api-openapi.yml
- filename: civitai-users-api-openapi.yml
  format: yaml
  label: Civitai Users API
  slug: civitai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-users-api-openapi.yml
- filename: civitai-vault-api-openapi.yml
  format: yaml
  label: Civitai Vault API
  slug: civitai-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-vault-api-openapi.yml
- filename: civitai-workflows-api-openapi.yml
  format: yaml
  label: Civitai Workflows API
  slug: civitai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/openapi/civitai-workflows-api-openapi.yml
consequence_counts:
  read: 20
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Civitai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'Civitai exposes 29 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Civitai
provider_slug: civitai
slug: civitai-agentic-access
source_filename: civitai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/civitai-orchestration-api-openapi.yml, openapi/civitai-site-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 9\n    connected: 20\n  by_consequence:\n    write: 9\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/consumer/workflows\n  method: post\n  operationId: submitWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/consumer/workflows\n  method: get\n  operationId:\
  \ queryWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/consumer/workflows/{workflowId}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/consumer/workflows/{workflowId}\n  method: put\n  operationId: updateWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/consumer/workflows/{workflowId}\n  method: patch\n  operationId: patchWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/consumer/workflows/{workflowId}\n  method: delete\n  operationId: deleteWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/consumer/blobs\n  method: post\n  operationId: uploadBlob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/consumer/blobs/upload-url\n  method: get\n  operationId: getBlobUploadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/consumer/blobs/{blobId}\n  method: get\n  operationId: getBlob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/consumer/blobs/{blobId}\n  method: head\n  operationId: headBlob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/consumer/blobs/{blobId}/refresh\n  method: post\n  operationId: refreshBlob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{id}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model-versions/{id}\n  method: get\n  operationId: getModelVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model-versions/mini/{id}\n  method: get\n  operationId: getModelVersionMini\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model-versions/by-hash/{hash}\n  method: get\n  operationId: getModelVersionByHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /model-versions/by-hash\n  method: post\n  operationId: getModelVersionsByHashes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model-versions/by-hash/ids\n  method: post\n  operationId: getModelVersionIdsByHashes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images\n  method: get\n  operationId: listImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creators\n  method: get\n  operationId: listCreators\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /permissions/check\n  method: get\n  operationId: checkPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vault/get\n \
  \ method: get\n  operationId: getVaultItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vault/all\n  method: get\n  operationId: getAllVaultItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vault/check-vault\n  method: get\n  operationId: checkVault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vault/toggle-version\n  method: post\n  operationId: toggleVaultVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enums\n  method:\
  \ get\n  operationId: getEnums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/agentic-access/civitai-agentic-access.yml
summary_line: 29 operations · 9 acting
tags:
- Artificial Intelligence
- Image-Generation
- Video Generation
- Stable Diffusion
- SDXL
- Flux
- LoRA
- Model Hosting
- Community
- Generative AI
---
