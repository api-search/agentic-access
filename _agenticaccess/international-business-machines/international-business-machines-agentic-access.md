---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 22
api_specs:
- filename: ibm-watsonx-ai-openapi.yml
  format: yaml
  label: IBM Watsonx.ai API
  slug: watsonx-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-watsonx-ai-openapi.yml
- filename: ibm-watsonx-assistant-openapi.yml
  format: yaml
  label: IBM Watsonx Assistant V2 API
  slug: watsonx-assistant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-watsonx-assistant-openapi.yml
- filename: ibm-natural-language-understanding-openapi.yml
  format: yaml
  label: IBM Natural Language Understanding API
  slug: natural-language-understanding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-natural-language-understanding-openapi.yml
- filename: ibm-speech-to-text-openapi.yml
  format: yaml
  label: IBM Speech to Text API
  slug: speech-to-text
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-speech-to-text-openapi.yml
- filename: ibm-text-to-speech-openapi.yml
  format: yaml
  label: IBM Text to Speech API
  slug: text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-text-to-speech-openapi.yml
- filename: ibm-cloud-object-storage-openapi.yml
  format: yaml
  label: IBM Cloud Object Storage API
  slug: cloud-object-storage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-cloud-object-storage-openapi.yml
- filename: ibm-kubernetes-service-openapi.yml
  format: yaml
  label: IBM Cloud Kubernetes Service API
  slug: kubernetes-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-kubernetes-service-openapi.yml
- filename: ibm-vpc-openapi.yml
  format: yaml
  label: IBM Cloud VPC API
  slug: vpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/openapi/ibm-vpc-openapi.yml
consequence_counts:
  physical: 2
  read: 22
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: International Business Machines Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/assistants/{assistant_id}/message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/assistants/{assistant_id}/sessions/{session_id}/message
operation_count: 42
overview: 'International Business Machines exposes 42 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 18 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: International Business Machines
provider_slug: international-business-machines
slug: international-business-machines-agentic-access
source_filename: international-business-machines-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ibm-cloud-object-storage-openapi.yml, openapi/ibm-kubernetes-service-openapi.yml,\n  openapi/ibm-natural-language-understanding-openapi.yml, openapi/ibm-speech-to-text-openapi.yml,\n  openapi/ibm-text-to-speech-openapi.yml, openapi/ibm-vpc-openapi.yml, openapi/ibm-watsonx-ai-openapi.yml,\n  openapi/ibm-watsonx-assistant-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 22\n    acting: 20\n  by_consequence:\n    read: 22\n    write: 18\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: listBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}\n  method: put\n  operationId: createBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}\n  method: delete\n  operationId: deleteBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}\n  method: get\n  operationId: listObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}/{key}\n  method: put\n  operationId:\
  \ putObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}\n  method: get\n  operationId: getObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}/{key}\n  method: delete\n  operationId: deleteObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/getClusters\n  method: get\n  operationId: getClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/getCluster\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/createCluster\n  method: post\n  operationId: createCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/removeCluster\n  method: delete\n  operationId: removeCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/getWorkers\n\
  \  method: get\n  operationId: getWorkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/getWorkerPools\n  method: get\n  operationId: getWorkerPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyze\n  method: post\n  operationId: analyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models/sentiment\n  method: get\n  operationId: listSentimentModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/categories\n\
  \  method: get\n  operationId: listCategoriesModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recognize\n  method: post\n  operationId: recognize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/{model_id}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customizations\n  method:\
  \ get\n  operationId: listLanguageModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customizations\n  method: post\n  operationId: createLanguageModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/synthesize\n  method: post\n  operationId: synthesize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voices\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/voices/{voice}\n  method: get\n  operationId: getVoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pronunciation\n  method: get\n  operationId: getPronunciation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vpcs\n  method: get\n  operationId: listVpcs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vpcs\n  method: post\n  operationId: createVpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/instances\n  method: get\n  operationId: listInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instances\n  method: post\n  operationId: createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subnets\n  method: get\n  operationId: listSubnets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/security_groups\n  method: get\n  operationId: listSecurityGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/volumes\n  method: get\n  operationId: listVolumes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ml/v1/text/generation\n  method: post\n  operationId: textGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ml/v1/text/generation_stream\n  method: post\n  operationId: textGenerationStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /ml/v1/text/embeddings\n  method: post\n  operationId: textEmbeddings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ml/v1/foundation_model_specs\n  method: get\n  operationId: listFoundationModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ml/v1/text/tokenization\n  method: post\n  operationId: textTokenization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assistants/{assistant_id}/sessions\n\
  \  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assistants/{assistant_id}/sessions/{session_id}\n  method: delete\n  operationId: deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assistants/{assistant_id}/sessions/{session_id}/message\n  method: post\n  operationId: message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assistants/{assistant_id}/message\n  method: post\n  operationId: messageStateless\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assistants/{assistant_id}/environments\n  method: get\n  operationId: listEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/agentic-access/international-business-machines-agentic-access.yml
summary_line: 42 operations · 20 acting
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
---
