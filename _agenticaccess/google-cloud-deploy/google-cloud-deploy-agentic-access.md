---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: cloud-deploy-api-openapi.yml
  format: yaml
  label: Cloud Deploy API
  slug: cloud-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-deploy/refs/heads/main/openapi/cloud-deploy-api-openapi.yml
consequence_counts:
  physical: 7
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Deploy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{projectId}/locations/{location}/deliveryPipelines
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}/releases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}/releases/{releaseId}/rollouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}/releases/{releaseId}/rollouts/{rolloutId}:approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{projectId}/locations/{location}/targets
operation_count: 12
overview: 'Google Cloud Deploy exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Deploy
provider_slug: google-cloud-deploy
slug: google-cloud-deploy-agentic-access
source_filename: google-cloud-deploy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloud-deploy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 5\n    acting: 7\n  by_consequence:\n    read: 5\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines\n  method: get\n  operationId: listDeliveryPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines\n  method: post\n  operationId: createDeliveryPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}\n  method: get\n  operationId: getDeliveryPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}\n  method: patch\n  operationId: updateDeliveryPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}\n  method: delete\n  operationId: deleteDeliveryPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/locations/{location}/targets\n  method: get\n  operationId: listTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/locations/{location}/targets\n  method: post\n  operationId: createTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}/releases\n  method: get\n  operationId: listReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}/releases\n  method: post\n  operationId: createRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}/releases/{releaseId}/rollouts\n\
  \  method: get\n  operationId: listRollouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}/releases/{releaseId}/rollouts\n  method: post\n  operationId: createRollout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/locations/{location}/deliveryPipelines/{pipelineId}/releases/{releaseId}/rollouts/{rolloutId}:approve\n  method: post\n  operationId: approveRollout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-deploy/refs/heads/main/agentic-access/google-cloud-deploy-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Continuous Delivery
- Deployment
- DevOps
- Kubernetes
- Pipeline
- Release Management
---
