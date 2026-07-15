---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 10
api_specs:
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Projects API
  slug: openlayer-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Inference Pipelines API
  slug: openlayer-inference-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Data Stream API
  slug: openlayer-data-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
- filename: openlayer-openapi.yml
  format: yaml
  label: Openlayer Commits and Test Results API
  slug: openlayer-commits-test-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/openapi/openlayer-openapi.yml
consequence_counts:
  read: 10
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openlayer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Openlayer exposes 24 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Openlayer
provider_slug: openlayer
slug: openlayer-agentic-access
source_filename: openlayer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openlayer-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 10\n    acting: 14\n  by_consequence:\n    read: 10\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/versions\n  method: get\n  operationId: listCommits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/versions\n  method: post\n  operationId: createCommit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /projects/{projectId}/inference-pipelines\n  method: get\n  operationId: listInferencePipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/inference-pipelines\n  method: post\n  operationId: createInferencePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/tests\n  method: get\n  operationId: listTests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/tests\n  method: post\n  operationId: createTest\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/tests\n  method: put\n  operationId: updateTests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /versions/{projectVersionId}\n  method: get\n  operationId: retrieveCommit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /versions/{projectVersionId}/results\n  method: get\n  operationId: listCommitTestResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inference-pipelines/{inferencePipelineId}\n  method: get\n  operationId: retrieveInferencePipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inference-pipelines/{inferencePipelineId}\n  method: put\n  operationId: updateInferencePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inference-pipelines/{inferencePipelineId}\n  method: delete\n  operationId: deleteInferencePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inference-pipelines/{inferencePipelineId}/data-stream\n  method: post\n  operationId: streamData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inference-pipelines/{inferencePipelineId}/rows\n  method: post\n  operationId: streamRows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inference-pipelines/{inferencePipelineId}/rows\n  method: put\n  operationId: updateRow\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inference-pipelines/{inferencePipelineId}/rows/{inferenceId}\n  method: get\n  operationId: retrieveRow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inference-pipelines/{inferencePipelineId}/rows/{inferenceId}\n  method: delete\n  operationId: deleteRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inference-pipelines/{inferencePipelineId}/results\n  method: get\n  operationId: listInferencePipelineTestResults\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tests/{testId}/evaluate\n  method: post\n  operationId: evaluateTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tests/{testId}/results\n  method: get\n  operationId: listTestResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/presigned-url\n  method: post\n  operationId: createPresignedUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openlayer/refs/heads/main/agentic-access/openlayer-agentic-access.yml
summary_line: 24 operations · 14 acting
tags:
- AI
- Evaluation
- Testing
- Observability
- LLM
- MLOps
---
