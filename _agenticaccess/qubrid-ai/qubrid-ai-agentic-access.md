---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 15
api_specs:
- filename: qubrid-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Qubrid AI Chat Completions API
  slug: qubrid-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-chat-completions-api-openapi.yml
- filename: qubrid-ai-datasets-api-openapi.yml
  format: yaml
  label: Qubrid AI Datasets API
  slug: qubrid-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-datasets-api-openapi.yml
- filename: qubrid-ai-documents-api-openapi.yml
  format: yaml
  label: Qubrid AI Documents API
  slug: qubrid-ai-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-documents-api-openapi.yml
- filename: qubrid-ai-embeddings-api-openapi.yml
  format: yaml
  label: Qubrid AI Embeddings API
  slug: qubrid-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-embeddings-api-openapi.yml
- filename: qubrid-ai-fine-tuned-models-api-openapi.yml
  format: yaml
  label: Qubrid AI Fine-Tuned Models API
  slug: qubrid-ai-fine-tuned-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-fine-tuned-models-api-openapi.yml
- filename: qubrid-ai-fine-tuning-jobs-api-openapi.yml
  format: yaml
  label: Qubrid AI Fine-Tuning Jobs API
  slug: qubrid-ai-fine-tuning-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-fine-tuning-jobs-api-openapi.yml
- filename: qubrid-ai-gpu-catalog-api-openapi.yml
  format: yaml
  label: Qubrid AI GPU Catalog API
  slug: qubrid-ai-gpu-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-gpu-catalog-api-openapi.yml
- filename: qubrid-ai-instances-api-openapi.yml
  format: yaml
  label: Qubrid AI Instances API
  slug: qubrid-ai-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-instances-api-openapi.yml
- filename: qubrid-ai-knowledge-bases-api-openapi.yml
  format: yaml
  label: Qubrid AI Knowledge Bases API
  slug: qubrid-ai-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-knowledge-bases-api-openapi.yml
- filename: qubrid-ai-models-api-openapi.yml
  format: yaml
  label: Qubrid AI Models API
  slug: qubrid-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-models-api-openapi.yml
- filename: qubrid-ai-rag-queries-api-openapi.yml
  format: yaml
  label: Qubrid AI RAG Queries API
  slug: qubrid-ai-rag-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-rag-queries-api-openapi.yml
- filename: qubrid-ai-ssh-keys-api-openapi.yml
  format: yaml
  label: Qubrid AI SSH Keys API
  slug: qubrid-ai-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-ssh-keys-api-openapi.yml
- filename: qubrid-ai-templates-api-openapi.yml
  format: yaml
  label: Qubrid AI Templates API
  slug: qubrid-ai-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/openapi/qubrid-ai-templates-api-openapi.yml
consequence_counts:
  read: 15
  safety-critical: 2
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Qubrid Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /instances/{instance_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /instances/{instance_id}/stop
operation_count: 33
overview: 'Qubrid AI exposes 33 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 16 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qubrid AI
provider_slug: qubrid-ai
slug: qubrid-ai-agentic-access
source_filename: qubrid-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/qubrid-ai-compute-openapi.yml, openapi/qubrid-ai-fine-tuning-openapi.yml, openapi/qubrid-ai-inference-openapi.yml,\n  openapi/qubrid-ai-rag-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 15\n    acting: 18\n  by_consequence:\n    read: 15\n    write: 16\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /instances\n  method: get\n  operationId: listInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances\n  method: post\n  operationId: createInstance\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}\n  method: get\n  operationId: getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances/{instance_id}\n  method: delete\n  operationId: deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /instances/{instance_id}/start\n  method: post\n  operationId: startInstance\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances/{instance_id}/stop\n  method: post\n  operationId: stopInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gpus\n  method: get\n  operationId: listGpuTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /ssh-keys\n  method: get\n  operationId: listSshKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ssh-keys\n  method: post\n  operationId: createSshKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ssh-keys/{key_id}\n  method: delete\n  operationId: deleteSshKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fine-tuning/jobs\n  method: get\n  operationId: listFineTuningJobs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fine-tuning/jobs\n  method: post\n  operationId: createFineTuningJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fine-tuning/jobs/{job_id}\n  method: get\n  operationId: getFineTuningJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fine-tuning/jobs/{job_id}/cancel\n  method: post\n  operationId: cancelFineTuningJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fine-tuning/datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fine-tuning/datasets\n  method: post\n  operationId: uploadDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fine-tuning/datasets/{dataset_id}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fine-tuning/datasets/{dataset_id}\n  method: delete\n  operationId: deleteDataset\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fine-tuning/models\n  method: get\n  operationId: listFineTunedModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fine-tuning/models/{model_id}\n  method: delete\n  operationId: deleteFineTunedModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model_id}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rag/knowledge-bases\n\
  \  method: get\n  operationId: listKnowledgeBases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rag/knowledge-bases\n  method: post\n  operationId: createKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rag/knowledge-bases/{knowledge_base_id}\n  method: get\n  operationId: getKnowledgeBase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rag/knowledge-bases/{knowledge_base_id}\n  method: delete\n  operationId: deleteKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rag/knowledge-bases/{knowledge_base_id}/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rag/knowledge-bases/{knowledge_base_id}/documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rag/knowledge-bases/{knowledge_base_id}/documents/{document_id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rag/query\n  method: post\n  operationId: queryRag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qubrid-ai/refs/heads/main/agentic-access/qubrid-ai-agentic-access.yml
summary_line: 33 operations · 18 acting · 2 human-in-the-loop
tags:
- Artificial Intelligence
- Cloud Computing
- GPU
- Inference
- Large Language Models
- Machine Learning
- NVIDIA
- Serverless
---
