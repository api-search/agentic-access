---
acting_count: 227
action_class_counts:
  acting: 227
  connected: 184
api_specs:
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Chat Completions API
  slug: fireworks-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Completions API
  slug: fireworks-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Vision API
  slug: fireworks-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Embeddings API
  slug: fireworks-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Rerank API
  slug: fireworks-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Images API
  slug: fireworks-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Audio API
  slug: fireworks-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Batch Inference API
  slug: fireworks-batch-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Fine-Tuning API
  slug: fireworks-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Files API
  slug: fireworks-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Models API
  slug: fireworks-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Deployments API
  slug: fireworks-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Account API
  slug: fireworks-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
consequence_counts:
  physical: 42
  read: 184
  safety-critical: 2
  write: 183
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Fireworks Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/accounts/{account_id}/deployments/{deployment_id}/ledger
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/accounts/{account_id}/deployments/{deployment_id}/ledger
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{account_id}/deployedModels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{account_id}/deployedModels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deployedModels/{deployed_model_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/accounts/{account_id}/deployedModels/{deployed_model_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deployedModels/{deployed_model_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/accounts/{account_id}/deployedModels/{deployed_model_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{account_id}/deploymentShapes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{account_id}/deploymentShapes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}/versions/{version_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}/versions/{version_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{account_id}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{account_id}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/accounts/{account_id}/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/accounts/{account_id}/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deployments/{deployment_id}:scale
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/deployments/{deployment_id}:scale
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{account_id}/deployments/{deployment_id}:undelete
operation_count: 411
overview: 'Fireworks AI exposes 411 API operations that an AI agent could call, of which 227 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 184 read, 183 write, 42 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fireworks AI
provider_slug: fireworks-ai
slug: fireworks-ai-agentic-access
source_filename: fireworks-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fireworks-ai-anthropic-messages-openapi.json, openapi/fireworks-ai-gateway-openapi.yml,\n  openapi/fireworks-ai-merged-openapi.yml, openapi/fireworks-ai-responses-openapi.yml, openapi/fireworks-ai-text-completion-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 411\n  by_action_class:\n    acting: 227\n    connected: 184\n  by_consequence:\n    write: 183\n    read: 184\n    physical: 42\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/messages\n  method: post\n  operationId: messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts\n  method: get\n  operationId: Gateway_ListAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/refresh\n  method: post\n  operationId: Gateway_RefreshSessionToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/creditCodes:redeem\n  method: post\n  operationId: Gateway_RedeemCreditCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/validateModelConfig\n  method: post\n  operationId: Gateway_ValidateModelConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}\n  method: get\n  operationId: Gateway_GetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/accountUsageFilterOptions\n  method: get\n  operationId: Gateway_GetAccountUsageFilterOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/auditLogs\n \
  \ method: get\n  operationId: Gateway_ListAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/batchInferenceJobs\n  method: get\n  operationId: Gateway_ListBatchInferenceJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/batchInferenceJobs\n  method: post\n  operationId: Gateway_CreateBatchInferenceJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/batchInferenceJobs/{batch_inference_job_id}\n  method: get\n  operationId: Gateway_GetBatchInferenceJob\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/batchInferenceJobs/{batch_inference_job_id}\n  method: delete\n  operationId: Gateway_DeleteBatchInferenceJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/billing/summary\n  method: get\n  operationId: Gateway_GetBillingSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/billingUsage\n  method: get\n  operationId: Gateway_GetAccountUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/checkpoints/{checkpoint_id}:promote\n  method: post\n  operationId: Gateway_PromoteCheckpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/clusters\n  method: get\n  operationId: Gateway_ListClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/clusters\n  method: post\n  operationId: Gateway_CreateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/clusters/{cluster_id}\n  method: get\n  operationId: Gateway_GetCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/clusters/{cluster_id}\n  method: patch\n  operationId: Gateway_UpdateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/clusters/{cluster_id}\n  method: delete\n  operationId: Gateway_DeleteCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/clusters/{cluster_id}:getConnectionInfo\n  method: get\n  operationId: Gateway_GetClusterConnectionInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/creditRedemptions\n  method: get\n  operationId: Gateway_ListCreditRedemptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/datasets\n  method: get\n  operationId: Gateway_ListDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/datasets\n  method: post\n  operationId: Gateway_CreateDataset\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/datasets/{dataset_id}\n  method: get\n  operationId: Gateway_GetDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/datasets/{dataset_id}\n  method: patch\n  operationId: Gateway_UpdateDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/datasets/{dataset_id}\n  method: delete\n  operationId: Gateway_DeleteDataset\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/datasets/{dataset_id}:getDownloadEndpoint\n  method: get\n  operationId: Gateway_GetDatasetDownloadEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/datasets/{dataset_id}:getUploadEndpoint\n  method: post\n  operationId: Gateway_GetDatasetUploadEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/datasets/{dataset_id}:splitDataset\n\
  \  method: post\n  operationId: Gateway_SplitDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/datasets/{dataset_id}:validateUpload\n  method: post\n  operationId: Gateway_ValidateDatasetUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deployedModels\n  method: get\n  operationId: Gateway_ListDeployedModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/accounts/{account_id}/deployedModels\n  method: post\n  operationId: Gateway_CreateDeployedModel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deployedModels/{deployed_model_id}\n  method: get\n  operationId: Gateway_GetDeployedModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deployedModels/{deployed_model_id}\n  method: patch\n  operationId: Gateway_UpdateDeployedModel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deployedModels/{deployed_model_id}\n  method: delete\n  operationId: Gateway_DeleteDeployedModel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deploymentShapes\n  method: get\n  operationId: Gateway_ListDeploymentShapes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deploymentShapes\n  method: post\n  operationId: Gateway_CreateDeploymentShape\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}\n  method: get\n  operationId: Gateway_GetDeploymentShape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}\n  method: patch\n  operationId: Gateway_UpdateDeploymentShape\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}\n  method: delete\n  operationId: Gateway_DeleteDeploymentShape\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}/versions\n  method: get\n  operationId: Gateway_ListDeploymentShapeVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}/versions/{version_id}\n  method: get\n  operationId: Gateway_GetDeploymentShapeVersion\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deploymentShapes/{deployment_shape_id}/versions/{version_id}\n  method: patch\n  operationId: Gateway_UpdateDeploymentShapeVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deployments\n  method: get\n  operationId: Gateway_ListDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deployments\n  method: post\n  operationId: Gateway_CreateDeployment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}\n  method: get\n  operationId: Gateway_GetDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}\n  method: patch\n  operationId: Gateway_UpdateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}\n  method: delete\n  operationId: Gateway_DeleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}/ledger\n  method: get\n  operationId: Gateway_GetLedger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}/ledger\n  method: delete\n  operationId: Gateway_ResetLedger\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}/shards\n  method: get\n  operationId: Gateway_ListDeploymentShards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}/terminationMessage\n  method: get\n  operationId: Gateway_GetTerminationMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}:metrics\n  method: get\n  operationId: Gateway_GetDeploymentMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}:scale\n  method: patch\n  operationId: Gateway_ScaleDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/deployments/{deployment_id}:undelete\n  method: post\n  operationId: Gateway_UndeleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/developerPasses\n  method:\
  \ get\n  operationId: Gateway_ListDeveloperPasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/developerPasses\n  method: post\n  operationId: Gateway_CreateDeveloperPass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/developerPasses/{developer_passe_id}\n  method: get\n  operationId: Gateway_GetDeveloperPass\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/developerPasses/{developer_passe_id}\n  method: patch\n  operationId: Gateway_UpdateDeveloperPass\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/dpoJobs\n  method: get\n  operationId: Gateway_ListDpoJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/dpoJobs\n  method: post\n  operationId: Gateway_CreateDpoJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/dpoJobs/{dpo_job_id}\n  method: get\n  operationId: Gateway_GetDpoJob\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/dpoJobs/{dpo_job_id}\n  method: delete\n  operationId: Gateway_DeleteDpoJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/dpoJobs/{dpo_job_id}:cancel\n  method: post\n  operationId: Gateway_CancelDpoJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/dpoJobs/{dpo_job_id}:getMetricsFileEndpoint\n  method: get\n \
  \ operationId: Gateway_GetDpoJobMetricsFileEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/dpoJobs/{dpo_job_id}:resume\n  method: post\n  operationId: Gateway_ResumeDpoJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluationJobs\n  method: get\n  operationId: Gateway_ListEvaluationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluationJobs\n  method: post\n  operationId: Gateway_CreateEvaluationJob\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluationJobs/{evaluation_job_id}\n  method: get\n  operationId: Gateway_GetEvaluationJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluationJobs/{evaluation_job_id}\n  method: delete\n  operationId: Gateway_DeleteEvaluationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluationJobs/{evaluation_job_id}:getExecutionLogEndpoint\n\
  \  method: get\n  operationId: Gateway_GetEvaluationJobExecutionLogEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluations\n  method: get\n  operationId: Gateway_ListEvaluations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluations\n  method: post\n  operationId: Gateway_CreateEvaluation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluations/{evaluation_id}\n  method: get\n  operationId: Gateway_GetEvaluation\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluations/{evaluation_id}\n  method: delete\n  operationId: Gateway_DeleteEvaluation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluations/{evaluation_id}:preview\n  method: post\n  operationId: Gateway_PreviewEvaluation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluations:validateAssertions\n  method: post\n  operationId:\
  \ Gateway_ValidateAssertions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluators\n  method: get\n  operationId: Gateway_ListEvaluators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluators\n  method: post\n  operationId: Gateway_CreateEvaluator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}\n  method:\
  \ get\n  operationId: Gateway_GetEvaluator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}\n  method: patch\n  operationId: Gateway_UpdateEvaluator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}\n  method: delete\n  operationId: Gateway_DeleteEvaluator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}/versions\n\
  \  method: get\n  operationId: Gateway_ListEvaluatorVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}/versions/{version_id}\n  method: get\n  operationId: Gateway_GetEvaluatorVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}/versions/{version_id}\n  method: delete\n  operationId: Gateway_DeleteEvaluatorVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}/versions/{version_id}:alias\n\
  \  method: post\n  operationId: Gateway_AliasEvaluatorVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}/versions/{version_id}:rollback\n  method: post\n  operationId: Gateway_RollbackEvaluator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}:getBuildLogEndpoint\n  method: get\n  operationId: Gateway_GetEvaluatorBuildLogEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}:getSourceCodeSignedUrl\n  method: get\n  operationId: Gateway_GetEvaluatorSourceCodeEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}:getUploadEndpoint\n  method: post\n  operationId: Gateway_GetEvaluatorUploadEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluators/{evaluator_id}:validateUpload\n  method: post\n  operationId: Gateway_ValidateEvaluatorUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluators:previewEvaluator\n  method: post\n  operationId: Gateway_PreviewEvaluator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/evaluatorsV2\n  method: post\n  operationId: Gateway_CreateEvaluatorV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/genericDeploymentTypes\n\
  \  method: get\n  operationId: Gateway_ListGenericDeploymentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/genericDeploymentTypes\n  method: post\n  operationId: Gateway_CreateGenericDeploymentType\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/genericDeploymentTypes/{generic_deployment_type_id}\n  method: get\n  operationId: Gateway_ListGenericDeploymentTypeVersions\n  x-agentic-acc\n\n# --- truncated at 32 KB (135 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/agentic-access/fireworks-ai-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/agentic-access/fireworks-ai-agentic-access.yml
summary_line: 411 operations · 227 acting · 2 human-in-the-loop
tags:
- AI
- LLM
- Inference
- Multimodal
- Fine-tuning
- GPU
---
